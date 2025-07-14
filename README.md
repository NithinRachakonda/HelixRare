# HelixRare: AI-Powered Patient-Trial Matching for Rare Diseases
HelixRare is an AI-driven system designed to match rare disease patients to clinical trials using zero-shot natural language inference. By combining patient genomic attributes with a BART-large MNLI model and prompt-based semantic reasoning, HelixRare ranks patient eligibility without task-specific training, outperforming existing baselines like TrialGPT.

## Key Features
- **Zero-shot inference** using BART-large MNLI
- **Prompt-based reasoning** for trial eligibility matching
- Integration of **genomic features and trial criteria**
- Outperforms baselines like TrialGPT in relevance ranking
- Tailored for **rare disease clinical trial recruitment**

## Repository Contents
- `model.ipynb`: Jupyter Notebook containing the full model pipeline, including data preprocessing, prompt generation, model inference, and scoring.
- `Data.rar`: Includes anonymized patient-trial data for testing and evaluation.
- `HelixRare_Memo.pdf`: A short write-up explaining the model, approach, and results.
- `HelixRare_Presentation.pdf`: Slide deck presented at Harvard HackRare 2025.
- `vrachakonda_MDC_Poster.pptx`: Research poster presented at Clark University’s Multidisciplinary Conference 2025.

## Methodology Overview
HelixRare uses a pre-trained `facebook/bart-large-mnli` model to infer the relevance between a patient profile (premise) and trial eligibility criteria (hypothesis) without explicit labels. The scores are then used to rank patients for each clinical trial, prioritizing best fits based on semantic alignment.

## Results
- Achieved higher accuracy and interpretability over existing models like TrialGPT.
- Enabled semantic trial filtering without requiring labeled training data.
- Demonstrated success on generalization datasets beyond training distribution.

## Applications
- Rare disease patient-trial matchmaking
- Precision medicine eligibility modeling
- Zero-shot clinical text inference pipelines

## Presentations
- Harvard HackRare 2025 – Demo for rare disease orgs and clinicians
- Clark University Multidisciplinary Conference 2025 – Poster session

> For research/demo use only. Not intended for clinical deployment without further validation.
