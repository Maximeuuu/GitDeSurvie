# Duplication de projets

## A - Créer un nouveau dépot à partir d'un projet existant

*Utile si on veut une copie **indépendante** COPIE_PROJET du premier projet PROJET_ORIGINE.
Il n'y aura plus aucune relation avec le projet initial PROJET_ORIGINE tout en ayant conservé l'historique sur COPIE_PROJET.*

1. Créer un nouveau dépot `COPIE_PROJET` complètement vide
2. `git clone COPIE_PROJET`
3. `cd COPIE_PROJET`
4. `git remote add original PROJET_ORIGINE`
5. `git pull original main`
6. `git push origin main`

## B - Réunir plusieurs dépots dans un seul dépot

Préparer le dépot

1. Créer un dépot `GROUPE_PROJET`
2. Cloner : `git clone GROUPE_PROJET`
3. Aller dans le dépot : `cd GROUPE_PROJET`

Ajouter les dépot `SOUS_PROJET_X` à `GROUPE_PROJET`

1. Cloner chaque projet à réunir : `git clone SOUS_PROJET_X`
2. Supprimer le dossier `.git` de chaque sous-projet

Indexer le contenu

1. `git add .`
2. `git commit -m "groupement des sous projets"`
3. `git push`
