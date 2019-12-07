# GiveMeCredit Kaggle - Jupyter notebook 

Participation au challenge Kaggle [Give Me Some Credit ](https://www.kaggle.com/)


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

    ![idprojectbigml](https://github.com/vlagache/GiveMeCredit/blob/master/img/idprojectbigml.JPG) 


__________________________________________________________________
### Table des matières


*  [Ensemble avec BigML](https://github.com/vlagache/GiveMeCredit/blob/master/GiveMeCredit-Ensemble.ipynb)
> Création d'un dataset ( avec nouvelles features ) sur BIGML , création d'un modèle ensemble , prediction &   envoi à kaggle
*  [Ensemble Model Review - bigml](https://github.com/vlagache/GiveMeCredit/blob/master/GiveMeCredit-Ensemble-ModelReview.ipynb)
> Confusion matrix , Profits , Accuracy , AUC , ROC Curve , 100 + grosses erreurs
*  [fonctions](url)
> Modifications des features du dataset initial 

________________________
### Score Kaggle 
* Ensemble BigML : 0.00000 
* XBoost : 