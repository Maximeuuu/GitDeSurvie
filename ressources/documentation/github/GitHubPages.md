# GitHub pages

## A - Initialiser le site

1. ``https://github.com/<utilisateur>/<projet>``
2. rendre publique : `settings` > `change visibility` > `make public`
3. source : `settings` > `pages` > `deploy from a branch`, branch : `main`, folder : `/(root)`
4. ajouter la page : `add file` > `README.md` ou `index.md`

## B - Liens utiles pour les thèmes

- [Liste des thèmes](https://pages.github.com/themes/)
- [Ajouter un thème](https://docs.github.com/fr/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll)

## C - Ajouter un thème

1. ajouter un theme : `add file` > `_config.yml`
2. dans le fichier de configuration :

    ```yml
    remote_theme: pages-themes/<[nom-theme](https://pages.github.com/themes/)>@v0.2.0
    plugins:
    - jekyll-remote-theme # add this line to the plugins list if you already have one
    
    title: <titre>
    
    description: <description>
    
    gem "github-pages", group: :jekyll_plugins
    ```

3. `commit changes` puis attendre 10min

## D - Ajouter du contenu

- utiliser du [markdown](https://www.markdownguide.org/)
- utiliser du [HTML](https://www.w3schools.com/tags/default.asp)

## E - Accèder à la page

lien : `https://<utilisateur>.github.io/<projet>/`
