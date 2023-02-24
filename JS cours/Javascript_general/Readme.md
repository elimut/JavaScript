#JavaScript

##Introduction au JS

JavaScript est un langage de programmation du Web. Il a été créé en 1995. Avec les comportements dynamiques qu’il introduit, comme les boîtes de dialogue qui s’affichent à
l’écran, les formulaires interactifs ou encore les changements d’image au survol de la souris, le
succès de JavaScript est immédiat. Depuis, le JavaScript fait l’objet de nombreuses évolutions et
la dernière version a été officialisée en 2016 et constitue la septième édition du standard ECMA.
Son objectif est de dynamiser les pages Web et de les rendre interactives. Exemple un
slider, grâce à JavaScript, nous pouvons réaliser un défilement automatique des images. Avec JS,
toute la page (ou le **DOM**) est manipulable et suite à des évènements créés par l’utilisateur, il est
possible de modifier le code HTML et CSS.
>Le DOM (Document Object Model) est une API qui représente et interagit avec tous types de documents HTML ou XML. Le DOM est un modèle de document chargé dans le navigateur. La représentation du document est un arbre nodal. Chaque nœud représente une partie du document (par exemple, un élément, une chaîne de caractères ou un commentaire).

>Le terme DOM est, au contraire du BOM, un terme standardisé et donc défini de manière officielle. Le DOM est une interface de programmation pour des documents HTML ou XML qui représente le document (la page web actuelle) sous une forme qui permet aux langages de script comme le JavaScript d’y accéder et d’en manipuler le contenu et les styles.
Le DOM est ainsi une représentation structurée du document sous forme « d’arbre » crée automatiquement par le navigateur. Chaque branche de cet arbre se termine par ce qu’on appelle un nœud qui va contenir des objets. On va finalement pouvoir utiliser ces objets, leurs propriétés et leurs méthodes en JavaScript.
Le DOM contient ou correspond à un ensemble d’APIs qui font partie du BOM comme l’interface Document par exemple qui représente une page et sert de point d’entrée dans l’arborescence du DOM.
Pour utiliser les propriétés et méthodes de l’interface Document, nous allons tout simplement utiliser la propriété document de Window. Nous avons déjà utilisée cette propriété de nombreuses fois dans ce cours, notamment lorsqu’on souhaitait injecter du texte dans un paragraphe avec le code document.getElementById('#').innerHTML.
Lorsqu’on demande à un navigateur d’afficher une page Web, celui-ci va automatiquement créer un modèle objet de la page ou du document. Ce modèle objet correspond à une autre représentation de la page sous forme d’arborescence contenant des objets qui sont de type Node (nœuds).

Tous les navigateurs sur le marché sont capables d’exécuter JavaScript mais attention, ils
n’ont pas tous le même moteur. C’est pourquoi il est important de tester son programme sur les
principaux navigateurs.
Pour le moment, vous avez appris à taper des lignes de HTML et de CSS, ce sont des
langages de description, c'est-à-dire que vous décrivez, par le biais de ces langages, ce que vous
voulez voir apparaître dans le navigateur… et le navigateur vous suit…
Le JavaScript est quand à lui un langage de programmation impératifs, c'est-à-dire qu’il
donne des ordres au navigateur :
• Affiche ceci !
• Passe à l’image suivante
• Si l’utilisateur clique là, alors tu fais ça !!
• ….
Ces ordres vont constituer un programme qui est en fait une liste d’instructions qui vont
être lues et interprétées par un navigateur.

Permet la création de page interactive et vivante à l'aide de **scripts**.
Script = suite d'instructions qui vont être interprétées par un programme
Pour lire le JS il faut un **interpréteur**, tous les nav en possèdent.
Langage de prog majoritairement **client-side**
>>client side: exécuté du côté de l'ordi de la personne qui demande la page (server-side=exécuté côté serveur(ordi puissant qui stocke les pages et l'envoie quand elles sont demandés par le client).
Client intéragit très rarement avec le server-side(php par exemple, traitement des données en arrière plan).
Client demande page stockée sur serveur,le serveur reçoit demande, le langage server-side est exécuté côté serveur, des calculs sont fait..., une fois exécutation terminée serveur envoie la page qui ne contient que du langage client-side dont JS.Exécution client-side se fait lorsque l'on reçoit la page.
(node.JS projet pour avoir JS côté serveur?)

**Langage orienté objet à prototype**= JS va utiliser des objets dans son fonctionnement global et ces objets sont prototypés.
Objet= bloc cohérent de code qui sert à effectuer telle ou telle opération.

Js utilisé pour manipuler dynamiquement le code HTML d'un page.
>>Attention différence JAVA et JS, concepts totalement différents, tâches différentes.

##L'environnement de travail

Pour coder en JS:

- Editeur de texte(VS,Komodo?,notepad++...)
- Sites pour tester

##Ou écrire le code JS

- Dans élément head d'une page HTML
- Dans élément body ""
- Dans un fichier séparé, portant extension .js (surtout gros projet)

###Dans head:

Placer un élément script à la fin de head.

    <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script>
        alert("Ceci est affiché en JavaScript");
        // boite de dialogue
    </script>
    <title>JavaScript</title>
    </head>

    ###Dans body:

    <body>
    <script>
        alert("Ceci est affiché en JavaScript");
        // boite de dialogue
    </script>
    </body>


>>**Quand écrit dans fichier Html,on peut utiliser autant de script que nécessaire dans head,body, ou les deux, mais par souci de clarté et performance, on le place dans un même élément.
Ceci seront lu linéairement (ordre d'écriture)**.

###Dans fichier séparé:

Avec **extension.js**
Meilleure maintenabilité du code grâce à la séparation des langages, réutilisation du code dans plusieurs fichiers Html.

Il faudra lier les fichiers html et js:
**on utilise la balise script avec son attribut "src" (chemin relatif du fichier js par rapport au fichier html)**.(:/si dossier parent)

    <script src=""></script>
Placé en fin de l'élément body de préférence (permet de charger la page html avant lancement du script).

Méthode de préférence.

##Syntaxes générales et commentaires

**Chaque instruction doit être terminée par un ";"**.

- Texte entre guillemets: "" ou ''
- Chiffres: rien
- Chiffres décimaux: pas de virgule, mais "."(5.40)

ex:
    alert("Une deuxième instruction js");
    alert(5);

**Indentation** : pour plus de clarté
Quand : hiérarchie?
nouvelle indentation à l'intérieure, si instruction en contient sinon même indentation.

Les commentaires en JS:
Il existe des commentaires monoligne et des commentaires multilignes.
On peut utiliser la syntaxe des commentaires multi pour les mono.
**// -> mono
/* début et */ fin -> multi (on peut rajouter une étoile sur les lignes du milieu).**

###Les variables 

####Déclaration

Pour déclarer une variable on utilise la syntaxe : **var ou let**.
var ancienne syntaxe
let nouvelle, à privilégier.

Le nom d'une variable:
- doit commencer par une lettre
- doit contenir uniquement des lettres, _,chiffres
- aucun espace
- est sensible à la casse (Se dit de tout programme qui fait une distinction entre les lettres majuscules et les lettres minuscules, et qui ne traite donc pas de la même façon les données ou les commandes selon qu'elles sont entrées en majuscules ou en minuscules.).

exemple, la variable prénom est déclarée ainsi: 
    let prenom;

####Initialisation

Initialiser= assigner une valeur pour la première fois.
On utilise le signe **=**.

Elle peut se faire:
- en même temps que la déclaration
- après la déclaration
- on peut déclarer plusieurs variables sur une ligne en les séparant par une virgule.

Exemples:

    let prenom = "paul;
Initialisation en même temps que déclaration.

    let nom;
    nom = "paul;
Déclaration puis initialisation.

    let titre = "chat", production = "universal", annee = 2013;
Déclaration de plusieurs variables sur une même ligne.

####Remontée ou hoisting des variables

Une variable déclarée avec var peut-être manipulée en haut de code et être déclarée en fin de code car le JS va traiter les déclarations avant le reste du code JS.Ce comportement est appelé **remontée ou hoisting**, il est dorénavant jugé inadapté.
Avec let, il faut déclarer la variable avant de l'utiliser.

exemples:
    prenom = "paul";
    var = prenom;
Initialisation suivi de déclaration avec var, ok.
Avec let ne fontionne pas!

####La redéclaration de variable

Avec var, il est possible de redéclarer, plusieurs fois, la même variable pour modifier sa valeur.
Avec let, on ne déclare qu'une seule fois.Pour changer sa valeur, il faut lui affecter une autre valeur.

Exemples:

    var prenom= "paul";
    var prenom= "julien";

    let prenom= "david";
    prenom= "nicolas";

####Constante

Pour créer ou déclarer une cosntante en JS, il faut utiliser le mot clef : **const**.
On la déclare de la même façon que let.
**Il faut obligatoirement l' initialiser lors de sa déclaration sinon une erreur sera retournée.**













