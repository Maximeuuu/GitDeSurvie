Markdown
===

- [Markdown](https://www.markdownguide.org/cheat-sheet)

## A - Titres
* titres
	```md
	# h1
	## h2
	### h3
	```
* ajouter un identifiant
	`### My Great Heading {#custom-id}`

## B - Styles
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

## C - Code
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

## D - Graphique
barre horizontale :
	```
	---
	* * *
	```

## E - Images, liens, émojis et tableaux
* image : `![alt text](image.jpg)` ![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)
* lien : `[title](https://www.example.com)` [lien](https://github.com/Maximeuuu/tp5)
* émoji : `:joy:`
* tableau :
	```md
	| Syntax | Description |
	| ----------- | ----------- |
	| Header | Title |
	| Paragraph | Text |
	```
* tableau 2 :
	```md
	| Item         | Pris | Stock |
	|--------------|:-----:|-----------:|
	| Pommes |  1.99 |        739 |
	| Bananas      |  1.89 |          6 |
	```

## F - Listes
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
