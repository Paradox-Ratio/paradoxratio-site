# Exploitation du site public

Le site reste un site statique déployé par GitHub Pages via le workflow existant. Il ne dépend pas directement de Supabase et ne nécessite aucune variable Render. Le contenu public est volontairement informatif et ne consomme plus de contenu dynamique de pronostics.

## Vérification après publication

Vérifier le workflow GitHub Pages, puis contrôler `https://paradoxratio.com` et `https://www.paradoxratio.com` en HTTP 200. Contrôler également que la page ne contient pas de termes de bookmaker, de cotes, d’offres de mise, de résultats gagné/perdu ou de lien d’affiliation.

## Rollback

Le retour au commit précédent est sans migration : il suffit de restaurer le commit GitHub Pages précédent et de relancer le workflow. Les fichiers `index.html`, `legal.html`, `cgv.html`, les images et le domaine CNAME restent indépendants du CMS Render.
