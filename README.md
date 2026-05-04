# DimABSA_SemEval

This repository contains the code and experiments for our submission to the **SemEval Dimensional Aspect-Based Sentiment Analysis (DimABSA) Track A**.

We explore **Valence–Arousal (VA) prediction** using:
- In-Context Learning (ICL) with large language models
- Fine-tuned transformer-based models
- A hybrid ensemble of both approaches

---

## Repository Contents

This repository includes **6 model implementations**:

### In-Context Learning (ICL)
- `ICL-FS.ipynb` – Standard few-shot prompting
- `ICL-FS-CoT.ipynb` – Few-shot + chain-of-thought reasoning
- `ICL-FS-RDoC.ipynb` – Few-shot with RDoC-inspired affective signals

### Fine-Tuned Models (FT)
- `FT-RDoC-Setup.ipynb` – Feature engineering for RDoC-based signals used across fine-tuned models
- `FT-ST-RDoC.ipynb` – Single-task RoBERTa regression with RDoC features
- `FT-MT-RDoC.ipynb` – Multi-task RoBERTa model with auxiliary RDoC objective

### Ensemble Model
- `ICL-FT-Ensemble.ipynb` – Weighted ensemble of ICL-FS-RDoC and FT-MT-RDoC
