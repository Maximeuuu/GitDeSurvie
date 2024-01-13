Duplication de projets github
===

## A - Créer un nouveau dépot GitHub à partir d'un projet existant

*Utile si on veut une copie indépendante COPIE_PROJET du premier projet PROJET_ORIGINE sur notre compte GitHub.
Il n'y aura plus aucune relation avec le projet initial PROJET_ORIGINE tout en ayant conservé l'historique sur COPIE_PROJET.*

1. Créer un nouveau dépot ``COPIE_PROJET`` complètement vide
2. ``git clone COPIE_PROJET``
3. ``cd COPIE_PROJET``
4. ``git remote add original PROJET_ORIGINE``
5. ``git pull original main``
6. ``git push origin main``


## B - Réunir plusieurs dépots dans un seul dépot GitHub

Dans GitHub :

1. Créer un nouveau projet ``repositories > new``
2. Lui donner un nom (exemple : projets)
3. Récupérer l'URL du projet

Dans un terminal :

1. Créer un nouveau répertoire : ``mkdir <repertoire>``
2. Se déplacer dedans : ``cd <repertoire>``
3. Créer un répertoire pour chaque projet à réunir : ``mkdir <projetX>``
4. Cloner chaque repertoire : ``git clone <url_projetX>``
5. Supprimer le ``.git`` de chaque répertoire cloné
6. Ajouter le contenu à l'index GIT : ``git add .``
7. Enregistrer les modifications : ``git commit -m "Initial commit"``
8. Ajouter le référenciel distant : ``git remote add origin <url_projet>``
9. Vérifier que l'origine est bien configuré : ``git remote -v``
10. Envoyer le projet local vers le distant : ``git push -u origin main``
