# covid19-project
Pour apprendre et par intérêt pour ce sujet d'actualité. 

Il s'agit de prévoir le diagnostique covid19 de patients (5644 individus) sur la base de ses données cliniques (111 variables mixtes).
  (Dataset kaggle)

EDA:  
- localisation des valeurs manquantes et nettoyage des colonnes peu parlantes (plus de 90% de valeurs manquantes)
- lien target/ âge
- lien target/données sanguines: observation de la distribution des variables quantitatives selon la classe 
- lien target/tests viraux : matrices de confusion des variables qualitatives 
- observation de la corrélation des variables sanguines

Modèles (prise de décision en évaluant le meilleur choix à chaque étape grâce à unique indicateur chiffré): 
- encodage des variables qualitatives
- imputation sur les valeurs manquantes (médiane, moyenne, zéro, drop, etc...)
- essais de feature engineering
- implémentation d'une fonction d'évaluation de la performance (à base de score f1) qui donne aussi les courbes d'apprentissage.
- comparaison de nombreux modèles (régression logistique, naïve bayes, arbres, forêts, adaboost, SVM, voisins, xgboost)
- pipelines aves kbest features, pca, expansion polynomiale pour adresser l'overfitting ou l'underfitting selon le cas
- optimisation du meilleur modèle par un gridsearch et mieux encore : randomizedsearch
- courbes precision/recall pour aider au meilleur choix de seuill selon les contraintes métier 
- bonne réussite globale : f1 > 0.6 et recall > 0.75
