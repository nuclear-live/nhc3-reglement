PATCH NHC #3 — DOCUMENTS MODÉRATEURS
======================================

Contenu :
- espace-moderateurs.md
- assets/documents/tuto-moderateurs-nhc3.pdf
- assets/documents/calculateur-points-nhc3.xlsx

INSTALLATION
------------
Déposez les fichiers à la racine du dépôt en conservant exactement leur arborescence.
Il n'est pas nécessaire de modifier _sass/custom/custom.scss : la page réutilise les cartes
et encadrés déjà présents dans la refonte NHC #3.

ÉTAT ACTUEL : NON PUBLIÉ
-------------------------
Le fichier espace-moderateurs.md contient :
  published: false
  nav_exclude: true
  search_exclude: true

Ainsi, la page n'est pas générée par GitHub Pages pour le moment.

POUR LA DIFFUSION OFFICIELLE
----------------------------
1. Remplacer :
     published: false
   par :
     published: true

2. Deux possibilités :
   - Laisser nav_exclude: true et search_exclude: true
     => la page existe mais reste accessible uniquement par son lien direct :
        /moderateurs/
   - Supprimer nav_exclude et search_exclude
     => la page pourra apparaître dans la navigation et la recherche du site.

IMPORTANT
---------
Le dépôt GitHub étant public, les PDF/XLSX ajoutés au dépôt restent techniquement visibles
par quelqu'un qui fouille directement les fichiers du dépôt, même tant que la page reste
non publiée. La page du site, elle, ne sera pas générée avec published: false.
