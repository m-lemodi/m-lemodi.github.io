# Site Personnel - Merlin FAREZ

Bienvenue sur le dépôt de mon site personnel et blog, construit avec Jekyll et hébergé sur GitHub Pages.

## Structure du projet

```
.
├── _config.yml          # Configuration principale de Jekyll
├── _posts/              # Articles de blog (format: YYYY-MM-DD-titre.md)
├── _layouts/            # Modèles de pages
├── _includes/           # Composants réutilisables
├── _sass/               # Styles Sass (optionnel)
├── _data/               # Données structurées
├── index.md             # Page d'accueil (Français)
├── index-en.md          # Page d'accueil (Anglais)
├── blog.md              # Page du blog
├── style.css            # Styles CSS
├── CV_MerlinFAREZ_FR.pdf # CV en PDF
└── README.md            # Ce fichier
```

## Comment ajouter un article de blog

1. Créer un nouveau fichier dans `_posts/` avec le format `YYYY-MM-DD-titre-de-l-article.md`
2. Ajouter le front matter requis:

```markdown
---
layout: post
title: "Titre de l'article"
date: YYYY-MM-DD HH:MM:SS +0100
author: Merlin FAREZ
categories: [categorie1, categorie2]
tags: [tag1, tag2]
---

Votre contenu en Markdown ici...
```

3. Utiliser Markdown pour le contenu (support GFM - GitHub Flavored Markdown)

## Développement local

Pour tester localement, vous avez besoin de:
- Ruby 2.6+ (recommandé: 3.0+)
- Bundler
- Jekyll

Installation:
```bash
# Installer les dépendances
gem install bundler jekyll

# Installer les gems du projet
bundle install

# Lancer le serveur de développement
bundle exec jekyll serve --livereload

# Accéder à http://localhost:4000
```

## Déploiement

Le site est automatiquement déployé sur GitHub Pages à l'adresse:
https://m-lemodi.github.io

Toute modification poussée sur la branche `master` sera automatiquement compilée et déployée par GitHub.

## Personnalisation

- **Thème**: Modifiez `_config.yml` pour changer le thème
- **Styles**: Éditez `style.css` pour personnaliser l'apparence
- **Layouts**: Modifiez les fichiers dans `_layouts/` pour changer la structure
- **Navigation**: Éditez les fichiers dans `_includes/header*.html`

## Licence

Ce projet est sous licence MIT. Voir le fichier LICENCE pour plus de détails.

## Contact

Pour toute question ou suggestion, vous pouvez me contacter via:
- Email: merlin.farez@epita.fr
- GitHub: https://github.com/m-lemodi