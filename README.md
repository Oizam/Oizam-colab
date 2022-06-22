<div align="center">

  ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
# MODELES DE MACHINE LEARNING

</div>

- [A. Classification d'images d'oiseaux Nord-américains](#ClassImgUS)

- [B. Classification d'images d'oiseaux Français](#ClassimgFR)

- [C. Data Augmentation](#DataAug)

- [D. Classification de chants d'oiseaux Nord-américains](#ClassSonUS)

- [E. Classification de chants d'oiseaux Français](#ClassSonFR)

- [F. Détection d'oiseaux Nord-américains dans une image](#DetectUS)

- [G. Détection d'oiseaux Français dans une image ](#DetectFR)

***

# A. CLASSIFICATION DES OISEAUX NORD-AMERICAINS <a id="ClassImgUS"></a>

## 1. Choix du dataset

<img align="right" src="/img/caltech.jpeg" width=450>

Dataset choisi : [**Caltech Birds 2011**](https://www.tensorflow.org/datasets/catalog/caltech_birds2011)
contenant 200 espèces et 11788 images avec leurs bounding boxes (pour un futur travail sur la détection).

Il peut s'implémenter directement depuis tensorflow_datasets.

Mais pour la data augmentation, nous pouvons aussi utiliser le jeu de données complet : [**Ici**](https://data.caltech.edu/records/20098)

Une data augmentation a été faite à l'aide d'un deuxième jeu de données [**Kaggle - 400 species**](https://www.kaggle.com/datasets/gpiosenka/100-bird-species), ainsi qu'une augmentation manuelle (explication dans la partie [Data Augmentation](#DataAug))

## 2. Modèle le plus performant (Xception)

Colab: [**Xception US**](https://colab.research.google.com/drive/10Eqvw4c016xSLJZQ6nnrrRPUHYOdba9O#scrollTo=4QZV8XJ2Yn_E)

En savoir plus sur le modèle [**Keras - Xception**](https://keras.io/api/applications/xception/)

## 3. Modèle plus léger déployable (MobileNetV3)

Colab: [**MobileNetV3Large US**]()

En savoir plus sur le modèle [**Keras - MobileNetV3Large**](https://keras.io/api/applications/mobilenet/#mobilenetv3large-function)

<br clear="right"/>

***

# B. CLASSIFICATION DES OISEAUX FRANCAIS <a id="ClassImgFR"></a>

## 1. Création du dataset

<img align="right" src="/img/oiseauxnet.png" width=450>

Ne trouvant pas de dataset d'oiseaux français, nous avons été crontraints de le faire nous-même, notamment à l'aide de photos prises sur [**Oiseaux.net**](https://www.oiseaux.net/) et y en ajoutant d'autres provenant de Google Images et d'autres sites.

## 2. Modèle le plus performant (Xception)

Colab: [**Xception FR**]()

## 3. Modèle plus léger déployable (MobileNetV3)

Colab: [**MobileNetV3 FR**]()

<br clear="right"/>

***

# C. DATA AUGMENTATION <a id="DataAug"></a>

## 1. Extension : Image Downloader

<img align="right" src="/img/LogoIMGDL.jpg" width=250>

Télécharger pour Chrome : [**Image Downloader**](https://chrome.google.com/webstore/detail/image-downloader/kdbfjpagopjjaiofmgodphiklmjhcnok?hl=fr)


## 2. Fonctions pour gestion de la data

- Déplacer des images d'un dataset vers un autre (avec noms de dossiers identiques)

- Convertir tous les formats d'images du dataset en .jpg

- Changer les noms des dossiers/classes d'un dataset (en y ajoutant un numéro/index)

- Renommer toutes les images des dossiers/classes d'un dataset en fonction de leur nom de dossier



<br clear="right"/>

***


