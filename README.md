# 🦙 Fine-Tuning Llama 2 for Financial Sentiment Analysis

This repository demonstrates how to fine-tune the Llama 2 7B model for **sentiment analysis of financial and economic news headlines**. The goal is to accurately classify news headlines as **positive**, **neutral**, or **negative** from an investor's perspective
## 📈 Why Financial Sentiment Analysis?

Sentiment analysis in finance provides key insights for:
- **Market insights** – Tracking investor confidence and consumer sentiment.
- **Risk management** – Detecting reputational threats early.
- **Investment decisions** – Informing stakeholders based on media sentiment trends.

---

## 📂 Dataset: FinancialPhraseBank

- Human-annotated by 16 financial experts.
- ~5,000 sentences labeled as `positive`, `neutral`, or `negative`.
- Original source: Malo et al., *Journal of the Association for Information Science and Technology (2014)*.

---

## 🛠️ Installation

### Python Environment Requirements
- Python ≥ 3.10
- CUDA-enabled GPU (recommended: NVIDIA Tesla P100 or better)

### Key Dependencies

```bash
pip install torch==2.1.2 tensorboard
pip install transformers==4.36.2 datasets==2.16.1 accelerate==0.26.1 bitsandbytes==0.42.0
pip install git+https://github.com/huggingface/trl@a3c5b71
pip install git+https://github.com/huggingface/peft@4a15595
