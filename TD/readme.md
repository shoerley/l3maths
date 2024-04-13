scholet - mars 2024

# Environnement de travail


Vous avez deux méthodes préconnisées pour travailler :
1. Les machines de la salle TP
2. Google Colab

## 1. Usage des machines de TP
 
Il est recommandé d'utiliser les machines de la salle de TP, sous Windows. Les instructions ci-dessous s'appliquent à ces machines, où Python est déjà installé. Vous avez la possibilité d'utiliser votre machine personnelle, mais dans ce cas, vous êtes seul responsable de sa configuration.

### 1.1 Emplacement des codes sources

Vous devez créer un dossier `IntroIAL3_<nom>` sous le dossier `Documents`. Dans ce dossier, vous mettrez tous les éléments relatifs aux TD : codes sources, sujets, brouillons, etc. Vous y mettrez également l'éditeur Sublime Text.

Plus loin, le dossier `IntroIAL3_<nom>` sera appelé "dossier de travail". Prenez bien note du _chemin d'accès_ vers ce dossier. Quand on notera par exemple "dossier de travail/TD1/essai1.py", cela voudra désigner le fichier `essai1.py`, placé dans un sous-dossier nommé `TD1`, qui lui-même se trouve dans le dossier de travail `IntroIAL3_<nom>`.

### 1.2 Sublime Text

Vous pouvez utiliser le logiciel SublimeText pour éditer vos codes sources, c'est à dire pour programmer. 

- Téléchargez la **version portable** de Sublime text depuis le site internet officiel du logiciel. Décompressez l'archive dans votre dossier de travail.
- Un nouveau dossier nommé `sublime_text_build_4169_x64` (par exemple) vient d'être créé avec, à l'intérieur, le logiciel Sublime Text.
- Pour lancer l'éditeur, vous devrez lancer le fichier `sublime-text.exe` présent dans ce sous-dossier.

### 1.3 Installation de Python

Lors des séances de TD, vous avez besoin d'une installation Python fonctionnelle. Les machines de la salle disposent déjà de Python installé. 

Pour vous en assurer :
- Ouvrez l'invite de commande (Windows + R, puis "cmd"; ou bien tapez "Invite" dans la barre de recherche)
- Tapez python, puis validez
Si vous entrez dans l'environnement Python, c'est que Python est installé :
```
    Python 3.10.10 (tags/v3.10.10:aad5f6a, Feb  7 2023, 17:20:36) [MSC v.1929 64 bit (AMD64)] on win32
    Type "help", "copyright", "credits" or "license" for more information.
    >>>
```

### 1.4 Installation d'un package Python

Pour installer un package, vous devez suivre la procédure suivante :
- Ouvrez l'invite de commande (Windows + R, puis "cmd"; ou bien tapez "Invite" dans la barre de recherche)
- Pour installer le package "numpy" : 
````bash
pip install numpy --user
````
Si vous avez plusieurs packages à installer, saisissez leur nom l'un à la suite de l'autre, en terminant par `--user`.

Attention : ces commandes sont à saisir dans l'invite de commande, et non dans l'environnement Python !

### 1.5 Lancer un programme

Cette procédure vous servira de rappel pour savoir comment lancer un programme Python.

- Avec Sublime Text, créez un fichier "hello_world.py", que vous enregistrez sous "dossier de travail/hello_word/hello_world.py". Voici le contenu du fichier :
```bash
    for i in range(5):
      print("Me voici toute mignone je suis une nouvelle planete. Hello World !")
```

- Ouvrez l'invite de commande :
```bash
  C:\Users\shoerley>
```
Grâce à la commande `cd`, changez le dossier de l'invite de commande :
- Depuis l'invite de commande, changer le dossier pour pointer vers le dossier où se trouve votre fichier Python :
```bash
  C:\Users\shoerley>cd C:\Users\scholet\Documents\IntroIA_shoerley\hello_world
```
- Désormais, l'invite affiche : 
```bash
    C:\Users\shoerley\Documents\IntroIA_shoerley\hello_world>
```
- Pour lancer le programme `hello_world.py` :
```bash
    C:\Users\shoerley\Documents\IntroIA_shoerley\hello_world>python hello_world.py
```
Si cela ne fon[main.py](..%2F..%2Fautres%2Fmain.py)ctionne pas, essayez avec ``python3`` au lieu de `python`.

Retenez : l'invite de commande doit pointer vers le dossier où se trouve votre programme pour pouvoir le lancer :

## 2. Google Colab

Si vous avez une adresse Gmail, vous pouvez utiliser Google Colab en vous connectant depuis https://colab.research.google.com/?hl=fr. 

Google Colab permet (entre-autres) de coder en Python sur des notebooks. L'approche est légèrement différente que le codage dans un éditeur de texte tel que Sublime-Text ou Idle. Parmi les avantages :
- permet de programmer par "bouts de code"
- possibilité de lancer une partie ciblée de son code
- nombreux packages déjà installés, et possibilité d'utiliser pip pour les autres
- facilité pour partager du code

Toutefois, il faudra vous former à ce nouvel outil. Pour cela, vous avez à votre disposition pas mal de ressources. Cette vidéo, par exemple, est une bonne introduction :
- https://www.youtube.com/watch?v=f7T_CMm8z8s
