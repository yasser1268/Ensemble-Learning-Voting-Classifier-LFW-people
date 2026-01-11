# Ensemble Learning – Voting Classifier on LFW People

Projet d'apprentissage automatique appliquant l'Ensemble Learning sur le dataset Labeled Faces in the Wild (LFW) pour la reconnaissance faciale.

## 👥 Auteurs

- El Yemni Yasser
- Ihab Bensselllak
- Malak Sabir
- Yassir Arif

## 📌 Description

Ce projet utilise un **Voting Classifier** combinant trois modèles (Logistic Regression, SVM, Random Forest) pour classifier des visages de personnalités publiques. Le dataset LFW contient 1288 images de 7 personnes différentes.

## 🎯 Objectifs

1. Charger et explorer le dataset LFW
2. Prétraiter les données (normalisation, PCA)
3. Implémenter un Voting Classifier
4. Optimiser les hyperparamètres avec GridSearchCV
5. Évaluer et comparer les performances

## ⚙️ Méthodologie

- **Prétraitement** : StandardScaler + PCA (150 composantes)
- **Modèles** : Logistic Regression, SVM (RBF), Random Forest
- **Ensemble** : Voting Classifier (Soft Voting)
- **Optimisation** : GridSearchCV avec validation croisée (k=5)
- **Split** : 70% train / 15% validation / 15% test

## 📊 Résultats

Le projet génère 9 visualisations :
- Échantillons du dataset
- Distribution des classes
- Analyse PCA et Eigenfaces
- Comparaison des modèles
- Matrice de confusion
- Analyse des erreurs

## 🛠️ Technologies

- Python 3.8+
- scikit-learn
- NumPy, Pandas
- Matplotlib, Seaborn

## 🚀 Installation

```bash
pip install numpy pandas scikit-learn matplotlib seaborn jupyter
jupyter notebook ML.ipynb
```

## ⚠️ Limites

- Dataset déséquilibré
- Perte d'information due au PCA
- Temps de calcul élevé (GridSearchCV)
- Sensibilité aux hyperparamètres

## 📚 Références

- [LFW Dataset](http://vis-www.cs.umass.edu/lfw/)
- [Scikit-learn Documentation](https://scikit-learn.org)
