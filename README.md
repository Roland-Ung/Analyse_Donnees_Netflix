# Analyse_Donnees_Netflix

## 🎯 Objectifs
L'objectif principal de ce projet est de mener une analyse de données de bout en bout pour extraire des insights concrets sur la stratégie de Netflix. Plus spécifiquement, les objectifs techniques étaient :
- **Nettoyage de données** : Traiter les valeurs manquantes et corriger les types de données (conversion des chaînes de caractères en variables numériques pour les durées).
- **Manipulation avancée avec Pandas** : Maîtriser le découpage des chaînes complexes (séparation et explosion des pays coproducteurs avec `split` et `explode`) et l'agrégation de données (`groupby`, `crosstab`, `agg`).
- **Visualisation de données** : Concevoir des graphiques clairs et pertinents avec Matplotlib et Seaborn, notamment la création de graphiques complexes à double axe Y (`twinx()`).
- **Interprétation analytique** : Traduire des courbes et des tableaux de données brutes en conclusions logiques sur les choix de production de la plateforme.

## 🛠️ Technologies utilisées
- Python
- Bibliothèques : Pandas, Numpy, Matplotlib, Seaborn

## 📖 Plan du Notebook Jupyter
### 1 - Importation des bibliothèques
### 2 - Importation et Nettoyage des données
### 3 - Compréhension globale du fichier
### 4 - Analyse des données

## 📈 Dataset
Les variables utilisés pour l'analyse des données sont :
- `type` : Films ou Séries
- `country` : Dans quel(s) pays cela a été tourné
- `release_year` : A partir de quelle année le film ou la série a été diffusée
- `duration` : durée d'un film (en minutes) ou nombre de saisons d'une série

## 🌍 Principales analyses réalisés
Le projet inclut plusieurs analyses exploratoires :
- Nombre de films et séries
- Evolution du nombre de films et séries au fil du temps
- Top 5 des pays avec le plus grand nombre de films et de séries
- Durée moyenne des films par pays
- Durée total de tous les films produits par pays
- Nombre moyen de saisons des séries par pays
- Nombre total de saisons de toutes les séries produites par pays
- Evolution de la durée moyenne des films et du nombre moyens de saisons des séries

## 📊 Insight Clés
- Les films représentent la grande majorité du catalogue global (presque les 3 quarts) face aux séries (environ 30%).
- On observe une baisse régulière de la durée moyenne des films, passant de 111 minutes en 2000 à 80 minutes en 2021.
- Pour les séries, après une forte instabilité au début des années 2000, le nombre moyen de saisons s'est complètement stabilisé (autour de 1,5 saisons)
- Les États-Unis dominent totalement le reste du monde sur la production de films et séries, suivis par l'Inde qui est deuxième, mais uniquement sur les films.
- Le Japon et la Corée du Sud se distinguent par un profil inversé : ils produisent plus de séries (Animes et K-Dramas) que de films.
- Le volume de films et de séries a augmenté de manière exponentielle entre 2014 et 2018, avant de connaître une chute brutale autour de 2020
- En 2020, alors que la production de films s'effondre déjà, les séries continuent d'augmenter et finissent par dépasser les films pour la première fois

## 📁 Structure du projet
```
Analyse_Donnees_Netflix/
│
├── Graphiques/
│   ├── EvolutionDureeMoy-NbrMoySaison.png      Evolution de la durée moyenne des films et du nombre moyens de saisons des séries
│   ├── EvolutionsNbrFilmsSeries.png            Evolution du nombre de films et séries au fil du temps
│   ├── NbrFilmsSeries.png                      Repartition des productions par type de contenu
│   ├── Top5Pays.png                            Top 5 des pays avec le plus grand nombre de films et de séries
├── analyse_NetflixData.ipynb                   Notebook Jupyter
└── README.md
```
