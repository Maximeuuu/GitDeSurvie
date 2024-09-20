Fonctionnalité -> Issue -> Branche
===

## A - Infos branches

- 'main' : branche principale qui correspond à une version finie du projet disponible de l'extérieure
- 'dev' : branche principale de dévelopement non disponible pour l'extérieur
- 'feature branch' : branches supplémentaires temporaire de fonctionnalité.

Chaque fonctionnalité indépendante doit être dans une nouvelle branche.

## B - Initialisation du projet

- inviter des collaborateurs : `settings > Collaborator people >` saisir id utilisateur

## C - Ajouter une nouvelle fonctionnalité

### a. Le chef de projet

**Créer une issue :**

1. Aller sur GitHub dans l'onglet "Issues" du dépôt.
2. Cliquer sur `New issue`.
3. Remplir la description de l'issue

### b. Le développeur

**Ajouter la fonctionnalité :**

1. `cd <PROJET>`
2. Créer une nouvelle branche dédiée : `git checkout -b <BRANCHE-FEATURE>`
3. Ajouter la/les fonctionnalité/s dans le code
4. Mettre à jour la branche
```git
git add .
git commit -m "Ajout de ..."
```
5. "Comparer et pousser" la branche de fonctionnalité vers la branche principale : `git push origin <BRANCHE-PRINCIPALE>`

**Proposer une révision de code :**

1. Aller sur GitHub dans l'onglet "Code" du dépôt
2. Cliquer sur `Compare & pull request`
3. Remplir les détails et soumettre la pull request
4. Ajouter un reviewer dans la partie "Assignees"
5. Attendre la validation externe

### c. Le reviewer

**Valider le travail :**

1. Aller sur GitHub
2. Aller sur le projet puis au menu "Pull requests"
3. Vérifier le code
4. Accepter la fusion avec `Merge pull request` puis `Confirm merge`

**Nettoyer l'espace de projet :**

1. Voir toutes les branches : "Code" > `main` > `View all branches`
2. Effacer la branche de fonctionnalité
3. Aller dans le menu "Issues" puis dans l'issue ouverte liée
4. Fermer l' "issue" en cliquant sur : `Close issue`
