# VulnLocAI

This repository is the replication package of "VulnLocAI: Lightweight Java Vulnerability Detection with Fine-Tuned Domain Specific Large Language Models"

## Overview

VulnLocAI is a specialized language model designed to detect vulnerabilities in Java code. Unlike traditional large language models (LLMs), VulnLocAI is specifically fine-tuned on a domain-specific dataset of Java vulnerabilities, making it more efficient and accurate for this specific task.

## Key Features

- **Domain-Specific Fine-Tuning**: Trained on 10,000 real-world vulnerable code snippets from 907 open-source Java projects
- **High-Precision Detection**: Achieves 96.39% precision, 99.58% recall, and 97.96% F1-score
- **CWE ID Prediction**: Identifies both Common Weakness Enumeration (CWE) IDs and exact line numbers of vulnerabilities
- **Outperforms State-of-the-Art**: Demonstrated superior performance compared to major LLMs including:
  - ChatGPT-4 (16.3% relative improvement)
  - Claude 3.5 Sonnet (20.5% relative improvement)
  - Gemini 2.0 Flash (23.5% relative improvement)
  - Llama 3.2 (1B) (42.9% improvement)
- **Lightweight Architecture**: Optimized for practical use in real-world development environments
- **Open-Source**: Fully transparent and extensible implementation

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Wala-Alnozmai/VulnLocAI.git
cd VulnLocAI
```

2. To reproduce the training process, run the Jupyter notebook:
```bash
jupyter notebook VulnLocAI.ipynb
```

The notebook contains all the necessary steps and dependencies required to reproduce the training process. Follow the instructions within the notebook to train your own instance of VulnLocAI.


## Citation

If you use this tool in your research, please cite:

```
@article{vulnlocai,
    title={VulnLocAI: A Java Vulnerability Detection Tool with Fine-Tuned Open-Source Small Language Models},
    author={Wala Alnozmai, Obieda Ananbeh, and Dae-Kyoo Kima},
    year={2025}
}
```


