# Projet d'entraînement d’un algorithme de classification de sentiments avec Pyspark

Ce projet d'analyse de données massives vise à exploiter des techniques avancées de traitement des données à grande échelle en utilisant Python avec la bibliothèque PySpark. L'objectif principal est de mettre en œuvre des méthodes d'analyse permettant de manipuler et d'extraire des informations significatives à partir de vastes ensembles de données massives. La distribution des calculs est utilisée pour optimiser le traitement de ces données, soulignant l'importance de l'efficacité dans la gestion de volumes importants d'informations.

   ## Le projet comprend les étapes suivantes :
- Lecture des données : Les données d'entraînement et de test sont lues à partir de fichiers JSON à l'aide de la bibliothèque PySpark. La session Spark est créée, et les données sont chargées dans des DataFrames.

- Prétraitement des données : Dans cette étape, les données sont préparées avant de les utiliser pour l'entraînement des modèles. Différentes méthodes d'extraction de caractéristiques sont utilisées, telles que HashingTF, TF-IDF et CountVectorizer, pour convertir les mots en vecteurs numériques. Les étiquettes de polarité sont également converties en valeurs numériques.

- Modélisation : Trois modèles de classification sont utilisés : la régression logistique, le Random Forest et le Naive Bayes. Le modèle de régression logistique a donné les meilleurs résultats, avec une précision de 73,46% sur les données de test. Une validation croisée est effectuée sur le modèle de régression logistique pour sélectionner les meilleurs paramètres.

- Autres méthodes d'extraction : Deux autres méthodes d'extraction de caractéristiques sont utilisées : TF-IDF et CountVectorizer. En utilisant CountVectorizer avec la régression logistique, le meilleur score obtenu est de 76,11%.

- Prédiction sur le fichier noclass.json : Le meilleur modèle, c'est-à-dire la régression logistique avec CountVectorizer, est utilisé pour faire des prédictions sur le fichier noclass.json. Les prédictions sont ensuite exportées dans un fichier JSON.

### Compétences
- Manipulation de données à grande échelle en Json
- Maîtrise de PySpark
- Méthodes d'Extraction de Caractéristiques 
- Modélisation avec des Algorithmes de Classification et optimisation des modèles
- Communication des Résultats 