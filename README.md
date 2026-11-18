# Pipelines de machine learning reproductibles avec tidymodels

Projet réalisé dans le cadre du Master MSID (Université de Pau et des Pays de l'Adour).

Application de l'écosystème tidymodels à la détection de spams : 4 recettes de prétraitement (données brutes, normalisation, ACP, Yeo-Johnson avec termes quadratiques) croisées avec 4 modèles (Random Forest, KNN, XGBoost, perceptron multicouche) dans un `workflow_set`, soit 16 pipelines réglés par validation croisée à 10 blocs sur l'AUC.

Le meilleur pipeline (XGBoost sur données brutes) obtient une AUC de 0,985 en validation croisée et de 0,984 sur l'échantillon test.

## Fichiers

- `projet_app.Rmd` : code complet
- `data/spam.txt` : données

## Packages

```r
install.packages(c("tidymodels", "randomForest", "xgboost", "kknn", "nnet", "doParallel", "vip"))
```
