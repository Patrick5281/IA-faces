# Module de Reconnaissance Faciale avec OpenCV et TensorFlow

Ce projet a été réalisé par **Patrick HOUNTON** et utilise **OpenCV** et **TensorFlow** pour implémenter un module de reconnaissance faciale capable d'identifier et de vérifier des visages en temps réel. Ce projet est idéal pour les développeurs travaillant dans le domaine de l'intelligence artificielle et de la vision par ordinateur.

## Prérequis

- Python 3.10 ou version supérieure
- Anaconda
- OpenCV
- TensorFlow

## Installation d'Anaconda

### Guide d'installation Anaconda

1. Aller sur la [page d'installation d'Anaconda](https://www.anaconda.com/products/distribution) et choisir l'installateur correspondant à votre système d'exploitation (Windows, Mac ou Linux). Sélectionner **Python 3.10** ou une version supérieure.
   
2. Suivre les instructions d'installation (très similaire à l'installation de tout autre logiciel).
   
3. Une fois installé, ouvrir le logiciel **Anaconda Navigator** via une recherche sur votre machine.

## Mise en place de l'environnement pour la reconnaissance faciale

1. Télécharger le fichier `formation-IA.yml` (fourni avec ce projet).
2. Ouvrir **Anaconda Navigator**, aller dans l'onglet **Environments**, puis sélectionner **Import**.
3. Sélectionner le fichier `formation-IA.yml`, importer l'environnement et l'activer.
4. Ouvrir **Spyder** depuis l'environnement `formation-IA`.

## Tester l'installation d'OpenCV et TensorFlow

### Test OpenCV et TensorFlow

Ouvrir **Spyder** et exécuter le code suivant pour vérifier que OpenCV et TensorFlow sont correctement installés :

```python
import cv2
print(cv2.__version__)

import tensorflow.compat.v1 as tf
tf.disable_v2_behavior()

hello = tf.constant('Hello, TensorFlow!')
with tf.Session() as sess:
    print(sess.run(hello))