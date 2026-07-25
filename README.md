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

| **Caractéristique** | **Valeur** |
|---------------------|------------|
| **Nom** | PlantVillage |
| **Images** | 54 305 images |
| **Classes** | 38 classes de maladies |
| **Format** | JPG, RGB |

### Distribution des classes

![Distribution des classes](images/EDA.png)

---

## 🧠 Modèles utilisés

| **Tâche** | **Modèle** | **Performance** |
|-----------|------------|-----------------|
| Classification | EfficientNet B0-B3 | **97,8% accuracy** |
| Détection d'objets | YOLOv8n | **mAP50: 44,9%** |
| Segmentation sémantique | DeepLabV3+ | **IoU: 95,76%** |

---

## 📈 Résultats détaillés

### Matrice de confusion

![Matrice de confusion](images/Matrice%20de%20confusion.png)

### Métriques par classe

![Métriques](images/M%C3%A9trique.png)

### Graphiques d'analyse

![Graphiques](images/Graphique.png)

---

## 🏗️ Architecture du projet

![Schéma d'architecture](architecture.png)

Le système est composé de 3 modules principaux :

| **Module** | **Modèle** | **Performance** |
|------------|------------|-----------------|
| **Classification** | EfficientNet B0-B3 | **97,8% accuracy** |
| **Détection d'objets** | YOLOv8n | **mAP50: 44,9%** |
| **Segmentation** | DeepLabV3+ | **IoU: 95,76%** |

L'ensemble est déployé via une **API FastAPI** et un **dashboard Streamlit**.

---

## 📸 Dashboard Streamlit

### Page d'accueil

![Page d'accueil](images/Page%20d'accueil.png)

### Page de connexion

![Page de connexion](images/Page%20de%20connexion.png)

### Paramètres

![Paramètres](images/param%C3%A8tre.png)

### Capteurs IoT

![Capteurs](images/capteur.png)

### Statistiques globales du dataset

![Statistiques globales](images/%F0%9F%93%8B%20Statistiques%20globales%20du%20dataset.png)

---

## 🎥 Vidéo de démonstration

[▶️ Regarder la démonstration complète du projet (10:16)](https://drive.google.com/file/d/1D3X0OknKJvb_A9PUGH0aEeouIggXTfbv/view?usp=sharing)

---

## 🏗️ Structure du projet
