# Repo public GitHub Pages

Ce repo ne doit contenir que le site statique public.

Configuration GitHub Pages recommandee:

- `Settings > Pages`
- `Source`: `Deploy from a branch`
- `Branch`: `main`
- `Folder`: `/docs`

Le dossier `docs/` est alimente par `site-source-private/publish.ps1`.

## Ajouter une publication au blog

1. Copier `docs/_drafts/modele-publication.md` dans `docs/_posts/`.
2. Renommer la copie au format `AAAA-MM-JJ-titre-court.md` (par exemple `2026-09-15-separation-terres-rares.md`).
3. Remplacer le titre, la description et le contenu du modèle, puis publier les changements.

GitHub Pages génère automatiquement la page de l’article. La page Blog classe les publications de la plus récente à la plus ancienne d’après la date présente dans le nom du fichier.
