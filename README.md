# Pipelines de machine learning reproductibles avec tidymodels

Application de l'écosystème tidymodels à la détection de spams : 4 stratégies de prétraitement (données brutes, normalisation, ACP, Yeo-Johnson avec termes quadratiques) croisées avec 4 modèles (Random Forest, KNN, XGBoost, perceptron multicouche) dans un `workflow_set`, soit 16 pipelines dont les hyperparamètres sont optimisés par cross-validation.

Le meilleur pipeline (XGBoost sur données brutes) obtient une AUC de 0,985 en validation croisée et de 0,984 sur l'échantillon test.

## Fichiers

- `projet_app.Rmd` : code complet
- `data/spam.txt` : données

## Packages

```r
install.packages(c("tidymodels", "randomForest", "xgboost", "kknn", "nnet", "doParallel", "vip"))
```
