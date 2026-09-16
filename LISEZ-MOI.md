# Site CV — Célia Quadrado

## RGPD / polices

Aucune requête vers Google Fonts n'est faite, ni par `index.html`, ni par la version
source. Les polices sont fournies dans ce dossier (`fonts/`) et intégrées directement
dans `index.html`. Rien ne sort du navigateur du visiteur.

## Contenu du dossier

- `index.html` — le site complet en un seul fichier, autonome : code, styles et polices
  intégrés. Fonctionne hors ligne, aucun fichier externe nécessaire.
- `fonts/` — les fichiers de polices `.woff2` + `fonts.css` (déclarations `@font-face`
  auto-hébergées).
- `source/` — la version source modifiable (`Site CV Celia Quadrado.html` + `support.js`),
  qui charge les polices depuis `../fonts/fonts.css`.

## Utilisation

Double-cliquez sur `index.html` pour ouvrir le site dans un navigateur.

## Mise en ligne

Option 1 (la plus simple) : déposez `index.html` seul à la racine de votre hébergement
(GitHub Pages, Netlify, Vercel…). Aucun autre fichier n'est nécessaire.

Option 2 : mettez en ligne `source/Site CV Celia Quadrado.html` renommé `index.html`,
avec `support.js` à côté et le dossier `fonts/` ; corrigez alors le chemin du CSS en
`fonts/fonts.css` (au lieu de `../fonts/fonts.css`).

## Polices utilisées

- Instrument Serif (400, italique) — titres
- Instrument Sans (400, 500) — textes courants
- IBM Plex Mono (400, 500) — étiquettes, dates, petites capitales

Les trois sont sous licence SIL Open Font License : utilisation libre, y compris
commerciale, et auto-hébergement autorisé. Seuls les jeux de caractères latin et
latin-ext sont inclus (suffisant pour le français).

## Couleurs

- Fond papier : `#f4f1ec`
- Encre : `#1b1a17`
- Terracotta (accent) : `#b5603c`
- Vert (secondaire) : `#3f7a5f`
- Cartes : `#eae6dd` et `#e5ece7`
