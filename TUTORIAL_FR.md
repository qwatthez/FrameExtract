# 📷 FrameExtract — Tutoriel Complet pour Débutants

**Bienvenue !** Ce guide vous explique comment installer et utiliser **FrameExtract** en français, **même si vous n'avez aucune expérience en informatique**.

---

## 📋 Table des matières

1. [Avant de commencer](#avant-de-commencer)
2. [Étape 1 : Télécharger Python](#étape-1--télécharger-python)
3. [Étape 2 : Télécharger FrameExtract](#étape-2--télécharger-frameextract)
4. [Étape 3 : Installer les dépendances](#étape-3--installer-les-dépendances)
5. [Étape 4 : Lancer le programme](#étape-4--lancer-le-programme)
6. [Étape 5 : Utiliser l'interface](#étape-5--utiliser-linterface)
7. [Résolution des problèmes](#résolution-des-problèmes)

---

## Avant de commencer

### Qu'est-ce que vous aurez besoin ?

- 💻 Un ordinateur Windows, Mac ou Linux
- 🎥 Des vidéos de pièges photos (format MP4, MOV ou AVI)
- 📁 Un dossier où vous gardez vos vidéos
- ⌚ Environ 10-15 minutes pour l'installation

**Aucune expérience en programmation n'est nécessaire !**

---

## Étape 1 : Télécharger Python

Python est un **logiciel gratuit** qui permet à FrameExtract de fonctionner. C'est comme d'avoir un "moteur" pour faire tourner le programme.

### Sur Windows :

1. Ouvrez votre navigateur web (Chrome, Edge, Firefox, etc.)
2. Allez sur : **https://www.python.org/downloads/**
3. Vous devriez voir un gros bouton jaune qui dit **"Download Python 3.x.x"** (le numéro peut être légèrement différent)
4. Cliquez dessus pour télécharger
5. Une fois téléchargé, **double-cliquez** sur le fichier téléchargé

**⚠️ IMPORTANT** : Quand l'installateur s'ouvre, **COCHEZ LA CASE** qui dit :
- ☑️ "Add Python 3.x to PATH" 

Cela permet à votre ordinateur de trouver Python. Puis cliquez sur **"Install Now"**.

6. Attendez que l'installation se termine (ça peut prendre 2-3 minutes)

### Sur Mac :

1. Ouvrez votre navigateur
2. Allez sur : **https://www.python.org/downloads/**
3. Téléchargez la version **macOS**
4. Double-cliquez sur le fichier téléchargé
5. Suivez les instructions (cliquez "Next" plusieurs fois)

### Vérifier que Python est installé

Maintenant, vérifions que tout fonctionne :

**Sous Windows :**
1. Appuyez sur la touche **Windows** de votre clavier
2. Tapez : `cmd`
3. Appuyez sur **Entrée**
4. Une fenêtre noire s'ouvre (c'est le "Terminal")
5. Tapez : `python --version`
6. Appuyez sur **Entrée**

Vous devriez voir quelque chose comme : `Python 3.11.0` ou similaire.

**Sous Mac :**
1. Appuyez sur **Cmd + Espace**
2. Tapez : `Terminal`
3. Appuyez sur **Entrée**
4. Une fenêtre s'ouvre
5. Tapez : `python3 --version`
6. Appuyez sur **Entrée**

Vous devriez voir : `Python 3.x.x`

✅ Si vous voyez un numéro de version, Python est installé ! Continuez.

---

## Étape 2 : Télécharger FrameExtract

Il y a deux façons de faire. Choisissez celle qui vous paraît la plus simple :

### Méthode 1 : Télécharger le fichier ZIP (la plus simple)

1. Allez sur le site GitHub du projet
2. Cherchez un bouton vert **"Code"** ou **"Download"**
3. Cliquez sur **"Download ZIP"**
4. Un dossier compressé se télécharge
5. **Double-cliquez** sur le fichier ZIP pour le décompresser
6. Un dossier nommé **"Videos_to_photos"** apparaît
7. Notez où ce dossier se trouve (par exemple : `Bureau` ou `Documents`)

✅ C'est fait ! Passez à l'étape 3.

### Méthode 2 : Utiliser Git (un peu plus avancé, mais très utile)

Si vous avez l'habitude des outils informatiques :

1. Installez **Git** depuis : https://git-scm.com/
2. Ouvrez le Terminal (cmd sous Windows, Terminal sous Mac)
3. Tapez :
```bash
git clone https://github.com/yourusername/Videos_to_photos.git
```
4. Appuyez sur Entrée
5. Le dossier se télécharge automatiquement

---

## Étape 3 : Installer les dépendances

Les "dépendances", ce sont les **petits programmes supplémentaires** dont FrameExtract a besoin pour fonctionner (comme les briques de LEGO qui s'assemblent).

### Sous Windows :

1. Ouvrez votre `Terminal` (appuyez sur Windows, tapez `cmd`, appuyez sur Entrée)
2. Naviguez vers le dossier **Videos_to_photos**. Tapez :
```bash
cd chemin\vers\Videos_to_photos
```

*(Remplacez "chemin\vers" par le vrai chemin de votre dossier. Par exemple si c'est sur le Bureau : `cd C:\Users\VotreNom\Desktop\Videos_to_photos`)*

3. Maintenant, créez un **environnement virtuel** (c'est un petit espace isolé juste pour ce programme). Tapez :
```bash
python -m venv venv
```

Attendez quelques secondes...

4. Activez cet environnement. Tapez :
```bash
venv\Scripts\activate
```

Vous devriez voir `(venv)` apparaître au début de la ligne. C'est bon signe !

5. Installez les dépendances. Tapez :
```bash
pip install -r requirements.txt
```

Attendez quelques minutes pendant que les logiciels s'installent. Vous verrez beaucoup de texte s'afficher.

### Sous Mac :

1. Ouvrez le `Terminal` (Cmd + Espace, tapez `Terminal`)
2. Allez dans le dossier Videos_to_photos. Tapez :
```bash
cd chemin/vers/Videos_to_photos
```

3. Créez l'environnement virtuel :
```bash
python3 -m venv venv
```

4. Activez-le :
```bash
source venv/bin/activate
```

Vous devriez voir `(venv)` apparaître.

5. Installez les dépendances :
```bash
pip install -r requirements.txt
```

Attendez que l'installation se termine.

---

## Étape 4 : Lancer le programme

Maintenant que tout est installé, lançons FrameExtract !

### Sous Windows :

1. **Vous devez toujours avoir le Terminal ouvert** (si vous l'avez fermé, réouvrez-le et faites à nouveau les étapes pour aller dans le dossier et activer venv)
2. Tapez simplement :
```bash
python app.py
```

3. Appuyez sur **Entrée**

Vous verrez peut-être quelque chose comme :
```
 * Serving Flask app 'app'
 * Running on http://127.0.0.1:5000
```

C'est parfait !

### Sous Mac :

1. **Le Terminal doit toujours être ouvert** (avec `(venv)` visible)
2. Tapez :
```bash
python3 app.py
```

3. Appuyez sur **Entrée**

Vous verrez la même chose.

### Ouvrir l'interface dans votre navigateur

1. Ouvrez votre navigateur web (Chrome, Firefox, Edge, Safari, etc.)
2. Allez à l'adresse : **http://localhost:5000**
3. L'interface FrameExtract s'ouvre ! 🎉

Vous devriez voir une belle interface avec :
- Un titre "Extrayez vos images de vidéos de pièges photographiques"
- Une zone pour glisser-déposer vos vidéos
- Des paramètres à régler

---

## Étape 5 : Utiliser l'interface

### 1️⃣ Sélectionner vos vidéos

**Vous avez deux options :**

**Option A : Glisser-déposer** (la plus facile)
1. Ouvrez votre dossier avec vos vidéos de pièges photos
2. Sélectionnez une ou plusieurs vidéos (MP4, MOV ou AVI)
3. Glissez-les vers la zone grise de l'interface qui dit "Glissez vos vidéos ici"
4. Relâchez la souris

La vidéo apparaît dans une petite carte avec son nom et sa taille.

**Option B : Parcourir**
1. Cliquez sur le bouton "parcourir vos fichiers"
2. Une fenêtre s'ouvre pour choisir vos fichiers
3. Sélectionnez une ou plusieurs vidéos
4. Cliquez "Ouvrir"

### 2️⃣ Régler les paramètres

Vous verrez trois curseurs :

**🕐 Intervalle (secondes)** 
- Combien de temps entre chaque image extraite
- **Exemple :** 1 seconde = 1 photo chaque seconde
- **Exemple :** 5 secondes = 1 photo toutes les 5 secondes
- *Pour un piège photo normal, 1-2 secondes est généralement bon*

**⏳ Délai départ (secondes)**
- Ignore le début de la vidéo
- **Exemple :** 0.5 seconde = saute les premières 0.5 secondes
- *Utile si le piège photo enregistre quelques secondes "blanches" au début*

**📐 Taille des images**
- La dimension des images qui seront extraites
- **100%** = taille originale (beaucoup de détails, fichiers plus gros)
- **50%** = moitié plus petite (fichiers plus légers, rapide)
- *Pour l'upload sur Agouti.eu, 100% ou 80% est recommandé*

### 3️⃣ Lancer l'extraction

1. Cliquez sur le grand bouton bleu **"▶ Lancer l'extraction"**
2. Vous verrez une barre de progression avec des statistiques :
   - Pourcentage complété
   - Nombre d'images extraites
   - Fichier en cours de traitement
3. **Patience !** Cela peut prendre quelques minutes selon la taille de vos vidéos

### 4️⃣ Télécharger les résultats

1. Quand l'extraction est terminée, vous verrez un message : ✅ **"Extraction terminée !"**
2. Un bouton **"⬇ Télécharger le ZIP"** apparaît
3. Cliquez dessus
4. Un fichier ZIP est téléchargé (par défaut dans votre dossier Téléchargements)
5. **Double-cliquez** sur le ZIP pour le décompresser
6. Vous trouvez un dossier avec toutes vos images extraites ! 🎉

### 5️⃣ Préparer les images pour Agouti.eu

1. Les images fonctionnent directement avec Agouti.eu
2. Vous pouvez les renommer si vous le souhaitez (pour une meilleure organisation)
3. Connectez-vous à votre compte Agouti.eu
4. Téléchargez les images dans vos relevés

---

## Résolution des problèmes

### ❌ "Python not found" ou "commande inconnue"

**Cause :** Python n'est pas correctement installé

**Solution :**
1. Vérifiez que Python est installé (voir Étape 1)
2. Sous Windows, réinstallez Python en **cochant bien la case** "Add Python to PATH"
3. Après la réinstallation, rouvrez le Terminal

### ❌ "Le Terminal disparaît immédiatement"

**Cause :** Erreur lors du lancement

**Solution :**
1. Ne relancez **pas** le programme en double-cliquant sur app.py
2. Utilisez toujours le Terminal (cmd sous Windows, Terminal sous Mac)
3. Suivez exactement les étapes 3 et 4

### ❌ "Page introuvable" ou "connexion refusée"

**Cause :** Le serveur n'a pas démarré correctement

**Solution :**
1. Vérifiez que le Terminal affiche bien : `Running on http://127.0.0.1:5000`
2. Attendez quelques secondes avant d'ouvrir le navigateur
3. Vérifiez que vous avez bien tapé : **http://localhost:5000** (pas https)
4. Essayez avec un autre navigateur (Chrome, Firefox, Edge)

### ❌ "Erreur lors de l'upload" ou "Fichier non supporté"

**Cause :** Format vidéo non reconnu

**Solution :**
1. Vérifiez que votre vidéo est en MP4, MOV ou AVI
2. Si c'est un autre format, convertissez-la (utilisez un outil comme Handbrake - gratuit)
3. Vérifiez que le fichier n'est pas corrompu

### ❌ "L'extraction est très lente"

**Cause :** Intervalle trop court ou vidéo très longue

**Solution :**
1. Augmentez l'intervalle (par exemple 2 ou 3 secondes au lieu de 1)
2. Réduisez la taille des images (50% au lieu de 100%)
3. Traitez une seule vidéo à la fois

### ❌ "Erreur lors du téléchargement du ZIP"

**Cause :** Dossier de téléchargements plein ou permissions

**Solution :**
1. Videz votre dossier Téléchargements
2. Assurez-vous que vous avez les droits d'écriture sur le dossier
3. Réessayez

---

## 💡 Conseils et astuces

### Pour les pièges photos

✅ **Intervalle recommandé :** 1-2 secondes
- Cela donne généralement les meilleurs résultats pour l'analyse comportementale

✅ **Taille recommandée :** 80-100%
- Cela préserve la qualité des images pour Agouti.eu et l'analyse

✅ **Délai départ :** 0 à 1 seconde
- Utile si votre caméra maison laisse un "blanc" au début

### Traitement par lots

Si vous avez beaucoup de vidéos :

1. **Lancez une première vidéo**
2. **Ouvrez une deuxième fenêtre** du navigateur
3. **Allez à nouveau sur http://localhost:5000**
4. Pendant que la première se traite, préparez la deuxième
5. Une fois la première terminée, lancez la deuxième

### Où trouver vos images extraites

- Les images se téléchargent dans un fichier ZIP
- Une fois décompressé, un dossier contient toutes vos images
- Vous pouvez les copier, renommer, ou supprimer comme n'importe quel fichier

---

## 🆘 Besoin d'aide supplémentaire ?

Si vous avez un problème non mentionné ci-dessus :

1. **Notez exactement le message d'erreur** que vous voyez
2. **Prenez une capture d'écran**
3. **Contactez le responsable du projet** sur GitHub ou par email
4. **Donnez le plus de détails possible :**
   - Votre système d'exploitation (Windows 10, Mac, etc.)
   - La version de Python
   - Le message d'erreur exact
   - Les étapes que vous avez suivies

---

## 🎉 Félicitations !

Vous avez maintenant **FrameExtract** qui fonctionne sur votre ordinateur ! 

Vous pouvez maintenant :
- ✅ Extraire des images de vos vidéos de pièges photos
- ✅ Les préparer facilement pour Agouti.eu
- ✅ Analyser le comportement des animaux avec des images plutôt que des vidéos
- ✅ Partager vos données facilement

**Bon travail !** 🐾📷

---

## Glossaire (pour les termes compliqués)

- **Terminal / Ligne de commande :** Une fenêtre noire où vous tapez des commandes texte
- **Python :** Un langage de programmation (un "langage" que les ordinateurs comprennent)
- **pip :** Un outil pour télécharger et installer des "petits programmes"
- **venv :** Un "espace isolé" pour que chaque programme ait ses propres outils
- **localhost:5000 :** L'adresse locale du serveur (127.0.0.1 c'est votre ordinateur, 5000 c'est le "port")
- **ZIP :** Un format de fichier compressé (comme une "valise" qui rend les fichiers plus petits)

---

**Version 1.0 - Avril 2026**
*Créé pour FrameExtract - Camera Trap Frame Extractor*
