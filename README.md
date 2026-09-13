# BDR-C 2026-2027 — site du cours

Site de l'unité BDR (Bases de données relationnelles) à la
[HEIG-VD](https://heig-vd.ch), classe BDR-C, construit avec
[Quarto](https://quarto.org) : https://heigvd-bdr-c-26.github.io/

## Structure

```
_quarto.yml        config du site (navigation, thème)
_variables.yml     valeurs propres à l'année (organisation, liens)
index.qmd          Planning
materiel/          Matériel de cours : table chapitre → slides PDF, compléments
labos/             Consignes et une page par labo
exercices/         Énoncés et corrigés par chapitre
projet/            Phases, échéances, livrables
assets/            thème et logo
```

Les fichiers réservés aux membres de l'organisation (slides PDF, corrigés)
sont dans le dépôt privé `cours` ; le site y pointe via la variable
`files-url`. Les fichiers placés à côté des pages (p. ex. `materiel/company.postgres.sql`)
sont publiés avec le site, donc publics.

## Aperçu local

```sh
quarto preview
```

Le site est rendu et déployé sur GitHub Pages par
`.github/workflows/publish.yml` à chaque push sur `main`.

## Auteurs

Slides d'origine : N. Fatemi, C. Meier, O. Lemer (HEIG-VD). Site et
adaptation : O. Tischhauser.
