Ce projet a pour objectif de développer un modèle de machine learning pour recommander le type de 
culture agricole le plus adapté à une parcelle de terre donnée, en se basant sur ses caractéristiques
 climatiques et pédologiques.
La base de données utilisée vient du  site Kaggle dont le lien est le suivant :
 https://www.kaggle.com/datasets/chitrakumari25/smart-agricultural-production-optimizing-engine



Fonctionnalités principales :

    Chargement des librairies pandas, numpy, matplotlib, seaborn et warnings.
    Chargement du jeu de données "data_agriculture.csv".
    Exploration des données :
        Recherche des valeurs nulles.
        Affichage de la moyenne de chaque élément par culture.
        Vérification des valeurs aberrantes à l'aide de diagrammes en boites à moustaches.
    Préparation des données :
        Séparation des caractéristiques (X) de la variable cible (y - label de la culture).
        Division des données en ensembles d'entraînement et de test.
        Normalisation des données avec un StandardScaler.
    Définition et entraînement des modèles de classification :
        Régression logistique
        Naive Bayes gaussienne
        SVM (Support Vector Machine)
        KNN (K plus proches voisins)
        Recherche des hyperparamètres optimaux pour chaque modèle avec GridSearchCV.
    Sélection du meilleur modèle en fonction du score de validation.
    Évaluation du modèle sélectionné :
        Calcul et affichage de la précision, du rappel et du F1-score.
        Génération de la matrice de confusion.
    Prédiction de la culture pour de nouvelles valeurs d'entrée.

Utilisation :

    Exécutez le script Python.
    Le script chargera automatiquement le dataset "data_agriculture.csv" et effectuera l'ensemble des analyses et classifications.
    La fonction evaluation affichera les performances du meilleur modèle sur l'ensemble de test.
    La fonction prediction permet de prédire la culture pour de nouvelles valeurs d'entrée.

Prérequis:

    Python 3.x
    librairies pandas, numpy, matplotlib, seaborn, scikit-learn

Note:

    Ce code suppose que le jeu de données "data_agriculture.csv" est présent dans le même répertoire que le script Python.
    Vous pouvez modifier le code pour charger un dataset différent en changeant le nom du fichier CSV dans 
la section "Chargement des données".