# GiveMeCredit Kaggle - Jupyter notebook 

Participation au challenge Kaggle [Give Me Some Credit ](https://www.kaggle.com/c/GiveMeSomeCredit)


### Démarrer le projet 
________________________________________________________
1. 
     ```
        git clone git@github.com:vlagache/GiveMeCredit.git
     ```
2. Création d'un fichier auth.env dans le dossier docker
3. dans le auth.env : 
    ```
    BIGML_USERNAME=xxx
    BIGML_API_KEY=xxx
    KAGGLE_USERNAME=xxx
    KAGGLE_KEY=xxx
    ```
    - [Api Key BigML](https://bigml.com/account/apikey)

    - [kaggle.com](https://www.kaggle.com/) > Account > Create New API Token
4. dans GiveMeCredit\docker :
    ```
    docker-compose up --build
    ```
5. dans le notebook ( fichier Ensemble_bigml ) modifier la ligne suivante 
    ```
    api = BigML(project="votre project ID")
    ```
    l'id de votre projet se trouve à l'adresse suivante : [projects BigML](https://bigml.com/dashboard/projects/)

    ![idprojectbigml](https://github.com/vlagache/give_me_credit/blob/master/img/idprojectbigml.JPG) 


__________________________________________________________________
### Table des matières


*  [Ensemble avec BigML](https://github.com/vlagache/give_me_credit/blob/master/1-Ensemble_bigml.ipynb)
> Création d'un dataset ( avec nouvelles features ) sur BIGML , création d'un modèle ensemble , prediction &   envoi à kaggle
*  [Ensemble Model Review - bigml](https://github.com/vlagache/give_me_credit/blob/master/2-Ensemble_ModelReview_bigml.ipynb)
> Confusion matrix , Profits , Accuracy , AUC , ROC Curve , 100 + grosses erreurs
*  [fonctions](https://github.com/vlagache/give_me_credit/blob/master/fonctions.ipynb)
> Modifications des features du dataset initial 
* [Xgboost](https://github.com/vlagache/give_me_credit/blob/master/3-Xgboost.ipynb)
> Modele xgboost et prédictions 
* [new_input_prediction](https://github.com/vlagache/give_me_credit/blob/master/4-new_input_prediction.ipynb)
> Prédiction sur de nouvelles données clients avec le modele entrainé précédement (xgboost)

________________________
### Score Kaggle ( vlagache )
* XGBoost : Public Score 0.86004 ( ~ 204 sur 924 participants )
* BigML : Public Score 0.85938