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
  * GPA: 3.74/4.0
  * Relevant coursework: Natural Language Processing, Bayesian Statistics, Machine Learning, Statistical Inference
* **B.S. in Mathematics & Finance**, University of Liverpool, Sep 2020 - Jun 2024
  * GPA: 3.94/4.0, First Class
  * Relevant coursework: Stochastic Modeling, Real Analysis, Statistical Models, Numerical Methods, Operational Research

Research Experience
======

### Multi-site ICU Electronic Health Record Analysis for Equitable Mortality Prediction

*Duke University, Nov 2025 - Apr 2026. Advised by Drs. Chuan Hong, Deepshikha Ashana, Matthew Engelhard, et al.*

* Studied racial and ethnic bias in ICU mortality risk prediction with the long-term goal of developing equitable, clinically deployable prognostic models.
* Preprocessed large-scale EHR data from Duke University and the Medical University of South Carolina and assisted with cohort construction.
* Evaluated mortality models including SOFA, APACHE II, and Cox proportional hazards models, focusing on robustness and fairness.

### SAGE Structured Agent for Diagnosis-Based EHR Cohort Extraction

*Duke University, Oct 2025 - Present. Advised by Drs. Chuan Hong and Tianxi Cai with Harvard-affiliated investigators.*

* Contributed to a modular, SQL-based agent for cohort identification using ICD-9/10 diagnosis codes and mentored junior students on implementation.
* Assisted with diagnosis-date identification, longitudinal incidence tracking, and multi-source EHR cohort extraction pipelines.
* Supported reusable phenotyping logic for inflammatory bowel disease with extensibility to additional disease phenotypes.

### MOSAIC An Agentic AI for Multi-Framework Communication Analysis

*Duke University, Jan 2025 - May 2026. Advised by Dr. Chuan Hong; collaborated with Drs. Michael Pencina, Kai Sun, and Kathryn Pollak.*

* Developed a LangGraph-based multi-agent framework using retrieval-augmented generation for multi-scale analysis of clinician-patient dialogues.
* Designed dynamic few-shot prompting and domain-adaptive retrieval, evaluating 70 transcripts (approximately 20 hours of audio) and achieving 93%+ human alignment and 90%+ F1.
* Generated aligned multimodal text-audio pairs and compared language models, text-to-speech models, and audio feature analysis methods.
* Contributed to manuscript methods, ablation studies, fairness, robustness, and evaluation; the paper was accepted for publication in *npj Digital Medicine*.

### An Internal Ambient Digital Scribing System

*Duke University, Jan 2025 - Apr 2026. Advised by Dr. Chuan Hong; collaborated with Drs. Michael Pencina, Kai Sun, and Kathryn Pollak.*

* Developed an end-to-end, privacy-safe ambient scribing tool integrating voice activity detection, Whisper-based automatic speech recognition, and speaker diarization.
* Generated structured medical notes for clinicians and implemented human-in-the-loop evaluation to improve factual consistency and transcription accuracy.

### Deep Learning for EEG in Mental Health Disorder Diagnostics

*Stevens Institute of Technology, Jun 2023 - Dec 2023. Advised by Dr. Feng Liu.*

* Investigated statistical, machine learning, and deep learning approaches for EEG-based mental health disorder diagnosis.
* Compared convolutional, recurrent, and graph neural networks for spatial-temporal features and brain connectivity patterns.

### Quantitative Analysis of Carbon Trading and Sustainable Finance

*Xi'an Jiaotong-Liverpool University, Jun 2022 - Sep 2022. Advised by Wen Qian.*

* Analyzed China's carbon market using emissions trajectories, allowance-price dynamics, lagged correlations, and cross-sector co-movements.
* Modeled structural transition risk using clustering and regression and delivered recommendations for financial institutions.

### Machine Learning Model for Credit Default Prediction

*Imperial College London Winter School, Dec 2021 - Mar 2022. Advised by Dr. Zhen Ye.*

* Trained and benchmarked XGBoost, random forest, and logistic regression models on real-world credit data.
* Deployed the final XGBoost model (AUC 0.96; precision 0.93) with FastAPI and Docker.

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

* Technical Skills: Python, PyTorch, R, SQL, Rust, MATLAB, Maple, Docker, Git, AWS
* Languages: English (Proficient), Mandarin (Native), Spanish (Conversational)
* Interests: Climbing, Badminton, Guitar, Reading
