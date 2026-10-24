# ⚡ CyberRunner 3D : L'Aventure Céleste

Jeu d'arcade et de plateforme en 3D qui se joue directement dans le navigateur. Traversez des îles flottantes, ramassez les pièces, écrasez les ennemis et atteignez le portail final !

Réalisé par **ANTON NELCON Steve**.

<img width="1912" height="867" alt="image" src="https://github.com/user-attachments/assets/4d151ed4-44c1-4793-b6e6-61a2f758b429" />


---

## 🎮 Présentation

CyberRunner 3D est un jeu de plateforme 3D à la troisième personne, développé en **HTML / JavaScript** avec la bibliothèque **[Three.js](https://threejs.org/)**. Aucune installation n'est nécessaire : il suffit d'un navigateur récent compatible WebGL.

**Objectif :** ramasser les **10 pièces** du niveau, éviter les dangers, vaincre les ennemis et franchir le **portail final**, le tout le plus vite possible.

---

## ✨ Fonctionnalités

- 🤖 **4 héros jouables**, chacun avec ses propres atouts
- 🪙 **10 pièces** à collecter
- 👾 **Ennemis** à écraser en leur sautant dessus
- 🚩 **Drapeaux de checkpoint** : en cas de chute, on repart du dernier drapeau activé
- 🧱 **Plateformes mobiles** et **bouncepads** (tremplins)
- 🎁 **Power-ups** : boost de vitesse, bouclier et aimant à pièces
- 🌌 **4 décors de ciel**, modifiables en cours de partie
- ⏱️ **Chronomètre**, compteur de vies, de pièces et d'ennemis vaincus
- 🔊 **Effets sonores** générés avec la Web Audio API, avec bouton pour couper le son
- 🏆 Écran de victoire avec récapitulatif (pièces, ennemis, temps)

---

## 🤖 Les héros

| Héros | Spécialité | Détails |
|-------|-----------|---------|
| 🤖 **CyberBot** | ⚖️ Équilibré | Polyvalent et agile, double saut, 3 vies |
| 🥷 **Shadow Ninja** | 🥷 Triple saut | Plus rapide, triple saut aérien, 3 vies |
| 🛡️ **Giga Titan** | ❤️ 5 vies max | Colosse blindé, plus lent mais plus résistant |
| ⚡ **Neon Flash** | ⚡ Hyper vitesse | Vitesse de pointe exceptionnelle et saut renforcé, 3 vies |

---

## 🌌 Les décors

| Décor | Ambiance |
|-------|----------|
| 🌌 **Nébuleuse Cosmique** | Ciel étoilé avec planète à anneaux |
| 🌅 **Crépuscule Doré** | Grand soleil couchant |
| 🌠 **Aurore Boréale** | Ciel étoilé aux teintes vertes |
| ☀️ **Ciel Céleste Azur** | Plein jour, ciel bleu |

---

## 🕹️ Contrôles

| Action | Touche |
|--------|--------|
| **Se déplacer** | `Z` `Q` `S` `D` |
| **Sauter** (double saut possible) | `Espace` |
| **Changer de ciel** | `V` |
| **Changer de héros** | `C` |
| **Réapparaître au dernier drapeau** | `R` |
| **Orienter la caméra** | Souris |

Des boutons en haut de l'écran permettent aussi de changer de ciel, de héros, de verrouiller la souris (mode « Vue Libre » / FPS-TPS) et de couper le son.

💡 **Astuce :** sautez sur les ennemis 👾 pour les vaincre, mais attention à ne pas les toucher de côté, vous perdriez une vie !

---

## 🚀 Lancer le jeu

### Méthode rapide (Windows)

Double-cliquez sur **`Lancer_Le_Jeu.bat`**.

### Méthode universelle (Windows, macOS, Linux)

1. Téléchargez ou clonez le dépôt :
   ```bash
   git clone https://github.com/an-Steve/CyberRunner3D.git
   ```
2. Ouvrez le fichier **`index.html`** dans votre navigateur (Chrome, Edge, Firefox…).

C'est tout ! Aucun moteur de jeu, compilateur ou dépendance à installer.

> 🌐 `three.min.js` est fourni dans le dépôt, donc le jeu fonctionne hors ligne. Si le fichier local est absent, le jeu bascule automatiquement sur la version hébergée par cdnjs (Three.js r128), ce qui demande alors une connexion Internet.

---

## 📁 Structure du projet

```
CyberRunner3D/
├── index.html          # Le jeu complet (interface, logique, sons)
├── three.min.js        # Bibliothèque Three.js (rendu 3D)
├── Lancer_Le_Jeu.bat   # Lanceur rapide pour Windows
├── .gitignore
└── README.md
```

---

## 🛠️ Technologies utilisées

- **HTML5 / CSS3** : interface et HUD
- **JavaScript** (sans framework) : logique du jeu
- **[Three.js](https://threejs.org/)** : rendu 3D WebGL
- **Web Audio API** : effets sonores

---

##  Auteur

**ANTON NELCON Steve**

---

Amusez-vous bien et bonne course ! 🏃⚡
