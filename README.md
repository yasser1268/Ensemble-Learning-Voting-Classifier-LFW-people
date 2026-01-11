Ensemble Learning – Voting Classifier on LFW People
📌 Description du projet

Ce projet illustre l’utilisation de l’apprentissage en ensemble (Ensemble Learning) à travers un Voting Classifier appliqué au jeu de données Labeled Faces in the Wild (LFW People).
L’objectif est de comparer plusieurs modèles de classification, puis de les combiner afin d’améliorer les performances globales.

🎯 Objectifs

Charger et explorer le dataset LFW People

Appliquer un prétraitement adapté (normalisation, PCA)

Implémenter plusieurs classifieurs de base

Construire un Voting Classifier

Comparer les performances avec une baseline

Évaluer les modèles via validation croisée

Discuter des limites de l’approche

🗂️ Jeu de données

Nom : Labeled Faces in the Wild (LFW People)
Source : Scikit-learn
Chargement :

from sklearn.datasets import fetch_lfw_people


Images de visages de personnalités publiques

Données réelles, bruitées et déséquilibrées

Utilisation d’un sous-ensemble pour réduire le coût de calcul

📚 Référence officielle :
https://scikit-learn.org/stable/datasets/real_world.html#lfw-people-dataset

⚙️ Méthodologie
1. Exploration des données

Dimensions du dataset

Nombre de classes

Distribution des labels

2. Prétraitement

Mise à l’échelle avec StandardScaler

Réduction de dimension via PCA

Justification : données haute dimension + bruit

3. Modèles utilisés

Logistic Regression

Support Vector Machine (SVM)

Random Forest

4. Ensemble Learning

VotingClassifier (Soft Voting)

Pondération égale des modèles

5. Optimisation

GridSearchCV

Validation croisée (k = 5)

📊 Métriques d’évaluation

Accuracy

F1-score (macro)

Matrice de confusion

▶️ Instructions d’exécution
Exécution locale
pip install numpy pandas scikit-learn matplotlib seaborn
jupyter notebook


Puis ouvrir :

Untitled-1.ipynb

Exécution sur Google Colab

Importer le notebook

Exécuter toutes les cellules (Runtime > Run all)

Aucun fichier externe requis

⚠️ Limites du projet

Dataset déséquilibré

Perte d’information due au PCA

Temps de calcul élevé sans sous-échantillonnage

Sensibilité aux hyperparamètres

📚 Références

Pedregosa et al., Scikit-learn: Machine Learning in Python, JMLR, 2011

Scikit-learn documentation
https://scikit-learn.org

LFW Dataset
http://vis-www.cs.umass.edu/lfw/