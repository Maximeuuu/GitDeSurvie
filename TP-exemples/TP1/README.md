**Nom :** Maxime Lemoine

**Groupe :** B

**Année :** 2023

**IUT Le Havre - Cours GIT**

---

# Compte-rendu TP1 - GIT
[tp1](https://abderzah.github.io/Introduction-GIT/tp1/)

Dans ce TP on apprend à travailler avec git.
[GIT](https://education.github.com/git-cheat-sheet-education.pdf) permet d'avoir un historique des modifications apportées à des fichiers.

## Configuration
- liste des configuration : `git config --list`
- ajouter un auteur : `git config --global user.name "Maxime L"`
- ajouter un email  : `git config --global user.email "maxime.lemoine1@etu.univ-lehavre.fr"`

## Créer un dépot
1. `cd <repertoire>`
2. `git init`

## Suivre les changement d'un fichier dans GIT
1. créer le fichier                           : `gedit <fichier>`
2. liste des fichiers à inclure dans le dépot : `git status`
3. ajouter le fichier au dépot                : `git add <fichier>`
4. valider l'ajout                            : `git commit -m "<description de l'ajout>"` 
5. historique des versions enregistrées       : `git log`

## 3 états d'un ficher dans git
- sélection    : `git add`
- validation   : `git commit`
- récupération : `git checkout`

## fichier .gitignore
- permet d'ignorer certains fichiers dans le projet
- **#** permet de commenter

---

# Markdown
- [Markdown](https://www.markdownguide.org/cheat-sheet)
- création d'un fichier : README.md

## titres
* titres
	```md
	# h1
	## h2
	### h3
	```
* ajouter un identifiant
	`### My Great Heading {#custom-id}`

## Styles
* gras : `**bold text**`
* italique : `*italicized text*`
* barré : `~~The world is flat.~~`
* citation : `> blockquote`
* note : 
	```md
	Here's a sentence with a footnote. [^1]

	[^1]: This is the footnote.
	```
* indice : `H~2~O`
* exposant : `X^2^`

## Code
* zone de code : 
	```
	\```
	bloc
	de code
	\```
	```
	```
	`ligne de code`
	```

## Graphique
barre horizontale : 
	```
	---
	* * *
	```
	
## Images, liens, émojis et tableaux
* image : `![alt text](image.jpg)`
* lien : `[title](https://www.example.com)`
* émoji : `:joy:`
* tableau :
	```md
	| Syntax | Description |
	| ----------- | ----------- |
	| Header | Title |
	| Paragraph | Text | 
	```

## Listes
* Ordonné :
	```md
	1. First item
	2. Second item
	3. Third item
	```
* Non ordonné :
	```md
	- First item
	- Second item
	- Third item
	```
* Liste de tache :
	```md
	- [x] Write the press release
	- [ ] Update the website
	- [ ] Contact the media 
	```
* Définition
	```md
	 	term
	: definition 
	```

