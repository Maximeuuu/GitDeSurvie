# Markdown

- [Markdown](https://www.markdownguide.org/cheat-sheet)

## A - Titres

- titres

  ```md
  # h1
  ## h2
  ### h3
  ```

- ajouter un identifiant

  `### Titre {#identifiant}`

## B - Styles

- gras : `**TEXTE**` : **exemple**
- italique : `*TEXTE*` : *exemple*
- barré : `~~TEXTE~~` : ~~exemple~~
- citation : `> blockquote`
  > exemple
- note : `TEXTE [^X]` ... `[^X]: LA NOTE CONCERNANT LE TEXTE`

  Here's a sentence with a footnote. [^1]

  [^1]: This is the footnote.

- indice : `H~2~O` : H~2~O
- exposant : `X^2^` : X^2

## C - Code

- zone de code :

  ```md
  \```
  bloc
  de code
  \```
  ```

  ```md
  `ligne de code`
  ```

## D - Graphique

barre horizontale :

- `---`
- `***`

## E - Images, liens, émojis et tableaux

- image : `![alt text](image.jpg)`

  ![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)
- lien : `[title](https://www.example.com)` : [lien](https://github.com/Maximeuuu/tp5)
- émoji : `:joy:` : :joy:
- tableaux :

  ```md
  | Syntax | Description |
  | ----------- | ----------- |
  | Header | Title |
  | Paragraph | Text |
  ```

  ```md
  | Item         | Pris | Stock |
  |--------------|:-----:|-----------:|
  | Pommes |  1.99 |        739 |
  | Bananas      |  1.89 |          6 |
  ```

  | Syntax | Description |
  | ----------- | ----------- |
  | Header | Title |
  | Paragraph | Text |

## F - Listes

- Ordonnée :

  ```md
  1. First item
  2. Second item
  3. Third item
  ```

- Non ordonnée :

  ```md
  - First item
  - Second item
  - Third item
  ```

- Liste de tache :

  ```md
  - [x] Write the press release
  - [ ] Update the website
  - [ ] Contact the media
  ```

- Définition

  ```md
    term
  : definition
  ```
