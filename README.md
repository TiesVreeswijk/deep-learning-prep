# Deep Learning prep

Personal preparation for the Deep Learning semester (starting February 2027). Over nine weeks, from 18 November 2026 to 20 January 2027, I train one small model of each type covered in the semester (ANN, CNN, NLP/LLMs and RL), so I start week 1 with hands-on experience and know which technique I want to go deeper into.

Each week has its own folder with a notebook and a short README that states the result in one line.

## Progress

| Week | Dates | Topic | Deliverable | Result |
|---|---|---|---|---|
| 0 | 18 to 22 Nov | [Setup](00_setup/) | Working environment | ✅ Environment ready |
| 1 | 23 to 29 Nov | [Python and basic ML](01_python_basic_ml/) | Clean-and-model notebook | Titanic: Random Forest 84.7%, Logistic Regression 84.4% (baseline 61.8%) |
| 2 | 30 Nov to 6 Dec | [Math essentials](02_math_gradient_descent/) | Gradient descent from scratch | |
| 3 | 7 to 13 Dec | [ANN](03_ann_mnist/) | MLP on MNIST | |
| 4 | 14 to 20 Dec | [CNN](04_cnn_cifar10/) | CNN on CIFAR-10 plus transfer learning | |
| Holiday | 21 Dec to 3 Jan | Transformers (optional) | [Idea list](notes/idea-list.md) | |
| 5 | 4 to 10 Jan | [NLP and LLMs](05_nlp_llms/) | Fine-tuned text classifier | |
| 6 | 11 to 17 Jan | [RL and reflection](06_rl_qlearning/) | Q-learning agent, [reflection](notes/reflection.md) | |
| 7 | 18 to 20 Jan | [Ready check](07_ready_check/) | Tidy repo, ticked ready check | |

Weekly hours, difficulties and lessons are kept in the [learning log](notes/learning-log.md).

## Repository layout

```
deep-learning-prep/
├── 00_setup/ … 07_ready_check/   one folder per week: notebook(s) + README with the result
├── notes/                        learning log, idea list, reflection
├── data/                         datasets (downloaded locally, not committed)
├── models/                       saved model weights (not committed)
├── requirements.txt              pip dependencies
└── environment.yml               the same environment for conda users
```

## Setup

Python 3.12 and PyTorch with CUDA (tested on an NVIDIA RTX 5060 Ti).

```powershell
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

Then open `00_setup/00_environment_check.ipynb` and run all cells. Without an NVIDIA GPU, install the CPU build of PyTorch instead (`pip install torch torchvision`) or use Google Colab or Kaggle for the GPU-heavy weeks (4 and 5).

Notebooks find the project root on their own, so they work whether Jupyter starts in the week folder or in the repository root. Datasets are downloaded into `data/` automatically the first time a notebook runs.

## Stack

PyTorch and torchvision for deep learning, Hugging Face `transformers` and `datasets` for NLP, Gymnasium and Stable-Baselines3 for RL, and NumPy, pandas, matplotlib and scikit-learn for data and baselines.
