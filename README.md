# 🎮 MyGame - Projet Unreal Engine 5

Bienvenue dans votre premier projet de jeu vidéo créé avec **Unreal Engine 5** !

---

## 📁 Ce qui a été créé dans ce dossier

Le projet est entièrement configuré en C++ et Blueprint avec les éléments suivants :

1. **`MyGame.uproject`** : Le fichier principal du projet Unreal Engine.
2. **`Source/MyGame/MyGameCharacter`** :
   - Contrôleur complet du personnage à la 3ème personne.
   - Système de santé (`CurrentHealth` / `MaxHealth`).
   - Système de score / pièces ramassées (`Score`).
   - Mécanique de sprint (vitesse normale à 600, sprint à 1000).
   - Caméra dynamique avec bras rétractable (`SpringArm` + `CameraComponent`).
3. **`Source/MyGame/CollectibleItem`** :
   - Objet ramassable en 3D qui tourne sur lui-même (`RotatingMovementComponent`).
   - Détection de collision (sphère de trigger) qui ajoute des points au joueur et affiche un message à l'écran.
4. **`Source/MyGame/MovingPlatform`** :
   - Plateforme mobile se déplaçant automatiquement en boucle (idéal pour les parcours de saut / plateformer).
5. **`Source/MyGame/MyGameGameMode`** :
   - Mode de jeu configuré pour spawner automatiquement votre personnage.
6. **`Config/`** :
   - Paramètres du moteur et touches configurées pour claviers **AZERTY** (Z, Q, S, D) et **QWERTY** (W, A, S, D), ainsi que les **manettes**.

---

## 🛠️ Prérequis indispensables

Unreal Engine n'est pas un simple script, c'est un moteur complet de plusieurs gigaoctets. Voici les deux éléments gratuits nécessaires pour le faire tourner sur votre PC :

1. **Epic Games Launcher & Unreal Engine 5** :
   - Téléchargez le lanceur sur [unrealengine.com](https://www.unrealengine.com/).
   - Ouvrez Epic Games Launcher -> Allez dans l'onglet **Unreal Engine** -> **Bibliothèque**.
   - Cliquez sur le `+` jaune et installez la version la plus récente (UE 5.4 ou 5.3).

2. **Visual Studio 2022 Community** (requis pour compiler le code C++) :
   - Téléchargez Visual Studio Community (gratuit) sur [visualstudio.microsoft.com](https://visualstudio.microsoft.com/).
   - Lors de l'installation, cochez impérativement la case : **"Développement de jeux en C++"** (*Game development with C++*).

---

## 🚀 Comment exécuter le jeu (Pas à pas)

### Option 1 : Ouvrir directement le projet

1. Faites un clic droit sur le fichier **`MyGame.uproject`**.
2. Cliquez sur **"Generate Visual Studio project files"** (cela va créer le fichier de solution `MyGame.sln`).
3. Double-cliquez sur **`MyGame.uproject`** : Unreal Engine va compiler les modules C++ et ouvrir l'éditeur graphique !

*(Note : si vous avez une version différente d'Unreal installée, faites clic droit sur `MyGame.uproject` -> **"Switch Unreal Engine version..."** et choisissez votre version).*

### Option 2 : Depuis Visual Studio 2022

1. Ouvrez le fichier **`MyGame.sln`** généré dans Visual Studio 2022.
2. En haut, assurez-vous que la configuration est bien sur **`Development Editor`** et la plateforme sur **`Win64`**.
3. Appuyez sur **F5** (ou `Ctrl + F5`) pour lancer la compilation et démarrer l'éditeur Unreal.

---

## 🕹️ Contrôles du jeu

| Action | Clavier AZERTY | Clavier QWERTY | Manette |
|---|---|---|---|
| **Avancer / Reculer** | **Z / S** | **W / S** | Stick gauche (Haut / Bas) |
| **Aller à gauche / droite** | **Q / D** | **A / D** | Stick gauche (Gauche / Droite) |
| **Tourner la caméra** | **Souris** | **Souris** | Stick droit |
| **Sauter** | **Espace** | **Espace** | Bouton A / Croix (Croix du bas) |
| **Sprinter** | **Shift Gauche** | **Shift Gauche** | Pression stick gauche (L3) |

---

## 📦 Comment créer un exécutable autonome (.exe) pour vos amis

Lorsque votre niveau est prêt dans Unreal Editor :
1. Allez dans le menu supérieur : **Platforms** -> **Windows**.
2. Cliquez sur **Package Project**.
3. Choisissez le dossier où enregistrer le jeu compilé.
4. Unreal générera un dossier avec un fichier `MyGame.exe` autonome jouable sans avoir besoin d'ouvrir l'éditeur !
