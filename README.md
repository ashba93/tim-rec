# TIM Rec: Sparse Feedback on Multi-Item Upselling Recommendations in an Industrial Dataset of Telco Calls


 **[SIGIR 2025] TIM Rec: Sparse Feedback on Multi-Item Upselling Recommendations in an Industrial Dataset of Telco Calls**

## Overview
This repository provides the dataset and benchmark results for our paper, which introduces a real-world **telecommunications upselling dataset** with **multi-item recommendations and sparse feedback**. The dataset captures customer interactions from a real customer care service, where multiple items can be recommended in a single session, and only a small fraction of offers are accepted. Our goal is to provide a resource for evaluating **Learning-to-Rank (LTR)** models and recommendation systems in real-world settings.

## Key Features
- **Real-World Telco Data**: Collected from customer care interactions in a live telecommunications setting.
- **Multi-Item Recommendations**: Each session contains multiple recommendations, reflecting real-world upselling scenarios.
- **Sparse Feedback**: A low acceptance rate, emphasizing the challenge of learning from limited positive signals.
- **Benchmark Baselines**: We provide results from various recommendation models, ranging from classical approaches to deep learning-based solutions.
- **Rich Feature Set**: Includes user contextual features, recommendation metadata, and interaction timestamps.

## Dataset Statistics
| Characteristic | Value |
|--------------|------|
| Total interactions | 1494061 |
| Time range | ∼6 months |
| Acceptance sparsity (%) | ∼5% |
| Avg. recommendations per session | ∼2.4 |

_For more details on the dataset schema and preprocessing, refer to the documentation._

## Benchmark Models
We evaluate several Learning-to-Rank and recommendation models, including:
- **Traditional Models**: Matrix Factorization Algorithm
- **Neural Models**: Neural Network based approaches
- **Graph-Based Models**: GNN-based recommendation approaches

Results and evaluation metrics such as **Precision@K, NDCG@K, and Recall@K** are included in the paper.

## Repository Structure
```
├── data/                  # Dataset files (to be released)
├── benchmarks/            # Code for baseline models
├── results/               # Evaluation results and metrics
├── src/                   # Scripts for preprocessing and training
├── docs/                  # Additional documentation
└── README.md              # This file
```

## Getting Started
1. Clone the repository:
   ```bash
   git clone https://github.com/ashba93/tim-rec.git
   cd tim-rec
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run preprocessing scripts:
   ```bash
   python src/preprocess.py
   ```
4. Train benchmark models:
   ```bash
   python src/train.py --model LTR_Model
   ```

## Citation
If you use this dataset or benchmark results in your research, please cite our paper:
```bibtex
@article{YourPaper,
  author    = {Alessandro Sbandi, Federico Siciliano, and Fabrizio Silvestri},
  title     = {TIM Rec: Sparse Feedback on Multi-Item Upselling Recommendations in an Industrial Dataset of Telco Calls},
  journal   = {48th International ACM SIGIR Conference on Research and Development in Information Retrieval (SIGIR ’25), July 13-18, 2025, Padua, Italy},
  year      = {2025},
  url       = {DOI or Link}
}
```

## Contact
For questions or collaborations, please open an issue or contact us at **alessandro.sbandi@gmail.com**.
