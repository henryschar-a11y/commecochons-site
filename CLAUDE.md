# Site commecochons.com

Site statique (HTML/CSS/JS, pas de build) du jeu « ...Comme cochons » d'Henry et Elisa.

## Modifier et publier
1. Modifier les fichiers dans ce dépôt, puis commit + push sur `main` (GitHub = source de vérité).
2. Publier sur Netlify : appeler l'outil Netlify `netlify-deploy-services-updater` (operation deploy-site, siteId 00c183c3-22b8-414b-b128-8d0a26caffeb), puis lancer depuis la racine du dépôt la commande `npx -y @netlify/mcp@latest --site-id ... --proxy-path "..."` qu'il renvoie.
3. Vérifier la page en ligne (https://commecochons.com).
Toujours publier depuis une copie à jour du dépôt, sinon on écrase le site en ligne.

## Repères
- Compteur de précommandes : index.html, `const NB_PRECOMMANDES` et `const EDITION = 100`.
- Prix affiché : 24,99 €, livraison offerte. Lien Stripe : https://buy.stripe.com/cNi7sDaqrd3F0H04EY53O02
- Ne jamais utiliser le caractère « — » dans les textes.
