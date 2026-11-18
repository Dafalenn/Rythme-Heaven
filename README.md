# Rythim Heaven

Jeu de rythme mobile (téléphone, clavier, manette) : importez vos propres musiques, les notes sont générées d'après le BPM et les voix.

Un seul fichier, `index.html`, sans dépendance. Aucune musique, vidéo ou image n'est incluse : tout vient du joueur (importé dans le navigateur, jamais envoyé nulle part).

## Mettre en ligne (GitHub Pages)

1. Créez un dépôt GitHub et poussez ces fichiers à la racine (branche `main`).
2. Dépôt → **Settings → Pages → Build and deployment → Source : GitHub Actions**.
3. Le workflow `.github/workflows/pages.yml` publie le jeu à chaque push.
4. Adresse : `https://<votre-compte>.github.io/<nom-du-depot>/`

Sans Actions : Settings → Pages → Source « Deploy from a branch » → `main` / `(root)`.

## Remarques

- Réglages, nom, touches, configuration de la manette et images sont enregistrés **dans le navigateur de chaque appareil** (localStorage) : il faut les refaire sur un autre appareil.
- Le jeu doit être servi en `https://` (GitHub Pages le fait) ou ouvert comme fichier local.
