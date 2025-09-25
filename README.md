<h1 align="center">🔬 AttriLens-Mol: Attribute Guided Reinforcement Learning for Molecular Property Prediction with Large Language Models</h1>

<p align="center">
  <strong>Official GitHub Repository for the AttriLens-Mol</strong><br>
</p>

---
## 🧠 Overview
This repository introduces **AttriLens-Mol**, an **attribute-guided reinforcement learning framework** for molecular property prediction with large language models.  

<p align="center">
  <img src="https://github.com/user-attachments/assets/00a47fd6-17f9-4f97-a06f-4f37609ded69" width="100%" />
</p>

---

## 📦 What’s Included  

├── Dataset/               # Datasets for both AttriLens-Mol and Random Forest experiments
│   ├── AttriLens-Mol/     # Training and test sets for AttriLens-Mol
│   └── Random_Forest/     # Train/validation/test splits for Random Forest baselines
│
├── training/              # Training scripts and utilities
│   ├── AttriLens-Mol/     # Training scripts for AttriLens-Mol
│   └── Random_Forest/     # Training scripts for Random Forest baselines
│
├── requirements.txt       # Dependency list for environment setup
└── README.md              # Project documentation

---
## 🛠️ Installation

Clone this repository and install dependencies:

```bash
git clone https://github.com/szu-tera/AttriLens-Mol.git
cd AttriLens-Mol
pip install -r requirements.txt
```

## 🚀 Usage

### 🔧 1. Pretrain AttriLens-Mol
```bash
python AttriLens_train.py # Before running the script, edit line 611 and 639 in the file:
                           # json_file_path = ""
                           # output_dir=""
                           # and set it to your data file path and ckpt output file.
```

### 🌲 2. Random Forest Building
cd Random Forest
```bash
python Random Forest_{task}.py # Before running the script, edit line 13-15 in the file:
                               # train_df = pd.read_csv('')
                               # valid_df = pd.read_csv('')
                               # test_df = pd.read_csv('')
```


