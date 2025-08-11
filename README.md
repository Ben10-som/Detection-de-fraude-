# Projet Détection de Fraude avec XGBoost

Ce projet a pour objectif de détecter les transactions frauduleuses à partir d’un jeu de données déséquilibré, en utilisant un modèle de machine learning XGBoost. Une API Flask est développée pour déployer le modèle et permettre des prédictions en temps réel.

---

## Contenu du projet

- `app.py` : application Flask pour servir le modèle et faire des prédictions via une API REST.  
- `xgb_model.json` : modèle XGBoost sauvegardé au format recommandé.  
- `script/` : scripts d’entraînement, de prétraitement et d’évaluation du modèle.  
- `requirements.txt` : liste des dépendances Python nécessaires.  

---

## Installation

1. Cloner le dépôt :  
```bash
git clone https://github.com/ton-utilisateur/ton-repo.git
cd ton-repo
