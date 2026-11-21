---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======

* **Ph.D. student in Quantitative Biology and Medicine (Biostatistics)**, Duke-NUS Medical School, Aug 2026 - Present
* **M.S. in Statistical Science**, Duke University, Aug 2024 - May 2026
  * Relevant coursework: Natural Language Processing, Bayesian Statistics, Machine Learning, Statistical Inference
* **B.S. in Mathematics & Finance**, University of Liverpool, Sep 2020 - Jun 2024
  * First Class Honours
  * Relevant coursework: Stochastic Modeling, Real Analysis, Statistical Models, Numerical Methods, Operational Research

Research Experience
======

### Multimodal Image-Clinical Deep Learning for Orthodontic Treatment Duration

*Duke-NUS Medical School, Oct 2026 - Present. Advised by Dr. Bibhas Chakraborty.*

* Leading a multimodal project that predicts orthodontic treatment duration from intraoral photographs and clinical records.
* Building image-clinical fusion models, including vision encoders and small vision-language models.
* Developing survival models that account for patients still in treatment.

### Efficient Multilingual Clinical Communication Coding

*Duke University, Oct 2026 - Present. Advised by Dr. Chuan Hong.*

* Co-first author on an extension of MOSAIC that aims to code clinical communication accurately at lower cost and latency.
* Building a multilingual synthetic benchmark of clinician-patient dialogues across three established communication codebooks.
* Developing lightweight decision models and a confidence-based agentic workflow that sends uncertain cases to stronger LLMs.

### Reinforcement Learning & Randomized Trials for Digital Health Interventions

*Duke-NUS Medical School, Sep 2026 - Present. Advised by Dr. Bibhas Chakraborty.*

* Developing RL algorithms and trial designs for two mHealth studies: COBRA (wearable-based lifestyle intervention) and FamNucleus (postpartum mental-health app).
* Designing micro-randomized trials and adaptive personalization to decide when and how to send nudges.
* Supported EMPOWER, a just-in-time adaptive intervention for physical activity in diabetes care.

### Multi-site ICU Electronic Health Record Analysis for Equitable Mortality Prediction

*Duke University, Nov 2025 - Apr 2026. Advised by Drs. Chuan Hong, Deepshikha Ashana, Matthew Engelhard, et al.*

* Studied racial and ethnic bias in ICU mortality risk prediction with the long-term goal of developing equitable, clinically deployable prognostic models.
* Preprocessed large-scale EHR data from Duke University and the Medical University of South Carolina and assisted with cohort construction.
* Evaluated mortality models including SOFA, APACHE II, and Cox proportional hazards models, focusing on robustness and fairness.

### SAGE Structured Agent for Diagnosis-Based EHR Cohort Extraction

*Duke University, Oct 2025 - Dec 2026. Advised by Drs. Chuan Hong and Tianxi Cai with Harvard-affiliated investigators.*

* Contributed to a modular, SQL-based agent for cohort identification using ICD-9/10 diagnosis codes and mentored junior students on implementation.
* Assisted with diagnosis-date identification, longitudinal incidence tracking, and multi-source EHR cohort extraction pipelines.
* Supported reusable phenotyping logic for inflammatory bowel disease with extensibility to additional disease phenotypes.

### MOSAIC An Agentic AI for Multi-Framework Communication Analysis

*Duke University, Jan 2025 - May 2026. Advised by Dr. Chuan Hong; collaborated with Drs. Michael Pencina, Kai Sun, and Kathryn Pollak.*

* Developed a LangGraph-based multi-agent framework using retrieval-augmented generation for multi-scale analysis of clinician-patient dialogues.
* Designed dynamic few-shot prompting and domain-adaptive retrieval, developing on 54 and evaluating on 120 gold-standard annotated transcripts across rheumatology and OB/GYN, achieving an overall weighted F1 of 95.6%.
* Generated aligned multimodal text-audio pairs and compared language models, text-to-speech models, and audio feature analysis methods.
* First-authored the paper, published in *npj Digital Medicine* (2026); co-authored SIMAX (under review), contributing evaluation and LLM/TTS model comparisons.

### Mediscribe: A Privacy-Safe Ambient Digital Scribing System

*Duke University, Jan 2025 - Apr 2026. Advised by Dr. Chuan Hong; collaborated with Drs. Michael Pencina, Kai Sun, and Kathryn Pollak.*

* Developed an end-to-end, privacy-safe ambient scribing tool integrating voice activity detection, Whisper-based automatic speech recognition, and voice-embedding-powered speaker diarization.
* Used Mediscribe to generate weekly structured notes for clinicians, reducing documentation burden.
* Implemented human-in-the-loop evaluation with clinicians to improve factual consistency and transcription accuracy.

### Deep Learning for EEG in Mental Health Disorder Diagnostics

*Stevens Institute of Technology, Jun 2023 - Dec 2023. Advised by Dr. Feng Liu.*

* Investigated statistical, machine learning, and deep learning approaches for EEG-based mental health disorder diagnosis.
* Compared convolutional, recurrent, and graph neural networks for spatial-temporal features and brain connectivity patterns.

Publications
======

  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Teaching
======

### DEC 546Q Modern Analytics

*Teaching Assistant, Duke University Fuqua School of Business, Oct 2025 - Dec 2025*

* Supported a graduate-level course covering neural networks, diffusion models, large language models, and other machine learning topics.
* Held weekly office hours on model training, regularization, and evaluation in Python.
* Graded coding assignments, case studies, and final projects and provided structured feedback.

Honors & Awards
======

* Sampford Memorial Prize, best final-year student in Statistics & Operational Research, Jul 2024
* University Exchange Scholarship, Top 1%, Jul 2023
* University Academic Excellence Award, Top 1%, Jun 2021 and Jun 2022

Additional Information
======

* Technical Skills: Python (PyTorch), R, SQL, Rust, MATLAB, Maple, Docker, Git, AWS, HPC (SLURM)
* Methods: Survival analysis, causal inference, micro-randomized trials, reinforcement learning (bandits), LLM agents (LangGraph, RAG), LoRA fine-tuning
* Languages: English (Proficient), Mandarin (Native), Spanish (Conversational)
* Interests: Climbing, Badminton, Guitar, Reading
