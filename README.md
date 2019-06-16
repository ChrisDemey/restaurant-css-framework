# Site web pour un restaurant (fictif)
Voici le lien vers mon site: [Le Sanglier Faisandé](https://chrisdemey.github.io/restaurant-css-framework/)

---
---

## Objectif
<p>Avec <span style="color:purple">**Bootstrap**</span>, réaliser uns site web pour un restaurant (inventé par mes soins) dans lequel je dois inclure plusieurs pages qui elles-mêmes devront contenir des éléments imposés:</p>

* **Page d'accueil**:
	* Un jumbotron.
	* 2 panels (pour afficher des news)
* **Menus**:
	* Des listes groupées (avec des badges).
* **Photos**:
	* Une pagination de minimum 4 pages (3photos par pages).
* **Restaurants**:
	* Adresse, plan d'accès et heures d'ouverture d’au moins deux autres restaurants de la même franchise.
* **Contacts**:
	* Un formulaire contenant le nom, prénom et e-mail du client. Ainsi qu'une liste déroulante, un champ de texte, et un bouton d'envoi.

---

## Le design

<p>Tout d'abord j'avais dans l'idée de partir sur quelque chose de très simple. M'est alors venu l'idée d'avoir un header qui serait présent sur chaque pages avec dedans le nom du restaurant avec de chaque côtés une image de sanglier.</p>
<p>Concernant le thème je suis parti sur des couleurs assez "neutre", rien de flashant.<br>Mais aussi avoir toujours une image de fond qui restera fixe.En partant de ce postulat il m'est très vite venu en tête d'avoir un thème forestier.
<p>Après quelques ébauches sur papier, c'est donc parti pour coder tout ça!</p>

## Le HTML

<p>Alors pour cette partie, on aura forcément beaucoup de div... (MERCI BOOTSTRAP!!!), mais ce n'est pas vraiment un problème, il "suffit juste" de s'organiser.<br>
Mais pas besoin de vous montrer tout mon code ici, ce serait trop longs à montrer et à expliquer. Ceux qui connaissent bien Bootstrap devraient comprendre.</p>

## Le CSS (mais surtout le SASS!)

<p>Pour mes fichiers <span style="color:blue">CSS</span>, j'ai créé des fichiers <span style="color:red">SCSS</span> qui leurs sont respectivement liés afin de mieux organiser la mise en page.</p>
<p>Comme expliqué plus haut dans la partie design, j'ai commencé par le header avec le nom au milieu, bien centré, puis une image de sanglier de chaque côtés.<br>
Ensuite je me suis occupé du fond du site, y mettre une image assez neutre mais qui représenterait bien le thème du site.</p>
<p>Pour tout les éléments de chaque pages je me suis basé sur le style Metro, qui a été beaucoup utilisé avec Windows 8.1 (paix à son âme) et qui utilise des tiles (tuiles).<br>
Excepté qu'a chaque tuiles j'ai mis une image de fond histoire de donner plus de personnalités à mon site.</p>

---

## Des difficultés?

<p>Oh que oui j'en ai rencontré...<br>
La première étant d'organiser mes dossiers afin que chaque fichiers <span style="color:red">SCSS</span>, <span style="color:blue">CSS</span>, et <span style="color:orange">HTML</span> soient bien liés et qu'ils soient facile d'accès.</p>
La seconde difficulté fut de comprendre <span style="color:purple">Bootstrap</span> avec son système de 12 colonnes dans un _row_, puis les équivalents des _media queries_ avec les _col-md_, _offset_, etc... .<br>
<p>Mais la plus grosses difficulté (ou encore celle qui m'a le plus pris la tête dirons-nous) ce sont les listes groupées dans la page des **Menus**.<br>
Mon problème étant que lorsque j'ai mis une image de fond, elle ne s'affichait pas. Mais comme dans beaucoup de situations, la solution était simple, mais il fallait quand même bien regarder.<br>En fait l'image de fond s'affichait bien. Mais les éléments de la liste ont eux-mêmes une couleur de fond. Donc la solution s'est présentée comme étant clair! Dans mon <span style="color:blue">CSS</span> j'ai pris les div des éléments de la liste groupée et je leurs ai attribués ceci: "```background: transparent ```"
<p>Hors mis tout ça, les reste du site n'était pas aussi compliqué à mettre en place.</p>

---

## Mes futurs améliorations

* Ajouter un **footer** sur toutes les pages.
* Ajouter un **zoom** aux photos lorsqu'on clique dessus (page photos, merci Captain Obvious!).
* Peaufiner un maximum la **responsive** sur smartphone (notamment pour le header)
