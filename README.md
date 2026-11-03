# Mieux Manger

PWA perso : profils du foyer, menus de la semaine équilibrés selon le budget, liste de courses avec tes prix. Fonctionne hors connexion une fois installée. Les données restent sur le téléphone.

## Contenu

- `index.html` : toute l'application
- `manifest.webmanifest` : nom, couleurs et icônes pour l'installation
- `sw.js` : service worker (mode hors connexion)
- `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` : icônes de l'app

## Mettre en ligne sur GitHub Pages (une fois)

1. Sur github.com, crée un nouveau dépôt **public** nommé `mieux-manger` (bouton **New**).
2. Dans le dépôt, clique **Add file → Upload files** et sélectionne les 8 fichiers du dossier. Valide avec **Commit changes**.
3. Va dans **Settings → Pages**. Dans *Source*, choisis **Deploy from a branch**, branche **main**, dossier **/ (root)**, puis **Save**.
4. Après une minute environ, l'app est en ligne à l'adresse :
   `https://pellizzarimax.github.io/mieux-manger/`

## Installer sur le téléphone

- **iPhone (Safari)** : ouvre l'adresse, bouton **Partager** → **Sur l'écran d'accueil**.
- **Android (Chrome)** : ouvre l'adresse, menu **⋮** → **Installer l'application** (ou « Ajouter à l'écran d'accueil »).

## Mettre à jour l'app

1. Remplace `index.html` dans le dépôt (Upload files, même nom).
2. Dans `sw.js`, passe `mieux-manger-v1` à `mieux-manger-v2` (puis v3, etc.) et envoie-le aussi.
3. Ferme et rouvre l'app sur le téléphone : la nouvelle version se charge.

## Bon à savoir

- Les profils, menus, prix et liens sont enregistrés dans le navigateur du téléphone. Ils ne sont pas partagés entre appareils, et effacer les données du navigateur les supprime.
- Le dépôt étant public, le code est visible, mais **pas tes données** : elles ne quittent jamais le téléphone.
- Les prix par défaut sont des moyennes estimées : remplace-les par les tiens dans la liste de courses.
