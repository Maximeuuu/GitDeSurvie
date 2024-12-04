# Résolution des conflits

## A - Situations de conflit

- Modifications sur le même fichier localement
- Modifications sur la même ligne
- Pas de synchronisation entre la branche locale et distante

## B - Résoudre

1. déterminer le conflit : `git diff --cc <fichier>`
    - `<<<<<<< HEAD` : indique la ligne locale
    - `=======`      : indique la séparation
    - `>>>>>>`       : indique la ligne distante
2. éditer le fichier
3. remplacer ce qu'il y a entre `<<<<<<<` HEAD' et `>>>>>>` par la version corrigée de la ligne
4. enregistrer le fichier
5. mettre à jour le référenciel local et distant
    - `git status`
    - `git add <fichier>`
    - `git commit -m "Conflit <fichier> résolu"`
    - `git push`

## C - Problèmes de retour à la ligne

1. git add --renormalize .
