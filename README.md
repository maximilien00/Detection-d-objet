# Detection-d-objet

**But du programme : La détection d'objets avec Python et le module OpenCV**

**Language de Programmation : Python**

Le code suivant fonctionne sur un ordinateur (tournant sous Windows) ou sur un Raspberry pi Modèle B+ avec Rasbian comme OS, le reste je n'ai pas essayé.
Vous trouverez la liste des objets détectés par le programme dans la partie [Index](https://github.com/maximilien00/Detection-d-objet/blob/main/README.md#index- "Index").

# Instructions : 

1. Ecrire les commandes suivantes dans l'Invite de commande (avec les droit administarteurs de préférences) :

```shell
pip install opencv-python
pip install numpy
pip install imutils 
```

2. Télécharger le projet dans son intégralité et dézipper le

3. Ouvrer le dans l'IDE de votre choix :

- Si vous l'ouvrer dans l'IDE de base fourni par python, cliquer dans le menu sur **Run** puis sur **Run... Customized (Shift+F5)** 

  Une fenêtre souvre puis une autre plus petite, la seconde porte le titre **Customize** suivi du nom de votre fichier.
  Dans cette fenêtre vous devez écrire la commande suivante : 

  ```
  --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
  ``` 

  Appuyer sur le bouton **OK** ou sur la touche **Entrée** 

  Vous venez de finir de lancer le programme ! 
  
  Dans le Shell vous devrier avoir se premier message : **...chargement du modèle...**
  
  Puis un deuxième qui arrive  **...démarrage de la camera...**

  Une fois ceci vue, il suffit de mettre devant la caméra un objet figurant parmi la liste d'objets indiqué en Index.
  
  Pour **arreter le programme** il suffit de faire **Ctrl + c** ou d'appuyer sur la lettre **q** de votre clavier.
  
- Si vous utilisé PyCharm:

  Cliquer sur le bouton **Terminal** qui se situe en bas à gauche de votre écran, puis entrer la commande suivante :
  
  ```
  python reconnaissance_objets.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
  ```
  Pour **arreter le programme** il suffit de faire **Ctrl + c**.
  
- Si vous utilisé l'Invite de Commande ou le PowerShell:

  Aller dans le répertoire où se trouve le dossier que vous venez de dezipper avec la ligne de commande suivante (qu'il faut adapter à votre situation):
  
   ```
  cd C:\Users\NomUtilisateur\Dossier
  ```

  Entrer la commande suivante :
  ```
  python reconnaissance_objets.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
  ```
  
  Pour Arreter le programme il suffit de faire **Ctrl + c**
  
# Index :

Liste des objets détéctés : 
 - avion
 - velo
 - oiseau
 - bateau
 - bouteille
 - autobus
 - voiture
 - chat
 - chaise
 - vache
 - table
 - chien
 - cheval
 - moto
 - personne
 - plante en pot
 - mouton
 - sofa
 - train
 - moniteur

# Remarque :

Le code vient du Site : www.framboise314.fr

Voici le lien exacte dédier à un raspberry pi : https://www.framboise314.fr/i-a-realisez-un-systeme-de-reconnaissance-dobjets-avec-raspberry-pi/#Le_programme_Python
