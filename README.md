# covid19-project
Pour apprendre et pour le fun! (dataset kaggle)

Analyse de données cliniques (111 variables) d'un groupe de 5644 patients en vue de prévoir le diagnostic covid19. 

Le premier fichier est une analyse exploratoire pour guider la tactique à venir et le choix des modèles. 
-localisation des valeurs manquantes
-nettoyage des colonnes peu parlantes (plus de 90% de valeurs manquantes)
-observation de la répartition des classes positives et négatives
-lien target/ âge
-lien target/données sanguines: observation de la distribution des variables quantitatives selon la classe 
-lien target/tests viraux : matrices de confusion des variables qualitatives 
-observation de la corrélation des variables sanguines
-essai de feature engineering

Le deuxième est une méthodologie simple appliquée pour proposer un modèle final optimal. 
(prise de décision en évaluant le meilleur choix à chaque étape grâce à unique indicateur chiffré)
-encodage des variables qualitatives
-essais de feature engineering
-imputation sur les valeurs manquantes (médiane, moyenne, zéro, drop, etc...)
-implémentation d'une fonction d'évaluation de la performance (à base de score f1) qui donne aussi les courbes d'apprentissage.
-comparaison de nombreux modèles (régression logistique, naïve bayes, arbres, forêts, adaboost, SVM, voisins, xgboost)
-pipelines aves kbest features, pca, expansion polynomiale pour adresser l'overfitting ou l'underfitting selon le cas
-optimisation du meilleur modèle par un gridsearch
-mieux encore : optimisation par un randomizedsearch
-courbes precision/recall pour aider au meilleur choix de seuill selon les contraintes métier (f1 > 0.6 et recall > 0.75)
