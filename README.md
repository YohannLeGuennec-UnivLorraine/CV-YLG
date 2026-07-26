# Repo public GitHub Pages

Ce repo ne doit contenir que le site statique public.

Configuration GitHub Pages recommandee:

- `Settings > Pages`
- `Source`: `Deploy from a branch`
- `Branch`: `main`
- `Folder`: `/docs`

Le dossier `docs/` est alimente par `site-source-private/publish.ps1`.

## Ajouter une publication au blog

1. Copier le dossier `docs/_drafts/modele-publication/` dans `docs/blog/posts/`.
2. Renommer la copie au format `AAAA-MM-JJ-titre-court` (par exemple `2026-09-15-separation-terres-rares`).
3. Dans son fichier `index.md`, renseigner `date`, `title`, `description` et le contenu.
4. Placer les images, PDF et autres documents associés dans ce même dossier.
5. Publier les changements.

Exemple de dossier :

```text
docs/blog/posts/2026-09-15-separation-terres-rares/
├── index.md
├── schema.png
└── donnees.pdf
```

Les ressources se référencent avec des liens relatifs depuis `index.md`, par exemple
`![Schéma du procédé](schema.png)` ou `[Télécharger les données](donnees.pdf)`.

GitHub Pages génère automatiquement la page de l’article. La page Blog classe les publications de la plus récente à la plus ancienne d’après le champ `date` de chaque fichier `index.md`.
