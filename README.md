TabM Heart Disease Prediction (Kaggle Playground S6E2)
**CV AUC: 0.9548** | **Top 1%** | **Beats CatBoost by +0.0013**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-orange.svg)](https://pytorch.org/)
[![Kaggle](https://img.shields.io/badge/Kaggle-Playground%20S6E2-yellow.svg)](https://www.kaggle.com/competitions/playground-series-s6e2)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

</div>

## 🎯 **Competition Results**
| Model | CV AUC | Public LB | vs CatBoost |
|-------|--------|-----------|-------------|
| **CatBoost Baseline** | 0.9535 | 0.9532 | - |
| **TabM Transformer** | **0.9548** | **0.9545** | **+0.0013** 🥇 |

## 🔥 **3 Key Innovations**

### 1. **Original UCI Dataset Statistics** ⭐
python
tabm-mini-normal | k=24 experts | 150 epochs | Categorical embeddings
Mean CV: 0.9548 ± 0.0003 | Best Fold: 0.9552 | Clipped predictions
train.csv (75k rows) 
↓
Original UCI Stats (+42 engineered features) 
↓ 
TabM Categorical Encoding 
↓ 
5-Fold CV Ensemble 
↓ 
submission_tabm.csv (0.9545 LB)
git clone https://github.com/shivan-codes/heart-disease-prediction
cd heart-disease-prediction
pip install -r requirements.txt
python main.py  # Auto-trains + generates submission
pytabkit (TabM) | PyTorch | pandas | scikit-learn | seaborn | matplotlib
✅ submission_tabm.csv      # 0.9545 LB - Submit this!
✅ oof_predictions.csv      # OOF validation (0.9548 AUC)
✅ tabm_grandmaster_dashboard.png  # 20" analysis
✅ skewed_features.png      # EDA visuals
pytabkit>=1.0.0
torch>=2.0.0
pandas>=2.0.0
numpy>=1.24.0
scikit-learn>=1.3.0
seaborn>=0.12.0
matplotlib>=3.7.0

