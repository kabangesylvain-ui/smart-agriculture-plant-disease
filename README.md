# 🌱 Smart Agriculture - Détection des maladies des plantes

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0-red)](https://pytorch.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.95-green)](https://fastapi.tiangolo.com/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.22-FF4B4B)](https://streamlit.io/)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

---

## 📌 Contexte du projet

Les agriculteurs tunisiens subissent des pertes de rendement importantes dues aux maladies des plantes, mais la **détection manuelle est lente et coûteuse**.

**Objectif** : Concevoir un système de vision par ordinateur pour **détecter et segmenter automatiquement** les maladies foliaires.

---

## 📊 Dataset

- **Nom** : PlantVillage
- **Images** : 54 305 images
- **Classes** : 38 classes de maladies
- **Format** : JPG, RGB

---

## 🧠 Modèles utilisés

| **Tâche** | **Modèle** | **Performance** |
|-----------|------------|-----------------|
| Classification | EfficientNet B0-B3 | **97,8% accuracy** |
| Détection d'objets | YOLOv8n | **mAP50: 44,9%** |
| Segmentation sémantique | DeepLabV3+ | **IoU: 95,76%** |

---

## 🏗️ Structure du projet
smart-agriculture-plant-disease/
├── README.md # Documentation
├── requirements.txt # Dépendances Python
├── .gitignore # Fichiers ignorés
├── .env # Variables d'environnement
│
├── 📓 notebooks/
│ ├── EDA.ipynb # Analyse exploratoire
│ ├── Modèle.ipynb # Entraînement EfficientNet
│ ├── Segmentation.ipynb # Segmentation DeepLabV3+
│ ├── YOLOv8.ipynb # Détection YOLOv8
│ └── Évaluation.ipynb # Évaluation des modèles
│
├── 🐍 scripts/
│ ├── app.py # API FastAPI
│ ├── streamlit_app.py # Dashboard interactif
│ └── entraînement.py # Script d'entraînement
│
├── 📊 results/
│ ├── matrice_de_confusion.png
│ ├── courbes_d'entraînement.png
│ ├── yolo_visual_results_100epochs.png
│ └── ...
│
└── 📁 data/
├── diagnostic_feedback.db
└── base de données plantes_maladies.db


---

## 🚀 Déploiement

- **API** : FastAPI pour les prédictions en temps réel
- **Interface** : Dashboard Streamlit pour la visualisation
- **Stack** : PyTorch, YOLOv8, DeepLabV3+

---

## 📈 Résultats

| **Métrique** | **Valeur** |
|--------------|------------|
| Accuracy (classification) | **97,8%** |
| mAP50 (détection) | **44,9%** |
| IoU (segmentation) | **95,76%** |
| Dice Score (segmentation) | **0,9775** |

---

## 🎥 Vidéo de démonstration

[▶️ Regarder la démonstration complète du projet (10:16)](https://drive.google.com/file/d/1D3X0OknKJvb_A9PUGH0aEeouIggXTfbv/view?usp=sharing)

## 🏗️ Architecture du projet

![Schéma d'architecture](images/architecture.png)

Le système est composé de 3 modules principaux :
1. **Classification** : EfficientNet B0-B3 (97,8% accuracy)
2. **Détection** : YOLOv8n (mAP50: 44,9%)
3. **Segmentation** : DeepLabV3+ (IoU: 95,76%)

Le tout est déployé via une API FastAPI et un dashboard Streamlit.

## 🔧 Installation

```bash
# Cloner le dépôt
git clone https://github.com/kabangesylvain-ui/smart-agriculture-plant-disease.git
cd smart-agriculture-plant-disease

# Créer un environnement virtuel
python -m venv venv
source venv/bin/activate  # Sur Windows : venv\Scripts\activate

# Installer les dépendances
pip install -r requirements.txt


---

### Étape 2 : Valider les modifications

1. **En bas de la page**, vous verrez :
