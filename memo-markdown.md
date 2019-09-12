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
##### Balises de formatage
* **gras** (`<strong>`) ⇒⇒⇒ `**gras**`
* *italique* (`<em>`) ⇒⇒⇒ `*italique*`ou `_italique_`
* __souligné__ (`<u>`) ⇒⇒⇒ `__souligné__` (ne fonctionne pas sur GitHub ¯\_(ツ)_/¯)
* ~~barré~~ (`<strike>`) ⇒⇒⇒ `~~barré~~`
(`<blockquote>`)
* `code` (`<code>`) ⇒⇒⇒ ``­`code`­``
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

On peut aussi combiner des balises ! ~~***grosmichel***~~ ⇒ `~~***grosmichel***~~`
##### Listes
##### Titres
##### Tableaux
##### Liens et images
## 3. Pour aller plus loin…
Rien à voir avec Markdown, mais en matière de personnalisation de vos textes, Unicode offre tout un tas de possibilités intéressantes !
1. **Ajouter des emoji** 👺
    * Le standard Unicode contient naturellement un bon paquet d'emoji que vous pouvez simplement copier/coller dans vos textes. Une liste exhaustive est disponible à [cette adresse](https://unicode.org/emoji/charts/full-emoji-list.html)
    * ⚠ Il peut arriver que certains emoji ne soient pas tout à fait les mêmes d'un support à l'autre, ni même d'un système d'exploitation à l'autre !
2. **𝕾𝖙𝖞𝖑𝖎𝖘𝖊𝖗 𝖑𝖊𝖘 𝖕𝖔𝖑𝖎𝖈𝖊𝖘 𝖆𝖛𝖊𝖈 𝖀𝖓𝖎𝖈𝖔𝖉𝖊**
