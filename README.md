<h1 style="text-align: center; font-size: 35px;">Classification automatique de produits</h1>

## Description
Taille du fichier **CSV** : **1,7 Mo** <br>
Taille du dossier `data/images/` : **365,9 Mo**
Les données ainsi que les fichiers **csv** et les images créées au cours du projet se trouvent dans le dossier `data/`

## Procédure
- Exploration des données
- Etude de faisabilité NLP
    - Nettoyage des descriptions
    - Segmentation (Bag of Words, TF-IDF, Word2Vec, BERT, USE)
- Etude de faisabilite Computer Vision
    - Transformation des images
    - Segmentation (SIFT, VGG16)
- Classification
    - Data Augmentation
    - Segmentation à l'aide du modèle ImageNet
    - Application d'un RandomForestClassifier


## Dossiers & fichiers
- **graphics** &rarr; Dossier contenant les graphiques enregistrés au cours de l'analyse.
- **data** &rarr; Dossier contenant les données ainsi que les dataframes et images enregistrés et créés au cours du projet.
- **notebook_faisabilite.ipynb** &rarr; Notebook comportant l'analyse exploratoire des données ainsi que l'étude de faisabilité sur la classification via description (NLP) et images (Computer Vision)
- **notebook_classification.ipynb** &rarr; Notebook comportant une procédure de data augmentation pour la partie Computer Vision ainsi qu'une classification sur la sortie du modèle retenu.
- **presentation_slides.pdf** &rarr; Fichier pdf des slides de présentation de l'analyse exploratoire utilisées à lors de la soutenance du projet.
- **requirements.txt** &rarr; Fichier texte contenant la liste des bibliothèques utilisées

## Installation
Pour une utilisation en local :

```bash
git clone https://github.com/amaysounabe/ocr-p6.git
cd ocr-p6
pip install -r requirements.txt
```

**ATTENTION** : L'utilitaire de NVIDIA **CUDA** étant nécessaire au fonctionnement de certaines librairies de traitement d'images, il est possible que vous rencontriez des problèmes à l'utilisation en local.