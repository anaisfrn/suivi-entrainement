# Suivi d'entraînement 🏋️

Application web personnelle pour suivre mes séances de musculation et ma progression.
Une seule page HTML autonome, hébergée sur GitHub Pages — accessible via le même lien
sur téléphone comme sur ordinateur.

## Deux modes

- **Analyse** — tableau de bord du bloc : volume total, régularité, heatmap charge ×
  semaine par exercice, et courbes de progression (charge max / volume / 1RM estimé).
- **S'entraîner** — mode séance en direct, pensé pour le téléphone : chrono, saisie au
  ± (poids en **lb**, reps), validation des séries, et un **comparatif avec la séance
  précédente** pour viser au moins pareil, sinon plus lourd. Record du bloc mis en
  avant, récap de fin de séance.

## Données & synchronisation

- Les séances saisies sont enregistrées **dans le navigateur** (localStorage), donc
  **par appareil**. Il n'y a pas de base de données ni de compte.
- Pour passer tes données d'un appareil à l'autre : **S'entraîner → Sauvegarde &
  transfert → Exporter** (fichier `.json`), puis **Importer** sur l'autre appareil.
  L'import est additif et dédoublonné : il n'écrase jamais les données déjà présentes.

## Mettre à la page d'accueil du téléphone

Ouvrir le lien dans le navigateur mobile, puis *Partager → Ajouter à l'écran
d'accueil* pour l'utiliser comme une application.

## Blocs

L'app gère plusieurs blocs de programme (sélecteur **Bloc 5 / Bloc 4** dans Analyse et dans
S'entraîner). Les séances fessiers changent à chaque bloc ; les hauts du corps (Upper 1 / 2)
sont communs. Un même exercice garde son historique d'un bloc à l'autre : « La dernière fois »
et les records tiennent compte de tous les blocs.

## Source

Données initiales du Bloc 4 importées depuis mon fichier Excel de suivi ; les blocs suivants sont saisis dans l'app. Charges
exprimées en livres (lb), telles que saisies.

---

Généré avec [Claude Code](https://claude.com/claude-code).
