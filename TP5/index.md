**Nom :** Maxime Lemoine

**Groupe :** B

**Année :** 2023

**IUT Le Havre - Cours GIT**

---

# Compte-rendu TP5 - Site web sur GitHub pages
[tp5](https://abderzah.github.io/Introduction-GIT/tp5/)

## initialiser le site
1. https://github.com/<utilisateur>/<projet>
2. rendre publique : `settings` > `change visibility` > `make public`
3. source : `deploy from a branch`, branch : `main`, folder : `/(root)`
4. ajouter la page : `add file` > `README.md` ou `index.md`

## liens utiles
- [Liste des thèmes](https://pages.github.com/themes/)
- [Ajouter un thème](https://docs.github.com/fr/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll)

## ajouter un thème
1. ajouter un theme : `add file` > `_config.yml`
2. dans le fichier de configuration :
	`
	remote_theme: pages-themes/<[nom-theme](https://pages.github.com/themes/)>@v0.2.0
	plugins:
	- jekyll-remote-theme # add this line to the plugins list if you already have one
	 
	title: <titre>

	description: <description>

	gem "github-pages", group: :jekyll_plugins
	`

3. `commit changes` puis attendre 10min

## ajouter du contenu
- utiliser [markdown](https://www.markdownguide.org/)
- utiliser [html](https://www.w3schools.com/tags/default.asp)

## accèder à la page
lien : `https://<utilisateur>.github.io/<projet>/`


* * *


# page web avec markdown - exemple

## lien vers une page
- [lien](https://github.com/Maximeuuu/tp5)

## image
![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

## tableau
| Item         | Pris | Stock |
|--------------|:-----:|-----------:|
| Pommes |  1.99 |        739 |
| Bananas      |  1.89 |          6 |
