# 🎬 Scène par Scène

Application web pour apprendre l'anglais avec des scènes de séries, du niveau **A1 au C2**.
L'application elle-même tient dans **un seul fichier** : `index.html` (elle marche même ouverte seule, par double-clic). Quelques petits fichiers en plus (icônes, manifeste) servent uniquement à l'**installer sur le téléphone** et à l'utiliser **hors connexion**.

👉 **Ouvrir l'application** : `https://TON-PSEUDO.github.io/scene-par-scene/`
*(remplace `TON-PSEUDO` par ton nom d'utilisateur GitHub, et `scene-par-scene` par le nom de ton dépôt si tu l'as changé)*

## Ce que contient l'application

- **18 scènes** (3 par niveau, A1 → C2) avec répliques, traduction affichable et audio
- **Lecture audio** réplique par réplique, avec les mots surlignés pendant la lecture, vitesse et voix au choix
- **Vidéos** : colle le lien YouTube d'un extrait, il s'intègre dans la scène
- **Exercices** : quiz, dictée, texte à trous
- **Micro** : enregistre-toi sur une réplique et réécoute-toi
- **Vocabulaire** enregistré et classé par session, export CSV, révision par cartes
- **Lexique avancé B2 / C1 / C2** : 90 mots utiles et peu connus, avec quiz et mot du jour
- **Série de jours**, thème clair / sombre, sauvegarde de la progression

---

## 🚀 Mettre l'application en ligne (GitHub Pages, gratuit)

### 1. Créer le dépôt
1. Va sur [github.com](https://github.com) et connecte-toi (ou crée un compte gratuit).
2. Clique sur **New** (nouveau dépôt).
3. Nom : `scene-par-scene` (ou ce que tu veux). Mets-le en **Public**.
4. Coche **Add a README file**, puis **Create repository**.

### 2. Ajouter les fichiers
1. Dans le dépôt, clique sur **Add file → Upload files**.
2. Glisse-dépose **tous les fichiers** du projet en une seule fois :

   | Fichier | Rôle |
   |---|---|
   | `index.html` | **l'application** (le nom doit rester exactement `index.html`) |
   | `manifest.webmanifest` | permet l'installation sur l'écran d'accueil |
   | `sw.js` | permet l'usage hors connexion |
   | `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | l'icône de l'application |
   | `README.md` | ce guide (il remplace le README vide) |

3. Clique sur **Commit changes**.

> Tous les fichiers doivent être **à la racine** du dépôt (pas dans un sous-dossier). Si tu n'envoies que `index.html`, l'application fonctionne, mais sans installation ni mode hors connexion.

### 3. Activer GitHub Pages
1. Va dans **Settings → Pages**.
2. Dans **Build and deployment → Source**, choisis **Deploy from a branch**.
3. Branche : **main**, dossier : **/ (root)**, puis **Save**.
4. Attends 1 à 2 minutes et rafraîchis la page : l'adresse de ton application s'affiche en haut.

Elle sera de la forme :

```
https://TON-PSEUDO.github.io/scene-par-scene/
```

Ouvre ce lien : l'application est en ligne. 🎉

---

## 📱 L'ouvrir comme une vraie application

Une fois en ligne, ouvre le lien sur ton téléphone ou ton ordinateur et ajoute-le à l'écran d'accueil :

- **iPhone / iPad (Safari)** : bouton **Partager** → **Sur l'écran d'accueil**
- **Android (Chrome)** : menu **⋮** → **Ajouter à l'écran d'accueil** (ou **Installer l'application**)
- **Ordinateur (Chrome / Edge)** : icône **Installer** à droite de la barre d'adresse

L'application s'ouvre ensuite en plein écran, avec son icône, comme une application classique.

**Hors connexion** : ouvre l'application **une fois avec internet** ; ensuite elle se lance même sans réseau (seules les vidéos YouTube et le chargement des voix éventuelles en ligne ont besoin de connexion).

---

## ℹ️ Bon à savoir

- **Ta progression reste dans ton navigateur** (mots enregistrés, scores, série de jours). Elle est propre à chaque appareil et à chaque navigateur. Pour la déplacer ou la protéger, utilise **« Sauvegarder ma progression »** en bas de la page d'accueil, puis **« Restaurer »** sur l'autre appareil.
- **Le micro** ne fonctionne que sur une adresse sécurisée (`https://`), ce qui est le cas avec GitHub Pages. Le navigateur te demandera l'autorisation.
- **Les voix** viennent de ton appareil : elles varient selon le navigateur et le système. Chrome et Edge proposent en général le plus de voix anglaises.
- **Les vidéos** : sur chaque scène, le bouton « Chercher sur YouTube » ouvre une recherche. Colle ensuite le lien d'un extrait dans le champ prévu.

## 🔄 Mettre à jour l'application

Quand tu reçois une nouvelle version de `index.html` :

1. Dans ton dépôt, clique sur **Add file → Upload files**.
2. Envoie le nouveau fichier avec le **même nom** (`index.html`), puis **Commit changes** (GitHub remplace l'ancien).
3. Attends 1 à 2 minutes : la nouvelle version est en ligne. Ta progression est conservée.

Les autres fichiers (icônes, manifeste, `sw.js`) ne changent presque jamais : tu n'as à les renvoyer que si on te le demande. Si l'ancienne version s'affiche encore, ferme l'application puis rouvre-la (ou rafraîchis la page).

## 🩹 Un problème ?

| Symptôme | Solution |
|---|---|
| Page **404** sur l'adresse | Vérifie que le fichier s'appelle exactement `index.html`, qu'il est à la racine, et que **Settings → Pages** pointe sur `main` / `(root)`. Attends 2 minutes. |
| **Pas d'option « Installer »** | Ouvre l'adresse en `https://` (pas depuis un fichier local) et vérifie que `manifest.webmanifest` et les icônes sont bien dans le dépôt. Sur iPhone, utilise **Safari** → Partager → *Sur l'écran d'accueil*. |
| **Pas de son** | Vérifie le volume et que le mode silencieux n'est pas activé. Choisis une autre voix dans la liste de la scène. |
| **Micro refusé** | Autorise le micro dans les réglages du site (cadenas à côté de l'adresse). |
| **Progression perdue** | Elle est liée à l'adresse et au navigateur. Utilise **« Sauvegarder ma progression »** avant de changer d'adresse ou d'appareil, puis **« Restaurer »**. |

## 🛠️ Ajouter tes propres scènes

Les scènes sont écrites en haut du fichier `index.html`, dans la liste `SCENES`. Chaque scène contient :
`id`, `emoji`, `title`, `genre`, `level` (A1 à C2), `lines` (répliques), `tr` (traductions), `vocab` (expressions clés) et `quiz`.
Copie une scène existante, modifie-la, et elle apparaît automatiquement dans l'application (elle est classée selon son niveau).

## 🧠 Ajouter des mots au lexique

Le lexique avancé est la liste `LEX` dans `index.html`. Chaque ligne suit ce format :

```js
["C1", "mitigate", "atténuer, limiter", "Measures to mitigate the impact.", "Verbes"],
```

c'est-à-dire `[niveau, mot, sens en français, exemple, catégorie]`. Ajoute une ligne, elle apparaît dans l'onglet **Lexique**, le quiz et le mot du jour.

---

*Les scènes sont des dialogues originaux écrits pour l'application, dans l'esprit des séries.*
