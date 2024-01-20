# Classification-dimages-de-legumes-et-de-fruits
Le code Python réalise une classification d'images de légumes et de fruits à l'aide de TensorFlow


Imports :

tensorflow : pour la création, l'entraînement et l'évaluation du modèle de machine learning.
matplotlib.pyplot : pour visualiser les images.
numpy : pour effectuer des opérations mathématiques efficaces sur les tableaux.
Chargement du Dataset :

Les données sont chargées à partir de répertoires distincts pour les ensembles d'entraînement, de validation et de test en utilisant image_dataset_from_directory de TensorFlow.
Les images sont redimensionnées à une taille spécifiée (img_height et img_width).
Les classes de fruits et de légumes sont définies dans class_names.
Visualisation du Dataset :

Quelques exemples d'images du jeu de données d'entraînement sont affichés pour visualiser les données.
Construction du Modèle CNN :

Un modèle séquentiel est créé avec plusieurs couches, notamment des couches de convolution (Conv2D), des couches de pooling (MaxPooling2D), une couche d'aplatissement (Flatten), et des couches denses (Dense).
Le modèle est compilé avec l'optimiseur "adam" et la perte SparseCategoricalCrossentropy pour la classification.
Entraînement du Modèle :

Le modèle est entraîné sur les données d'entraînement (train_ds) avec une validation sur les données de validation (val_ds) pendant 10 époques.
Évaluation du Modèle sur l'ensemble de test :

Le modèle est évalué sur l'ensemble de test (test_ds).
Visualisation des Résultats sur l'ensemble de test :

Conversion du Modèle en TensorFlow Lite (TFLite) :

![image](https://github.com/Makkaoui-Mohammed/Classification-dimages-de-legumes-et-de-fruits/assets/108239380/33afd6d8-afc8-48ab-b326-2a4468f1d919)
