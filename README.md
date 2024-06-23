# Objectif de l'application

L'objectif de cette application est de réaliser une régression linéaire simple à partir d'un fichier CSV fourni par l'utilisateur. La régression linéaire simple permet de prédire une variable dépendante (à prédire) en fonction d'une variable indépendante (servant à la prédiction). L'application est conçue avec Streamlit, une bibliothèque Python permettant de créer des interfaces web interactives pour l'apprentissage automatique et les analyses de données.

## Fonctionnement de l'application

### Chargement du fichier CSV:

1. L'utilisateur commence par uploader un fichier CSV contenant les données.
2. L'application lit le fichier CSV pour afficher un aperçu des données et permettre la sélection des colonnes pertinentes.

### Sélection des colonnes:

1. L'utilisateur sélectionne la colonne contenant la variable indépendante (variable X), qui est la valeur utilisée pour faire la prédiction.
2. L'utilisateur sélectionne également la colonne contenant la variable dépendante (variable y), qui est la valeur que le modèle essaiera de prédire.

### Préparation des données:

1. Les données des colonnes sélectionnées sont extraites du dataframe et converties en tableaux numpy.
2. Les données sont ensuite divisées en ensembles d'entraînement (80%) et de test (20%) pour entraîner et évaluer le modèle.

### Entraînement du modèle:

1. Un modèle de régression linéaire est créé à l'aide de la bibliothèque Scikit-learn.
2. Le modèle est entraîné sur les ensembles d'entraînement pour apprendre la relation entre les variables X et y.

### Prédiction:

1. L'utilisateur entre une nouvelle valeur pour la variable X.
2. Le modèle utilise cette valeur pour prédire la valeur correspondante de la variable y.
3. L'application affiche la prédiction arrondie à deux décimales.

Lien vers l'application streamlit : https://linearregression-mf6tze6fyztuyvaf9envxn.streamlit.app/