# Exploring the Dataset

Notebook Jupyter réalisé dans le cadre d'un lab (IBM Skills Network) portant sur l'exploration initiale d'un jeu de données.
Ce projet illustre les premières étapes essentielles de toute analyse de données : comprendre la structure, les types 
et les caractéristiques principales d'un dataset avant d'aller plus loin.

## 📋 Description

Ce lab utilise un jeu de données issu d'une enquête (survey) mondiale pour pratiquer les techniques de base de l'exploration
de données avec **pandas**. L'objectif est de se familiariser avec un dataset avant toute analyse approfondie :
dimensions, types de colonnes, valeurs manquantes, statistiques descriptives, etc.

## 🎯 Objectifs pédagogiques

À l'issue de ce lab, on est capable de :

- Résumer les caractéristiques clés d'un dataset
- Identifier les différents types de données couramment utilisés en analyse de données

## 🗂️ Jeu de données

Le dataset est chargé directement depuis une URL (fichier CSV hébergé sur IBM Cloud Object Storage) :

```
https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/VYPrOu0Vs3I0hKLLjiPGrA/survey-data-with-duplicate.csv
```

Il s'agit des résultats d'une enquête mondiale, incluant notamment des colonnes comme `Age` et `Country`.

## 🛠️ Technologies utilisées

- Python 3
- [pandas](https://pandas.pydata.org/)
- manipulation et analyse de données

## 📦 Installation

```bash
pip install pandas
```

## 🚀 Utilisation

1. Cloner ce dépôt
2. Ouvrir le notebook `ExploreDataSet_lab.ipynb` avec Jupyter Notebook, JupyterLab, ou VS Code
3. Exécuter les cellules dans l'ordre

## 📊 Contenu du notebook

Le notebook couvre les étapes suivantes :

1. **Chargement des données** — lecture du fichier CSV avec `pd.read_csv()`
2. **Aperçu du dataset** — affichage des 5 premières lignes avec `df.head()`
3. **Dimensions du dataset** — nombre de lignes et de colonnes avec `df.shape`
4. **Types de données** — identification des types de chaque colonne avec `df.dtypes`
5. **Statistiques sur l'âge** — conversion des tranches d'âge en valeurs numériques et calcul de l'âge moyen des participants
6. **Diversité géographique** — nombre de pays uniques représentés dans l'enquête (`df['Country'].nunique()`)

## 📄 Licence

Ce notebook est basé sur un lab éducatif © IBM Corporation, utilisé ici à des fins d'apprentissage personnel.
