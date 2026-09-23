# Site CV — Célia Quadrado

## RGPD / polices

Aucune requête vers Google Fonts ni vers un autre service tiers n'est faite. Les polices
sont auto-hébergées dans `fonts/`. Le site n'utilise ni cookie ni outil de mesure d'audience.

## Contenu du dossier

- `index.html` — le site complet : HTML et CSS statiques, quelques lignes de JavaScript
  (facultatives) pour surligner la rubrique courante dans le menu. C'est ce fichier qu'on
  modifie directement pour mettre à jour le CV.
- `fonts/` — les fichiers de polices `.woff2` + `fonts.css` (déclarations `@font-face`).
- `images/` — les images du site (`cyanotypes.jpg`, aussi utilisée pour l'aperçu sur les
  réseaux sociaux).
- `favicon.svg`, `robots.txt`, `sitemap.xml`, `CNAME` — fichiers de mise en ligne.
- `source/` — ancienne version du site (générée avec React), conservée pour archive ;
  elle n'est plus utilisée.

## Utilisation

Double-cliquez sur `index.html` pour ouvrir le site dans un navigateur.

## Mise en ligne

Le site est publié par GitHub Pages sur https://cv.quadrado.fr/. Mettez en ligne
`index.html` **avec** les dossiers `fonts/` et `images/` et le fichier `favicon.svg`.
Pensez à mettre à jour la date `<lastmod>` de `sitemap.xml` à chaque modification.

## Sécurité (Cloudflare)

Cloudflare ajoute des en-têtes de sécurité, dont une `Content-Security-Policy`
(Rules → Transform Rules → Modify Response Header). Elle n'autorise que le script en
bas de `index.html`, identifié par son empreinte `sha256-…`. **Si ce script est modifié**,
il faut recalculer l'empreinte et la remplacer dans la règle Cloudflare, sinon le
surlignage du menu ne fonctionne plus (le reste du site continue de marcher). Modifier
le texte ou le CSS du CV ne change rien.

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
