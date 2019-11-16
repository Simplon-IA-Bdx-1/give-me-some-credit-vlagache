# GiveMeCredit Kaggle - Jupyter notebook 

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
    docker-compose build 
    docker-compose up
    ```
5. dans le notebook ( fichier GiveMeCredit ) modifier la ligne suivante 
    ```
    api = BigML(project="votre project ID")
    ```
    l'id de votre projet se trouve à l'adresse suivante : [projects BigML](https://bigml.com/dashboard/projects/)

    ![idprojectbigml](https://github.com/vlagache/GiveMeCredit/blob/master/img/idprojectbigml.JPG) 


__________________________________________________________________
### Table des matières


*  [Ensemble](https://github.com/vlagache/GiveMeCredit/blob/master/GiveMeCredit-Ensemble.ipynb)
> Création d'un dataset ( avec nouvelles features ) sur BIGML , création d'un modèle ensemble ,  envoi à kaggle
*  [Ensemble Model Review](https://github.com/vlagache/GiveMeCredit/blob/master/GiveMeCredit-Ensemble-ModelReview.ipynb)
> Confusion matrix , Profits , Accuracy , AUC , ROC Curve , 100 + grosses erreurs
*  [Deepnet](https://github.com/vlagache/GiveMeCredit/blob/master/GiveMeCredit-Deepnet.ipynb)
> Création d'un dataset ( avec nouvelles features ) sur BIGML , création d'un modèle dataset ,  envoi à kaggle
* [Deepnet Model Review](https://github.com/vlagache/GiveMeCredit/blob/master/GiveMeCredit-Deepnet-ModelReview.ipynb)
>  Profits , AUC , ROC Curve
* [Ensemble AUC vs Deepnet AUC ](https://github.com/vlagache/GiveMeCredit/blob/master/GiveMeCredit-EnsemblevsDeepnet-AUC.ipynb)
> Affichage dans le meme repere AUC Ensemble - Deepnet
* [Learning Curve Ensemble - Deepnet ( val_set )](https://github.com/vlagache/GiveMeCredit/blob/master/Ensemble%20vs%20Deepnet%20Learning%20Curves(val_set).ipynb)
> Split du train_set et validation sur le validation_set pour Ensemble et Deepnet 
* [Learning Curve Ensemble - Deepnet ( train_set )](https://github.com/vlagache/GiveMeCredit/blob/master/Ensemble%20vs%20Deepnet%20Learning%20Curves(train_set).ipynb)
> Split du train_set et validation sur le train_set split pour Ensemble et Deepnet 
* [Learning Curve Ensemble Deepnet](https://github.com/vlagache/GiveMeCredit/blob/master/Learning%20Curves%20Ensemble%20%26%20Deepnet.ipynb)
> Affichage des courbes Ensemble validé sur train_set split & validation dans le meme repère  , pareil pour le deepnet


