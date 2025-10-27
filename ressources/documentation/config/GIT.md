# Installation et configuration de Git

## Installation

### 1 - Téléchargement

- [Télécharger Git](https://git-scm.com/downloads)

### 2 - Installation

- initial branch : Override the default branch name for new repositories `main`
- choose the default behavior of git pull : default (fast-forward or merge)

---

## Configuration

### A - Configuration utilisateur

- `git config --list` : liste des configuration
- `git config --global user.name "Maxime"` : ajouter un auteur
- `git config --global user.email "<email>"` : ajouter un email
- `git config --global init.defaultBranch main` : Changer la branche par défaut à "main"

### B - Vérification connexion SSH

- ping github : `ssh git@github.com`
- connaitre les informations de connexion utilisées : `ssh -v git@github.com`