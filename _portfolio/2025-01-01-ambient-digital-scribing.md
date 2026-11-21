---
title: "Mediscribe: Privacy-Safe, Speaker-Attributed Transcription of Clinical Consultations"
excerpt: "Built Mediscribe, a privacy-safe ambient scribing pipeline that turns consultation recordings into speaker- and role-attributed transcripts for clinical review."
collection: portfolio
permalink: /research/ambient-digital-scribing/
date: 2025-01-01
timeline_start: "Jan 2025"
timeline_end: "Apr 2026"
---

`Mediscribe` is a privacy-safe ambient digital scribing pipeline that turns recordings of clinical consultations into speaker-attributed transcripts: who said what, when, and in which clinical role. Its outputs supported clinician-facing structured notes and downstream communication analysis such as [`MOSAIC`]({{ '/research/mosaic/' | relative_url }}), and were refined through human-in-the-loop evaluation with clinicians.

## Version 2: speaker-attributed transcription

The second version, developed with Zhiyi (Bill) Liu, rebuilds the pipeline around accurate word-level timing and transparent speaker evidence.

* **Prepare.** Audio is decoded and resampled to 16 kHz mono on a common time base, with the original recording and file hashes kept for traceability.
* **Transcribe.** Two ASR passes (Whisper and a chunked Parakeet pass) are merged at the word level, keeping words both passes agree on, recovering words one pass missed, and removing duplicates. Optional MMS forced alignment provides word-level timestamps, and Silero voice activity detection filters out non-speech tokens.
* **Diarize.** pyannote (community-1) segments, embeds, and clusters the audio to determine who spoke when, with fixed or bounded speaker counts and explicit overlap regions.
* **Fuse.** Words are assigned to speakers by timing overlap, boundaries are refined and rescored using pause cues and speaker embeddings, and sentences and turns are reconstructed with fragment repair and echo removal.
* **Assign roles.** An LLM, served through a self-hosted vLLM endpoint or any OpenAI-compatible API, infers clinical roles from turn content and speaker similarity. A majority vote over three samples and configurable role definitions make assignments more stable, and speakers are labelled *unknown* when the evidence is weak.
* **Render and review.** The pipeline exports a plain-text transcript and a canonical JSON file with word timestamps and speaker evidence. Reviewers can correct text and speaker labels, with revision history and text or ZIP export.

<figure>
  <a href="{{ '/images/mediscribe-v2-pipeline.svg' | relative_url }}">
    <img src="{{ '/images/mediscribe-v2-pipeline.svg' | relative_url }}" alt="Mediscribe version 2 pipeline: prepare audio, two-pass transcription with Whisper and Parakeet plus forced alignment and voice activity detection, pyannote diarization, word-speaker fusion, LLM-based role assignment with majority voting, and rendered transcripts for manual review" loading="lazy">
  </a>
  <figcaption>Figure 1. The Mediscribe v2 pipeline, from raw consultation audio to reviewed, speaker-attributed transcripts. Select the figure to view it at full resolution.</figcaption>
</figure>

## Version 1: ambient digital scribing

The first version established the end-to-end workflow. An ensemble of voice activity detectors (Pydub, Silero VAD, and SpeechBrain) combined by majority vote produced clean speech. Whisper then generated sentence-level transcripts, while pyannote voice embeddings detected speaker turns. The aligned outputs were turned into a structured, time-stamped transcript, an LLM assigned clinician and patient roles, and the result was chunked for downstream agentic analysis.

<figure>
  <a href="{{ '/images/mediscribe-v1-pipeline.png' | relative_url }}">
    <img src="{{ '/images/mediscribe-v1-pipeline.png' | relative_url }}" alt="Mediscribe version 1 pipeline: majority-vote voice activity detection, Whisper speech recognition, pyannote speaker turn detection, aligned and structured transcripts, LLM speaker role assignment, and chunking for an agentic core" loading="lazy">
  </a>
  <figcaption>Figure 2. The original Mediscribe v1 pipeline. Select the figure to view it at full resolution.</figcaption>
</figure>
