**Prédiction de la Probabilité d’Automatisation des Métiers**

**Description du projet**



Ce projet a pour objectif de prédire la probabilité d’automatisation des métiers à partir de variables économiques, éducatives et professionnelles.



Il met en place un pipeline complet de data science comprenant :



* le nettoyage des données
* l’analyse exploratoire (EDA)
* l’ingénierie des variables
* la modélisation avec plusieurs algorithmes de machine Learning



**Objectifs**

* Prédire la variable cible : prob (probabilité d’automatisation)
* Analyser l’impact du salaire, de l’éducation et du secteur d’activité
* Nettoyer et préparer un dataset réel
* Comparer plusieurs modèles de machine learning
* Identifier les facteurs les plus influents



**Dataset**

Fichier utilisé : job-automation-probability.csv



**Variables principales :**

* occupation : métier
* education : niveau d’éducation
* median\_ann\_wage / average\_ann\_wage : salaire annuel
* numbemployed : nombre d’employés
* employed\_may2016 : données d’emploi
* prob : probabilité d’automatisation (variable cible)



**Prétraitement des données**

**Nettoyage effectué :**

* Normalisation des noms de colonnes
* Suppression des colonnes dupliquées
* Gestion des valeurs manquantes :

&#x20;              - variables numériques : médiane

&#x20;              - variables catégorielles : "Unknown"

* Suppression des valeurs aberrantes (Z-score > 3)
* Conversion des types de données



**Feature engineering :**

* Création de occupation\_clean
* Regroupement des métiers en catégories :

&#x20;     - technique

&#x20;     - management

&#x20;     - santé

&#x20;     - éducation

&#x20;     - vente, etc.

* Encodage des variables catégorielles (target encoding)
* Normalisation des variables numériques



**Analyse exploratoire des données (EDA)**

**Les analyses réalisées :**

* Distribution de la probabilité d’automatisation
* Relation entre salaire et probabilité
* Matrice de corrélation des variables numériques
* Impact du niveau d’éducation sur l’automatisation
* Top des métiers les plus et moins automatisables

**Insight principal :**

* Les métiers à faible salaire sont généralement plus exposés à l’automatisation
* Les métiers techniques et manuels présentent un risque plus élevé



**Modèles de machine learning**

**Plusieurs modèles ont été entraînés :**



**CatBoost Regressor**

* Gestion native des variables catégorielles
* Très performant sur données tabulaires

**Random Forest Regressor**

* Modèle robuste basé sur les arbres de décision
* Bonne performance de référence

**XGBoost Regressor**

* Modèle de boosting avancé
* Très performant sur données structurées



**Évaluation des modèles**

**Les modèles sont évalués avec :**

* RMSE (Root Mean Squared Error)
* R² Score

**Résultats**

* CatBoost donne de très bons résultats grâce aux variables catégorielles
* XGBoost offre une performance élevée
* Random Forest sert de baseline robuste
* Le feature engineering améliore significativement les performances



**Variables les plus importantes**

Les facteurs les plus influents sont :

* Niveau d’éducation
* Secteur d’activité
* Salaire annuel
* Nombre d’employés



**Technologies utilisées**

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* CatBoost
* Random Forest

















































































