PERSONNAL PROJECT. 
By personnal interest for the epidemic situation and to learn!
Attempt to predict covid-19 diagnostic on the basis of the patient's clinical data. Classification task.  

// LOTS TO IMPROVE. BEGINNER'S WORK//
###########################################################################

HOW TO USE THIS?
- download the dataset https://www.kaggle.com/einsteindata4u/covid19
- launch the EDA and modeles files in a Jupyter environnement

##############################################################################

EDA file :  
- localisation of NaNs and cleaning of empty columns (more than 90% of missing data)
- relationship age/target
- relationship blood data/target. Data distribution of quantitative features regarding to their class (positive or negative)
- relationship viral tests/target. confusion matrix over qualitatives features.
- blood data features' correlation

Modeles file: every decision is taken with a unique numerical indicator
- qualitative features encoding
- imputation of missing values attempts
- feature engineering attempts
- f1 score-based performance function, that also gives learning curves
- numerous modeles comparison (logistic regression, naïve bayes, trees, forests, adaboost, SVM, KNN, xgboost)
- pipelines : kbest features, PCA, polynomial expansion to adress overfitting or underfitting depending on the modele
- hyperparameters optimization by gridsearch (or best : randomizedsearch)
- precision/recall curves to find the best threshold 
- good global result : f1 > 0.6 et recall > 0.75
