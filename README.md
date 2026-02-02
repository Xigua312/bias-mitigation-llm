# Bias Mitigation for Large Language Models

This repository contains code, experiments, and evaluation notebooks for bias mitigation in large language models (LLMs).
The project focuses on analyzing social bias, applying debiasing techniques, and evaluating their effectiveness across different models.

---
**ICML 2026 paper**.
The project focuses on analyzing social bias, applying debiasing techniques, and evaluating their effectiveness across different models.
## 📁 Repository Overview

The repository is mainly organized around Jupyter notebooks for different models, debiasing methods, and evaluation pipelines.

```
bias-mitigation-llm/
├── CDA Model.ipynb
├── Dataset Winobias.ipynb
├── Original Model.ipynb
├── UGID Model.ipynb
├── KLAAD Model.ipynb
├── Evaluation/
├── Figure/
└── README.md
```

---

## 📄 File and Folder Description

- **CDA Model*.ipynb**  
  Implementation of Counterfactual Data Augmentation (CDA) for bias mitigation on different LLMs.

- **Original Model*.ipynb**  
  Baseline models without debiasing, used for comparison.

- **UGID Model*.ipynb**  
  Implementation of Unsupervised Gender-Informed Debiasing (UGID).

- **KLAAD Model*.ipynb**  
  KL-based adaptive debiasing method.

- **Dataset Winobias.ipynb**  
  Notebook for loading and preprocessing the Winobias dataset.

- **Evaluation/**  
  Evaluation notebooks for bias metrics, result analysis, and method comparison.

- **Figure/**  
  Generated figures and visualizations from experiments.

---

## 🧠 Bias Mitigation Methods

This repository explores several bias mitigation strategies, including:

- **Counterfactual Data Augmentation (CDA)**  
  Reduces bias by augmenting training data with counterfactual samples.

- **Unsupervised Gender-Informed Debiasing (UGID)**  
  A debiasing approach that leverages latent gender information without explicit supervision.

- **KL-based Adaptive Debiasing (KLAAD)**  
  Uses KL divergence to adaptively control bias during training or inference.

Each method is implemented and evaluated in separate notebooks for clarity and reproducibility.

---

## 🚀 Getting Started

### Clone the Repository
```bash
git clone https://github.com/Xigua312/bias-mitigation-llm.git
cd bias-mitigation-llm
```

### Run Notebooks
```bash
jupyter notebook
```
or
```bash
jupyter lab
```

Open any notebook of interest (e.g. `CDA Model-Qwen2.5-14B.ipynb`).

---

## 📊 Evaluation

Evaluation notebooks include:
- Bias metrics on benchmark datasets (e.g. Winobias)
- Comparison between original and debiased models
- Visualization of bias reduction results

Please refer to the `Evaluation/` directory for detailed experiments and results.

---

## 🔐 Environment Variables

Sensitive tokens (e.g., Hugging Face access tokens) must not be hard-coded.

```bash
export HF_TOKEN="your_huggingface_token"
```

```python
import os
token = os.getenv("HF_TOKEN")
```

---

## 📝 Notes

- This is a research-oriented, notebook-based repository.
- Results may vary depending on model size, dataset version, and hardware.
- Large models may require GPU resources.

---

## 🤝 Contributions

Contributions are welcome.
Please open an issue or submit a pull request if you have suggestions or improvements.

---

## 📜 License

Please specify the license for this project (e.g., MIT License).

---

## 🙏 Acknowledgements

This project builds upon open-source large language models, datasets, and prior research on fairness and bias mitigation.
