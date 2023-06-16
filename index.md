**Nom :** Maxime Lemoine

**Année :** 2023

**IUT Le Havre - GIT**

---

# Initiation GIT


* [TP1](https://github.com/Maximeuuu/initiation_GIT/tree/main/TP1)
* [TP2](https://github.com/Maximeuuu/initiation_GIT/tree/main/TP2)
* [TP3](https://github.com/Maximeuuu/initiation_GIT/tree/main/TP3)
* [TP4](https://github.com/Maximeuuu/initiation_GIT/tree/main/TP4)
* [TP5](https://github.com/Maximeuuu/initiation_GIT/tree/main/TP5)

* * *

## Exporter un projet local sur GitHub

Dans GitHub :

1. Créer un nouveau projet ``repositories > new``
2. Lui donner un nom (exemple : projet)
3. Récupérer l'URL du projet

Dans un terminal :

1. Se déplacer dans le projet local à exporter : ``cd <repertoire>``
2. Initialiser le dépot GIT : ``git init``
3. Ajouter le contenu à l'index GIT : ``git add .``
4. Enregistrer les modifications : ``git commit -m "Initial commit"``
5. Ajouter le référenciel distant : ``git remote add origin <url_projet>``
6. Vérifier que l'origine est bien configuré : ``git remote -v``
7. Envoyer le projet local vers le distant : ``git push -u origin main``

* * *

## Réunir plusieurs projets GitHub dans un seul répertoire de projet

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

* * *

## Commandes utiles

* changer le branche par défaut : ``git config --global init.defaultBranch main``
