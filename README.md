# Projet Détection de Fraude avec XGBoost

Ce projet a pour objectif de détecter les transactions frauduleuses à partir d’un jeu de données fortement déséquilibré, en comparant deux modèles de machine learning : **RandomForest** et **XGBoost**. Une API Flask sera développée pour déployer le modèle et permettre des prédictions en temps réel.

# Métriques et performances

Étant donné le fort déséquilibre des classes (fraudes très rares), les métriques principales utilisées pour évaluer les modèles sont :

    Précision (Precision) : proportion des prédictions positives correctes.

    Rappel (Recall) : proportion des vrais positifs détectés.

    F1-score : moyenne harmonique de la précision et du rappel, permettant un compromis entre les deux.

    Accuracy : taux de bonnes prédictions global, peu fiable en cas de fort déséquilibre.

Les modèles obtiennent un très bon rappel (~97-98%) pour la classe fraude, ce qui garantit que la majorité des fraudes sont détectées. Cependant, la précision reste faible (~6%), traduisant un grand nombre de fausses alertes. Le F1-score est donc limité (~0.11), ce qui montre la nécessité d’optimiser le compromis entre ces métriques.

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
