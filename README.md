# TIM Rec: Sparse Feedback on Multi-Item Upselling Recommendations in an Industrial Dataset of Telco Calls


 **[RECSYS 2025] TIM Rec: Sparse Feedback on Multi-Item Upselling Recommendations in an Industrial Dataset of Telco Calls**

 **Authors: Alessandro Sbandi, Federico Siciliano, Fabrizio Silvestri**
 
 **HugginFace**: https://huggingface.co/datasets/shba93/tim-rec

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

## Contact
For questions or collaborations, please open an issue or contact us at **alessandro.sbandi@gmail.com**.
