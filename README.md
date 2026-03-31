<div align="center">

# VulnLocAI

### Lightweight Java Vulnerability Detection with Fine-Tuned Domain-Specific Large Language Models

[![Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/jupyter-notebook-orange.svg)](https://jupyter.org/)


</div>

---

## 📋 Overview

**VulnLocAI** is a lightweight, domain-specific large language model (DSLLM) designed to detect vulnerabilities in Java code with exceptional accuracy and efficiency. Built by fine-tuning Meta's Llama 3.2 (1B parameters), VulnLocAI addresses the critical limitations of general-purpose LLMs—high computational costs, privacy concerns, and lack of domain specialization—while delivering superior vulnerability detection performance.

## 📁 Repository Structure

```
VulnLocAI-Repo/
│
├── 📓 VulnLocAI.ipynb                    # Main training notebook
├── 📓 alpaca_format_dataset.ipynb        # convert the dataset into Alpaca-formatted
├── 📄 README.md                          
│
├── 📂 training dataset/
│   ├── dataset.csv.zip                   # Original training dataset (20,000 snippets)
│   └── alpaca_format_dataset.csv.zip     # Alpaca-formatted dataset
│
├── 📂 Evaluation-Benchmark/
│   ├── README.md                         
│   └── SVD-Benchmark.csv                 # Evaluation benchmark (5,054 snippets)
│
└── 📂 Results/
    ├── Analysis Result By CWE Types.csv  
    └── AnalysisByProjects.csv             
```

---

## 🔧 Installation

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook
### Quick Start

1️⃣ **Clone the repository:**
```bash
git clone https://github.com/Wala-Alnozmai/VulnLocAI.git
cd VulnLocAI
```

2️⃣ **Install dependencies** (automatically handled in notebooks)
```bash
pip install torch transformers datasets trl unsloth
```

3️⃣ **Launch Jupyter Notebook:**
```bash
jupyter notebook VulnLocAI.ipynb
```

4️⃣ **Follow the notebook instructions** to reproduce the training process or use the pre-trained model!

---

## 🎓 Citation

If you use VulnLocAI in your research, please cite:

```bibtex
@article{vulnlocai2025,
    title={VulnLocAI: Lightweight Java Vulnerability Detection with Fine-Tuned Domain Specific Large Language Models},
    author={Wala Alnozmai and Obieda Ananbeh and Dae-Kyoo Kim},
    journal={},
    year={2026},
    publisher={}
}
```

