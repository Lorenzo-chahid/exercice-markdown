# Tuto – Enrichir vos textes avec la syntaxe Markdown !
## 1. Intro
Devoir systématiquement passer par les balises HTML pour personnaliser du contenu peut être sacrément pénible… fort heureusement, [John Gruber](https://fr.wikipedia.org/wiki/John_Gruber) et [Aaron Swartz](https://fr.wikipedia.org/wiki/Aaron_Swartz) ont inventé la syntaxe Markdown pour nous simplifier la tâche !
##### … Markdown ?
Markdown est un petit langage très léger qui permet d'écrire l'équivalent de certaines balises HTML de façon simplifiée. Par exemple, si je veux écrire **grosmichel** en gras, plutôt que d'écrire `<strong>grosmichel</strong>`, Markdown me permet d'écrire uniquement `**grosmichel**` !

Cette syntaxe est notamment très utile sur **GitHub**, car elle correspond au format de vos fichiers `README.md`… que vous pouvez donc embellir très facilement en utilisant Markdown ! Elle est également prise en charge par de nombreux forums et logiciels de communication, tels que **Discord** (partiellement) et **Ryver** (totalement).
###### Le logo de Markdown
![](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg?uselang=fr)
##### Créer un fichier markdown
Pour créer un fichier markdown, rien de plus simple ! Il suffit de créer un nouveau fichier avec l'extension `.md`. Il ne vous reste ensuite qu'à l'ouvrir et à le modifier avec votre éditeur de texte préféré 🤠
##### Tester son Markdown
Si vous travaillez sur GitHub, il est tout bêtement possible de prévisualiser vos modifications avant de les *commit*. Autrement, il existe plusieurs éditeurs markdown en ligne, [en voici un](https://dillinger.io/).
## 2. Les différentes balises markdown
#### Balises de formatage
* **gras** (`<strong>`) ⇒ `**gras**`
* *italique* (`<em>`) ⇒ `*italique*`ou `_italique_`
* s̲o̲u̲l̲i̲gn̲é (`<u>`) ⇒ `__souligné__` (ne fonctionne pas sur GitHub ¯\\\_(ツ)_/¯)
* ~~barré~~ (`<strike>`) ⇒ `~~barré~~`
* `code` (`<code>`) ⇒ ``­`code`­``
    * On peut aussi utiliser la coloration syntaxique !
    ```javascript
    function toCamelCase(str) {
	for (let firstIndex = str.indexOf("_"); ~firstIndex; firstIndex = str.indexOf("_"))
		str = str.substring(0, firstIndex) + str.charAt(firstIndex + 1).toUpperCase() + str.substring(firstIndex + 2);
	return str;
    }
    ```
    ```
    `­`­`javascript
    function toCamelCase(str) {
	for (let firstIndex = str.indexOf("_"); ~firstIndex; firstIndex = str.indexOf("_"))
		str = str.substring(0, firstIndex) + str.charAt(firstIndex + 1).toUpperCase() + str.substring(firstIndex + 2);
	return str;
    }
    `­`­`
* > Et finalement, il est également possible de faire des citations (`<blockquote>`) en commençant notre ligne par '>'.

On peut carrément combiner des balises ! ~~***grosmichel***~~ ⇒ `~~***grosmichel***~~`
#### Listes
###### Listes à puces (`<ul>`)
```
* Un élément
* Un autre élément
    * Un sous élément avec au moins quatre espaces devant
```
**N. B.** : L'astérique peut être remplacé par un '+' ou un '-'
###### Listes ordonnées (`<ol>`)
```
1. Premier élément
2. Deuxième élément
``` 
###### Cases cochables (`<input type="checkbox">`)
- [ ] Case non cochée `- [ ]`
- [x] Case cochée `- [x]`
#### Titres
Titres de niveau 1 à 6 (`<h1>` à `<h6>`) :
```
# Titre de niveau 1
## Titre de niveau 2
### Titre de niveau 3
[…]
```
Pour les titres de niveaux 1 et 2, il est également possible de les souligner avec des '=' et des '-' (au moins 2) :
```
Titre de niveau 1
=================
Titre de niveau 2
-----------------
```
#### Tableaux
Les tableaux se définissent en séparant les différentes colonnes qui le constituent par des tuyaux ('|'). La première rangée de votre tableau contient le titre de la colonne, et la deuxième doit contenir au moins un tiret pour que le tableau soit correctement défini. L'ajout d'un deux-points permet de spécifier l'alignement du contenu : à droite, à gauche, ou au centre, suivant où vous placez le deux-point par rapport au tiret. Les troisième et énièmes lignes reçoivent le contenu des différentes colonnes.
```
|  Titre col. 1 |   Titre col. 2  |  Titre col. 3  |
| :------------ | :-------------: | -------------: |
| shrek         |     bourdon     |        Dreyfus |
| michel        |      HELP       |       aarrgghh |
| yahou!!       |     centre      |                |
```
#### Liens et images
Il est possible d'ajouter des [liens](https://www.youtube.com/watch?v=dQw4w9WgXcQ) par dessus le texte : `[texte à afficher](http://ton-lien.com)`… mais aussi des images !

![Une incroyable image](https://cdn.discordapp.com/attachments/453599269526568960/621678263055679519/LTFOE_Rire_du_Roi.gif "Un super titre")

Ajouter une image : `![texte alternatif](http://ton-lien.com "titre de l'image")`
## 3. Pour aller plus loin…
Rien à voir avec Markdown, mais en matière de personnalisation de vos textes, Unicode offre tout un tas de possibilités intéressantes !
1. **Ajouter des emoji** 👺
    * Le standard Unicode contient naturellement un bon paquet d'emoji que vous pouvez copier/coller dans vos textes. Une liste exhaustive des émoticônes utilisables est disponible à [cette adresse](https://unicode.org/emoji/charts/full-emoji-list.html)
    * ⚠ Il peut arriver que certains emoji ne soient pas tout à fait les mêmes d'un support à l'autre, ni même d'un système d'exploitation à l'autre !
2. **ᔕTYᒪIᔕEᖇ ᒪEᔕ ᑭOᒪIᑕEᔕ ᗩᐯEᑕ ᑌᑎIᑕOᗪE**
    * Unicode dispose également de nombreux caractères alphabétiques alternatifs avec lesquels vous pouvez jongler pour customiser votre texte ! [Ce site](https://coolsymbol.com/text-decoration.html) en référence quelques-uns.
    * ⚠ Certains appareils (surtout les anciens appareils mobiles) peuvent parfois ne pas supporter ces caractères spéciaux. 
## 4. Index
1. README.md
2. jsp
