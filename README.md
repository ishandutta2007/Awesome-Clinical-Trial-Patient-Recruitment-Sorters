# Awesome-Clinical-Trial-Patient-Recruitment-Sorters

## Top Clinical Trial Patient Recruitment Sorters Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on EHR Screening, Eligibility Matching & Trial-to-Patient Fit*  

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Clinical Trial Patient Recruitment Sorters**. These tools parse electronic health records, genomic profiles, and clinical notes to match patients against complex eligibility criteria—reducing screening time and surfacing candidates who would otherwise be missed.



**Examples** include Deep 6 AI, Antidote, Trialbee, Paradigm, Clara Health, SubjectWell, TriNetX, Inato, AutoCruitment, and Reify Health (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, LLM-powered eligibility reasoning, and open trial matching—ideal for research institutions, clinical sites, and developers seeking transparent, vendor-independent recruitment.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Deep 6 AI](https://deep6.ai/)**  

  Clinical trial recruitment platform that parses structured and unstructured EHR data to match patients to trials in minutes. Uses AI to identify candidates from clinical notes, imaging, and genomics that traditional screening misses.



- **[Antidote](https://www.antidote.me/)**  

  Trial matching platform connecting patients to clinical trials. Features trial search, pre-screening questionnaires, and site referral for sponsors and CROs.



- **[Trialbee](https://trialbee.com/)**  

  Patient recruitment and retention platform for clinical trials. Features AI-powered matching, patient engagement, and site support.



- **[Paradigm](https://paradigmhealth.com/)**  

  Patient recruitment platform for oncology and rare disease trials. Features EHR-based pre-screening and site network integration.



- **[Clara Health](https://www.clarahealth.com/)**  

  Patient-facing trial matching platform. Helps patients find and enroll in clinical trials based on their condition and location.



- **[SubjectWell](https://subjectwell.com/)**  

  Patient recruitment marketplace connecting sponsors with patients for clinical trials. Features targeted outreach and pre-qualification.



- **[TriNetX](https://www.trinetx.com/)**  

  Global health research network providing access to de-identified EHR data for trial feasibility and site selection. Enables cohort discovery across 200+ healthcare organizations.



- **[Inato](https://inato.com/)**  

  Clinical trial marketplace connecting sponsors with community sites. Features trial feasibility, site matching, and enrollment analytics.



- **[AutoCruitment](https://autocruitment.com/)**  

  Patient recruitment platform with AI-powered pre-screening and site referral. Features campaign management and enrollment tracking.



- **[Reify Health](https://www.reifyhealth.com/)**  

  Clinical trial infrastructure with patient recruitment and site enablement. Features StudyTeam for site workflows and Care for patient engagement.



## Open-Source GitHub Projects



- **[MatchMiner](https://github.com/matchminer/matchminer)**  

  Open-source AI platform from Dana-Farber Cancer Institute that matches patients to precision oncology trials based on clinical and genomic profiles . **Launched in 2016**, now used at multiple institutions including Princess Margaret Cancer Centre . Original version used rules-based matching on structured data (genomic biomarkers, cancer type). **MatchMiner-AI** now analyzes unstructured clinical notes with LLMs to extract prior treatments, disease stage, and other trial-relevant features . Embedded in Dana-Farber's clinical workflows and supported **400+ patient enrollments**. A 2022 study in NPJ Precision Oncology found patients matched through MatchMiner enrolled **22% faster** than traditional methods .



- **[TrialGPT](https://github.com/ncbi-nlp/TrialGPT)**  

  Open-source LLM framework from NIH/NCBI for clinical trial matching . Three components: **TrialGPT-Retrieval** (hybrid-fusion retrieval recalling **90%+ of relevant trials using <6% of collection**), **TrialGPT-Matching** (criterion-level accuracy of **87.3%** with faithful explanations, close to expert performance of 88.7–90.0%), and **TrialGPT-Ranking** (outperforms best competing models by **28.8–53.5%** in ranking and excluding trials) . User study shows **42.6% reduction in screening time** . Requires OpenAI or Azure OpenAI API (HIPAA-compliant option available) .



- **[Stanford OVAL Clinical Trial Matcher](https://github.com/stanford-oval/clinical-trial-matching)**  

  Open-source matcher developed with Mayo Clinic combining **SatIR** (pure SQL, no LLM, no services) and **VERDICT** (accountable eligibility decisions with grounded rationales) . **SatIR** retrieval recall is checkable against TREC 2022 with reproducible published numbers . **VERDICT** matching accuracy on TREC 2021 held-out test set: **GPT-5-mini VERDICT achieves F1 0.828**; **Qwen2.5-7B with distillation reaches the same F1** (0.828), beating its own end-to-end chain-of-thought by **16.5 points** . Papers: SatIR (arXiv:2604.08849) and VERDICT (arXiv:2609.03366) .



- **[TrialMesh](https://pypi.org/project/trialmesh/)**  

  Open-source complete pipeline for clinical trial matching . Features **summarization** (LLM-based patient and trial summarization), **embedding and indexing** (BGE-large-en-v1.5 with FAISS flat/HNSW indices), and **matching** with configurable inclusion/exclusion/scoring prompts. Supports **Llama-3.3-70B-Instruct** with tensor parallelism for local deployment . Pipeline runs end-to-end from data prep to final matching .



- **[PyTrial](https://github.com/RyanWangZf/PyTrial)**  

  Open-source Python package for AI in drug development including **patient-trial matching** . Matches trial eligibility criteria to patients' EHRs for recruitment . Also supports patient outcome prediction, trial site selection, trial similarity search, and trial data simulation . Based on published research (arXiv:2306.04018) .



- **[CTIMS (Clinical Trial Integrated Matching System)](https://github.com/pughlab/ctims)**  

  Open-source matching system from Pugh Lab (Apache 2.0) . **Multi-institutional collaboration** with Princess Margaret Cancer Center, Dana-Farber, and Memorial Sloan Kettering . Uses **cBioPortal** to display matched patients in patient view. Features **CTML editor** for creating matching files in GUI. Architecture: Nx/Next/Nest monorepo with Docker containers, Keycloak for security . Website: ctims.ca .



- **[CancerTrialMatch](https://github.com/AveraSD/CancerTrialMatch)**  

  Open-source application for biomarker-based trial curation and patient matching (published in Bioinformatics, 2025) . Built with **R Shiny, MongoDB, and Docker** . Retrieves trial data via **clinicaltrials.gov API**, with manual entry for biomarkers and disease subtypes using **OncoTree classification** . Reduces institutional trial management time and supports precision oncology enrollment .



- **[John Snow Labs Clinical Trial Matching](https://www.johnsnowlabs.com/clinical-trial-matching/)**  

  Hybrid approach using **OMOP SQL queries** for structured data and **NLP/LLM prompts** for clinical notes . Every criterion evaluated across full patient record with evidence tied to source . Runs **inside your environment** (on-prem, AWS, Azure, Databricks, Snowflake, air-gapped)—no patient data or prompts leave perimeter . Features auditable decisions, reusable cohorts, and manual review flagging for criteria requiring human judgment (willingness, consent, literacy) .



### Additional Strong Open-Source Options



- **[OpenClinica / LibreClinica](https://github.com/OpenClinica/OpenClinica)** — Open-source clinical trial software for Electronic Data Capture (EDC) and Clinical Data Management (CDM) . LibreClinica is the community-driven successor .

- **[Phoenix CTMS](https://github.com/phoenixctms)** — Open-source CTMS/PRS/CDMS .

- Community **n8n** workflows for trial matching alerting and patient pre-screening automation.



**Frameworks for building custom systems**: Combine **MatchMiner** for clinical-genomic matching with **TrialGPT** for LLM-based eligibility reasoning, **Stanford OVAL Matcher** for reproducible retrieval and accountable decisions, **TrialMesh** for local LLM deployment, and **PostgreSQL/OMOP** for persistence—creating a fully self-hosted, enterprise-grade trial recruitment platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Clinical trial recruitment systems handling patient data must comply with HIPAA, GDPR, 21 CFR Part 11, and institutional review board (IRB) requirements.

- **Open-source trial matching is advancing rapidly but remains research-stage for clinical deployment.** MatchMiner is the most clinically validated open-source platform (400+ enrollments, 22% faster enrollment) . TrialGPT and Stanford OVAL Matcher achieve near-expert accuracy on benchmark datasets but require validation on local patient populations before clinical use .

- **Clinical notes are essential for accurate matching.** Structured EHR data alone misses eligible patients and includes ineligible ones. Stage, performance status, biomarkers, and prior therapies are often documented only in prose . Hybrid approaches combining OMOP SQL for structured fields with NLP/LLM extraction from notes are required for comprehensive screening .

- **Human review remains essential.** Even the best systems flag criteria requiring manual assessment (willingness, consent, ability to attend visits) . Final eligibility decisions rest with the study team and treating clinician—no automated system replaces clinical judgment.

- Self-hosted open-source solutions require proper security hardening, IRB approval, and ongoing validation. Model performance degrades with distribution shift—retraining and recalibration on local data are necessary for production deployment.



---



**Made for clinical research coordinators, site investigators, trial sponsors, and developers building transparent recruitment solutions.**  

Let's make Clinical Trial Patient Recruitment more open, data-driven, and equitable.
