# Site LYNAQE — version optimisée

## Contenu
- `index.html` — la page du site (~200 Ko, contre 8 Mo avant)
- `images/` — les 41 photos et logos en WebP (+ favicon PNG), chargés à la demande

## Déploiement (GitHub → Cloudflare Pages)
1. Pousser **tout le contenu de ce dossier** (index.html + dossier images/) à la racine du dépôt GitHub.
2. Cloudflare Pages détecte le commit et redéploie automatiquement.
3. Aucun réglage de build nécessaire (site statique).

## Modifier le site
- Textes : directement dans `index.html`. Chaque texte a sa traduction anglaise
  dans le dictionnaire `I18N_EN` en bas du fichier ("Texte français": "English text").
- Ajouter une photo : placer le fichier `.webp` dans `images/` et le référencer
  dans le HTML (`<img loading="lazy" src="images/mon-image.webp">`).
