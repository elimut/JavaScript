# JavaScript

## Introduction au JS

JavaScript est un langage de programmation du Web. Il a été créé en 1995. Avec les comportements dynamiques qu’il introduit, comme les boîtes de dialogue qui s’affichent à l’écran, les formulaires interactifs ou encore les changements d’image au survol de la souris, lesuccès de JavaScript est immédiat. Depuis, le JavaScript fait l’objet de nombreuses évolutions et la dernière version a été officialisée en 2016 et constitue la septième édition du standard ECMA (ECMAScript est un ensemble de normes concernant les langages de programmation de type script et standardisées par Ecma International dans le cadre de la spécification ECMA-262).
On dit que le HTML, le CSS et le JavaScript sont des standards du web car les principaux
navigateurs web (Google Chrome, Safari, Firefox, etc.) savent tous « lire » (ou «
comprendre » ou « interpréter ») ces langages et les interprètent généralement de la
même façon ce qui signifie qu’un même code va généralement produire le même résultat
dans chaque navigateur.
Son objectif est de dynamiser les pages Web et de les rendre interactives. Exemple un slider, grâce à JavaScript, nous pouvons réaliser un défilement automatique des images. Avec JS,toute la page (ou le **DOM**) est manipulable et suite à des évènements créés par l’utilisateur, il est possible de modifier le code HTML et CSS.
>Le DOM (Document Object Model) est une API.(Une API (Application Programming Interface) est un ensemble de fonctionnalités et de règles existant dans un logiciel permettant d'intéragir avec celui-ci de manière automatisée (plutôt que de passer par une interface utilisateur). L'API peut être vue comme un contrat simple passé entre le logiciel qui la propose et d'autres entités, telles que des logiciels ou matériels tiers. qui représente et interagit avec tous types de documents HTML ou XML. Le DOM est un modèle de document chargé dans le navigateur. La représentation du document est un arbre nodal. Chaque nœud représente une partie du document (par exemple, un élément, une chaîne de caractères ou un commentaire).Voir chapitre DOM.

>Le terme DOM est, au contraire du BOM, un terme standardisé et donc défini de manière officielle. Le DOM est une interface de programmation pour des documents HTML ou XML qui représente le document (la page web actuelle) sous une forme qui permet aux langages de script comme le JavaScript d’y accéder et d’en manipuler le contenu et les styles.
Le DOM est ainsi une représentation structurée du document sous forme « d’arbre » crée automatiquement par le navigateur. Chaque branche de cet arbre se termine par ce qu’on appelle un nœud qui va contenir des objets. On va finalement pouvoir utiliser ces objets, leurs propriétés et leurs méthodes en JavaScript.
Le DOM contient ou correspond à un ensemble d’APIs qui font partie du BOM comme l’interface Document par exemple qui représente une page et sert de point d’entrée dans l’arborescence du DOM.
Pour utiliser les propriétés et méthodes de l’interface.Le terme interface est généralement utilisé en informatique pour désigner un programme permettant un échange de données : Il peut s'agir d'un échange entre deux logiciels : l'interface est, par exemple, un programme qui reformate les données pour assurer la compatibilité entre ces deux logiciels.) Document, nous allons tout simplement utiliser la propriété document de Window. Nous avons déjà utilisée cette propriété de nombreuses fois dans ce cours, notamment lorsqu’on souhaitait injecter du texte dans un paragraphe avec le code document.                       getElementById('#').innerHTML.
Lorsqu’on demande à un navigateur d’afficher une page Web, celui-ci va automatiquement créer un modèle objet de la page ou du document. Ce modèle objet correspond à une autre représentation de la page sous forme d’arborescence contenant des objets qui sont de type Node (nœuds).
![DOM](img/interpretation.png)

Tous les navigateurs sur le marché sont capables d’exécuter JavaScript mais attention, ils
n’ont pas tous le même moteur. C’est pourquoi il est important de tester son programme sur les
principaux navigateurs.
Pour le moment, vous avez appris à taper des lignes de HTML et de CSS, ce sont des
langages de description, c'est-à-dire que vous décrivez, par le biais de ces langages, ce que vous
voulez voir apparaître dans le navigateur… et le navigateur vous suit…
Le JavaScript est quand à lui un **langage de programmation impératif**, c'est-à-dire qu’il
donne des ordres au navigateur :
• Affiche ceci !
• Passe à l’image suivante
• Si l’utilisateur clique là, alors tu fais ça !!
Ces ordres vont constituer un programme qui est en fait une liste d’instructions qui vont
être lues et interprétées par un navigateur = **scripts**.
Script = suite d'instructions qui vont être interprétées par un programme.
Pour lire le JS il faut un **interpréteur**, tous les nav en possèdent.
On peut encore séparer les langages selon qu’ils puissent être exécutés directement (on
parlera alors de langages interprétés) ou qu’il faille les transformer en une autre forme
pour pouvoir les exécuter (on parlera alors le langages compilés).
Le JavaScript est un langage interprété. Cela signifie qu’il va pouvoir être exécuté
directement sous réserve qu’on possède le logiciel interpréteur. Pas de panique ici : tous
les navigateurs connus possèdent leur interpréteur JavaScript.
>JavaScript est un langage de programmation de script largement utilisé pour animer les sites web.
Un langage de script est un langage interprété.
Sa syntaxe est dite de haut niveau, plus proche du langage naturel que du langage machine : par conséquent, il est relativement simple à apprendre et est indépendant de l'aspect matériel de la machine sur lequel il est lancé.
Langage interprété:
Un langage interprété est un langage qui est exécuté par un autre programme : l'interpréteur.
Celui-ci lit une ligne de code, l'analyse, l'exécute si elle est correcte et passe à la suivante ; il répète ce processus pour chaque instruction du programme. Un programme en langage interprété est donc exécuté au fur et à mesure de sa lecture.
![interpréteur](img/interpretation.png)

Langage de programation majoritairement **client-side**
La catégorisation langages statiques / langage dynamique est une première façon de
classer les différents langages de programmation.
On peut également classer les différents langages selon l’endroit où ils vont s’exécuter :
soit côté client, soit côté serveur.
Pour comprendre ce que sont les langages « côté client » et « côté serveur », il convient
avant tout de comprendre ce qu’est un client et ce qu’est un serveur et pour cela il faut
savoir ce qu’est un site.
Un site est un ensemble de ressources et de fichiers liés entre eux. Pour que notre site
soit accessible sur le web pour tous, on va l’héberger sur un serveur, c’est-à-dire envoyer
l’ensemble de nos fichiers sur le serveur et on va également acheter un nom de domaine
qui va servir à identifier notre site.
Un « serveur » est une sorte de super ordinateur, constamment accessible et connectés
aux autres serveurs (formant ainsi un réseau qu’on appelle le web) et qui va héberger les
fichiers constituant un (ou plusieurs) site(s) web et le(s) « servir » sur demande du client.
Lorsqu’on demande à accéder à une page web en tapant une URL dans notre navigateur,
nous sommes le client ou plus exactement notre navigateur est le logiciel client qui
effectue une demande ou « requête » au serveur qui est la suivante : « sers-moi le fichier
correspondant à l’adresse que je t’ai envoyée ».
Les fichiers ou pages d’un site web vont pouvoir être constituées de deux types de codes
différents : du code côté serveur et du code côté client. Lorsqu’on demande à un serveur
de nous servir une page, celui-ci se charge d’exécuter le code côté client s’il y en a et ne
va renvoyer que du code côté client en résultat.
Un langage « côté client » ou « client side » est un langage qui va être exécuté dans le
navigateur des utilisateurs qui demandent la page. On peut également appeler ces
langages des langages « web » puisqu’ils sont principalement utilisés dans un contexte
web.
Il existe aujourd’hui 3 langages côté client incontournables qui sont le HTML, le CSS et le
JavaScript.
Les langages côté serveur sont des langages qui vont s’exécuter sur le serveur. Les
navigateurs ne sont dans la grande majorité des cas pas capables de comprendre les
langages serveur.
Ces langages permettent notamment d’effectuer de manipuler les données pour renvoyer
des résultats. Les résultats renvoyés le sont sous forme de code compréhensible par le
navigateur (c’est-à-dire du HTML principalement) pour que le navigateur puisse afficher le
résultat final.
La chose importante à retenir ici est que le JavaScript est un langage principalement utilisé
côté client, mais qui va également pouvoir s’utiliser côté serveur à condition qu’on mette
en place un environnement favorable (en utilisant Node.js par exemple).


**Langage orienté objet à prototype**= JS va utiliser des objets dans son fonctionnement global et ces objets sont prototypés.
Objet= bloc cohérent de code qui sert à effectuer telle ou telle opération.

Js utilisé pour manipuler dynamiquement le code HTML d'un page.
>Attention différence JAVA et JS, concepts totalement différents, tâches différentes.
Retenez ici que ces deux langages, bien que syntaxiquement assez proches à la base,
reposent sur des concepts fondamentaux complètement différents et servent à effectuer
des tâches totalement différentes.
Pourquoi des noms aussi proches ? Java est une technologie créée originellement par
Sun Microsystems tandis que JavaScript est un langage créé par la société Netscape.
Avant sa sortie officielle, le nom original du JavaScript était « LiveScript ». Quelques jours
avant la sortie du LiveScript, le langage est renommé JavaScript.
A l’époque, Sun et Netscape étaient partenaires et le Java était de plus en plus populaire.
Il est donc communément admis que le nom « JavaScript » a été choisi pour des raisons
marketing et pour créer une association dans la tête des gens avec le Java afin que les
deux langages se servent mutuellement.
Le créateur du JavaScript a également expliqué que l’idée de base derrière le
développement du JavaScript était d’en faire un langage complémentaire au Java.

On oppose généralement les langages « dynamiques » aux langages « statiques » comme
le HTML et le CSS. Illustrons les différences d’utilisation entre ces types de langage en
discutant des possibilités du HTML, du CSS et du JavaScript.
Pour rappel, le HTML est un langage de balisage (langage qui utilise des balises) qui est
utilisé pour structurer et donner du sens aux différents contenus d’une page. Le HTML
nous permet de communiquer avec un navigateur en lui indiquant que tel contenu est un
titre, tel contenu est un simple paragraphe, tel autre est une liste, une image, etc.
Le navigateur comprend les différentes balises HTML et va alors afficher notre page à nos
visiteurs en tenant compte de celles-ci.

### JavaScript, API, librairies et framework

Le JavaScript en tant que langage correspond à un ensemble de structures de codes ou
un ensemble d’éléments qu’on va pouvoir utiliser pour implémenter des fonctionnalités sur
nos pages web.
Les API et les librairies JavaScript sont construites à partir de ces éléments de base du
JavaScript et vont nous permettre d’utiliser des structures plus complexes déjà prêtes à
l’emploi qui vont in-fine nous permettre de réaliser simplement des opérations qu’il aurait
été très difficile de réaliser si on avait dû les coder entièrement à la main.
Une API (« Application Programming Interface » ou « Interface de Programmation ») est
une interface qui nous permet d’utiliser facilement une application. Une application est un
programme, c’est-à-dire un ensemble cohérent de code qui permet de réaliser certaines
actions.
On utilise les API pour demander au programme d’effectuer certaines actions pour nous,
comme par exemple afficher une carte d’une certaine ville à une certaine échelle (Google
Maps API) ou pour afficher la liste de nos derniers Tweets (Twitter API) ou encore pour
manipuler le contenu HTML d’une page web (DOM API).
Pour utiliser une API et donc l’application correspondante, il faudra généralement
demander au propriétaire de l’application une clef qui va nous permettre de nous identifier.
Une librairie ou « bibliothèque » JavaScript est un ensemble de fichiers de code JavaScript
homogènes (= qui se concentrent sur un aspect particulier du langage) qu’on va devoir
télécharger pour les utiliser. Ces fichiers de code contiennent des structures de code
prêtes à l’emploi qu’on va pouvoir utiliser immédiatement pour gagner du temps en
développement. Parmi les librairies les plus célèbres, on peut notamment citer jQuery.
Il convient donc de ne pas confondre API et librairies : une librairie est un ensemble de
fichiers qu’on va télécharger et contient un ensemble de structures de codes prêtes à
l’emploi. Nous allons pouvoir choisir celles qui nous intéressent pour les intégrer dans nos
propres scripts et ainsi gagner du temps de développement. Une API, de l’autre côté, va
nous permettre d’utiliser une application qu’on n’a pas le droit de manipuler directement.
Finalement, un framework ou « cadre de travail » est relativement similaire dans son but
à une « super librairie ». Les framework vont également nous fournir un ensemble de
codes tout prêts pour nous faire gagner du temps en développement. La grande différence
entre un framework et une librairie réside dans la notion d’inversion du contrôle : lorsqu’on
télécharge une librairie, on peut l’utiliser comme on le souhaite en intégrant ses éléments
à nos scripts tandis que pour utiliser un framework il faut respecter son cadre (ses règles).
Les framework JavaScript les plus connus aujourd’hui sont Angular.js et React.js.
Dans le début de ce cours, nous n’utiliserons bien évidemment pas d’API ni de librairie et
encore moins de framework. Cependant, il reste intéressant de déjà définir ces différents
termes pour vous donner une première « vue d’ensemble » des outils JavaScript.

## L'environnement de travail

Pour coder en JS:

- Editeur de texte(VS,Komodo?,notepad++...)
- Sites pour tester.
  
### Les librairies JavaScript à télécharger

Pour coder en JavaScript, un simple éditeur de texte suffit en théorie. Cependant, pour
exploiter toute la puissance du JavaScript et pour gagner du temps de développement,
nous utiliserons régulièrement des librairies JavaScript en plus du JavaScript « vanilla »
(JavaScript « pur »).
Pour qu’une librairie JavaScript fonctionne, il va falloir que le navigateur des personnes
qui affichent la page la connaisse. Pour cela, on « forcera » le navigateur de nos visiteurs
à télécharger les librairies qu’on utilise dans nos pages.
Pour le début de ce cours, cependant, nous n’utiliserons pas de librairie car je veux que
vous compreniez bien comment fonctionne le JavaScript et que vous appreniez à résoudre
différents problèmes avec du **JavaScript vanilla**. Je pense que c’est en effet une grosse
erreur d’essayer de contourner certaines difficultés en JavaScript en utilisant des librairies
lorsqu’on ne maitrise pas suffisamment le JavaScript classique. 

## Ou écrire le code JS

- Dans élément head d'une page HTML,
- Dans élément body "",
- Dans un fichier séparé, portant extension .js (surtout gros projet),
- Directement dans la balise ouvrante d’un élément HTML,
- Dans un élément script, au sein d’une page HTML.


### Dans head:

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

## Dans body:

Dans une balise script:

    <body>
    <script>
        alert("Ceci est affiché en JavaScript");
        // boite de dialogue
    </script>
    </body>

Dans une balise ouvrante:

    <button onclick="alert("Bonjour!")>
    ->Ici, on crée deux boutons en HTML et on place nos codes JavaScript à l’intérieur
    d’attributs onclick. Le code placé en valeur des attributs va s’exécuter dès qu’on va cliquer
sur le bouton correspondant.
>**Quand écrit dans fichier Html,on peut utiliser autant de script que nécessaire dans head,body, ou les deux, mais par souci de clarté et performance, on le place dans un même élément.
Ceci seront lu linéairement (ordre d'écriture)**.

### Dans fichier séparé:

Avec **extension.js**
Meilleure maintenabilité du code grâce à la séparation des langages, réutilisation du code dans plusieurs fichiers Html.

Il faudra lier les fichiers html et js:
**on utilise la balise script avec son attribut "src" (chemin relatif du fichier js par rapport au fichier html)**(:/si dossier parent).Cette balise sera vide.

    <script src=""></script>
Placé en fin de l'élément body de préférence (permet de charger la page html avant lancement du script).

Méthode de préférence.

## La place du code et l’ordre d’exécution de celui-ci

Il y a un factuer très important lorsque l'on ajoute du JS dans les pages HTML: l'ordre d' exécution du code par le navigateur.
**Un navigateur va lire
et exécuter le code dans l’ordre de son écriture**.
Plus précisément, lorsque le navigateur arrive à un élément script, il va stopper le
traitement du reste du HTML jusqu’à ce que le code JavaScript soit chargé dans la page
et exécuté.
Nos codes JavaScript ci-dessus ont besoin des éléments button de notre page HTML pour
fonctionner. En effet, les codes getElementById('b1') et getElementById('b2') vont
récupérer les éléments dont les id sont « b1 » et « b2 » pour les manipuler.
Cela risque de poser problème dans le cas présent car si notre code JavaScript est
exécuté avant que le code HTML de nos boutons ne soit traité par le navigateur, il ne
fonctionnera puisqu’il cherchera à utiliser des éléments qui n’existent pas encore.
C’est la raison pour laquelle, lorsque j’ai choisi d’insérer le code JavaScript directement
dans la page HTML au sein d’éléments script, j’ai été obligé d’entourer le code JavaScript
qui affiche la boite d’alerte déclaré dans l’élément head par le
code document.addEventListener('DOMContentLoaded', function(){}) ;. Ce code indique
en effet au navigateur qu’il doit d’abord charger tout le contenu HTML avant d’exécuter le
JavaScript à l’intérieur de celui-ci.
Dans ce même exemple, mon deuxième élément script était lui placé en fin de body et est
donc par défaut exécuté après le reste du code. Il n’y avait donc pas de problème dans ce
cas.
Notez que le même problème va avoir lieu dans le cas où on fait appel à un fichier
JavaScript externe par défaut : selon l’endroit dans le code où le fichier est demandé, il
pourra ne pas fonctionner s’il utilise du code HTML pas encore défini.
**Ce souci est la raison pour laquelle il a longtemps été recommandé de placer ses
éléments script juste avant la balise fermante de l’élément body, après tout code HTML.
Cette façon de faire semble en effet résoudre le problème à priori mais n’est pas toujours
optimale en termes de performances.**
En effet résumons ce qu’il se passe dans ce cas :
1. Le navigateur commence à analyser (ou à traiter) le code HTML ;
2. L’analyseur du navigateur rencontre un élément script ;
3. Le contenu JavaScript est demandé et téléchargé (dans le cas où il se situe dans
un fichier externe) puis exécuté. Durant tout ce temps, l’analyseur bloque l’affichage du HTML, ce qui peut dans le cas où le script est long ralentir significativement le temps d’affichage de la page ;
4. Dès que le JavaScript a été exécuté, le contenu HTML finit d’être analysé et est
affiché.
Ce problème précis de temps d’attente de chargement des fichiers JavaScript va pouvoir
être résolu en grande partie grâce au téléchargement asynchrone des données qui va
pouvoir être ordonné en précisant un attribut **async ou defer** dans nos éléments script.
Le téléchargement asynchrone est une notion complexe et nous l’étudierons donc
beaucoup plus tard dans ce cours. Pour le moment, retenez simplement que nous n’allons
pouvoir utiliser les attributs async et defer que dans le cas où on fait appel à des fichiers
JavaScript externes (c’est-à-dire à du code JavaScript stocké dans des fichiers séparés).
C’est une raison supplémentaire qui nous fera préférer l’enregistrement du code
JavaScript dans des fichiers séparés.

    <script src=".js" async ou defer></script> 
    -> dans head.

## Commentaires, indentation et syntaxe de base

### Généralités:

#### Afficher des informations:
- alert("Une deuxième instruction js"); boîte de dialogue (pop-up).
- document.write("hello"); Affiche une information directement sur notre page, dans le navigateur à l’endroit où le lien vers
le fichier script est fait.
- console.log("hello"); Affiche info dans la console (F12),affiche les erreurs, vérification du contenu d'une variable.

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

####Les commentaires en JS:
Il existe des commentaires monoligne et des commentaires multilignes.
On peut utiliser la syntaxe des commentaires multi pour les mono.
**// -> mono
/ * début et * / fin -> multi (on peut rajouter une étoile sur les lignes du milieu).**

##Gestion des données

###Les variables:

![schéma](img/variables_schéma.png)

Sorte de petite boîte qui possède un nom et contient une valeur.
Comme son nom l'indique peut changer de valeur à tout moment.
Stocke différentes valeurs dans le temps, en écrasant les précédentes.
Doit être déclarée une et une seule fois dans un programme.
Il existe deux types de variables:
- **Globales**: utilisées dans tout le programme, déclarées à la base du code, en dehors de toute fonction.
- **Locales**: qui ne servent que pour un programme ou fonction particuliers, déclarées au sein de ce programme ou cette fonction.

####Déclaration: 

Pour déclarer une variable, on utilise la syntaxe : **var ou let**.
- var ancienne syntaxe,
- let nouvelle, à privilégier.

Règle de nommage (valable pour les fonctions)= **CamelCase** :

- Nom unique = **identifier**,
- Aucune ponctuation,accents,espace, 
- Mise en capitale de la première lettre des mots, sauf le premier,
- Doit commencer par une lettre,
- Doit contenir uniquement des lettres, _,chiffres,
- Aucun espace
- Est sensible à la casse (Se dit de tout programme qui fait une distinction entre les lettres majuscules et les lettres minuscules, et qui ne traite donc pas de la même façon les données ou les commandes selon qu'elles sont entrées en majuscules ou en minuscules).

Exemple: la variable prénom est déclarée ainsi: 

    let prenom;

Exemple :

    let ma PremiereVariable = "Bonjour";
    console.log(maPremiereVariable);
    

####Initialisation:

Initialiser = assigner une valeur pour la première fois.
On utilise le signe **=**. = est un **opérateur d' affectation** et non d' égalité, assigne voire affecte une valeur à une variable.Permet de stocker une valeur dans une variable.

Elle peut se faire:
- en même temps que la déclaration
- après la déclaration
- on peut déclarer plusieurs variables sur une ligne en les séparant par une virgule.

Exemples:

    let prenom = "paul;
->Initialisation en même temps que déclaration.

    let nom;
    nom = "paul;
->Déclaration puis initialisation.

    let titre = "chat", production = "universal", annee = 2013;
->Déclaration de plusieurs variables sur une même ligne.

####Remontée ou hoisting des variables/ 

Une variable déclarée avec var peut-être manipulée en haut de code et être déclarée en fin de code car le JS va traiter les déclarations avant le reste du code JS.Ce comportement est appelé **remontée ou hoisting**, il est dorénavant jugé inadapté.
Avec let, il faut déclarer la variable avant de l'utiliser.

Exemples:

    prenom = "paul";
    var = prenom;
->Initialisation suivi de déclaration avec var, ok.
Avec let ne fontionne pas!

    var x = 25;
    var x = 100;
->déclaration et initialisation 

var prenom = "pierre", nom = "gireaud", dpt = 83;
->déclaration plusieurs variables sur une même ligne

    var nom;
    nom = 25;
    ->déclaration sans valeur, puis initialisation (à éviter): var nom = ""; préférable affection valeur nulle à une variable.

####La redéclaration de variable:

Avec var, il est possible de redéclarer, plusieurs fois, la même variable pour modifier sa valeur.
Avec let, on ne déclare qu'une seule fois.Pour changer sa valeur, il faut lui affecter une autre valeur (La nouvelle valeur écrase la précédente).
**Il est possible de réaffecter une valeur de type différent dans une variable.**

Exemples:

    var prenom = "paul";
    var prenom = "julien";

    let prenom = "david";
    prenom = "nicolas";

    let x = 5;
    x = x + 5;
    ->On stocke dans x la valeur 5, puis dans x l'ancienne valeur de x + 5.Donc x stocke 10.

    let x = 4;
    x = "quatre";

###Constante:

Pour créer ou déclarer une cosntante en JS, il faut utiliser le mot clef : **const**.
On la déclare de la même façon que let.
**Il faut obligatoirement l' initialiser lors de sa déclaration sinon une erreur sera retournée.**
**Valeur inchangeable**.

Exemple:

    const x = 5;

##Les types:

###Quelles valeurs peuvent prendre mes variables?

Les types de valeurs contenues dans les variables en JS.Elles peuvent stocker différents types de valeur.
On ne stocke pas de la même façon un nombre ou une chaîne de caractères dans une variable, on effectue également pas les mêmes opérations en fonction des valeurs.

- **String** : chaîne de caractères, texte mis entre "" ou '' ou quotes:

        let prenom = "Pierre";
        let hello = "Bonjour, nous sommes...";
  Si l'on utilise les '', dans le cas où la chaîne de caractère contient des ', il faudra échapper avec \:

        let dpt = "Je vis dans le \"83"\";
  Un nombre entouré de "" est considéré comme un string (cela influence les opérations effectuées):

        var d = "65";
- **Number**: entiers, réels, float (attention au point):

        let x = 2.5;
        let y = -75;
        let z = 23;
- **Booléen**: contient deux valeurs true ou false (valeurs de type booléenne).Un booléen est une valeur binaire.
Surtout utilisée pour testes, vérification de condition,...
Pour qu'une variable stocke un booléen, elle doit stocker true ou false, sans "", et sans '':

        let a = true;
- **Tableau**: **array** en JS, il contient plusieurs valeurs classées dans un tableau.
- **Objet**: contient des propriétés et des méthodes.
- **Null**: non connaissance de la valeur.

        let n = null;
- **Undefined**: ne pas avoir défini de valeur pour la variable.
- 
        let u = undefined;
- **NaN**: not a number.

        var nn = NaN;
  
![objet schéma](img/objets_schéma.png)

>**-> JavaScript est conçu autour d'un paradigme simple, basé sur les objets. Un objet est un ensemble de propriétés et une propriété est une association entre un nom (aussi appelé clé) et une valeur. La valeur d'une propriété peut être une fonction, auquel cas la propriété peut être appelée « méthode ». En plus des objets natifs fournis par l'environnement, il est possible de construire ses propres objets. Ce chapitre aborde la manipulation d'objets, l'utilisation des propriétés, fonctions et méthodes, il explique également comment créer ses objets**.

###Tester type de valeur:

On utilise généralement fonction **typeof**.
Attention, renvoie parfois des valeurs contestables.

Exemple:

    alert("Variable x : " + typeof(x) +
    "\nVariable y : " + typeof(y) +
    "\nVariable a : " + typeof(a));
    ->voir main.js détails fonctions et usage.

##Concaténation 

Consiste en l' assemblage de texte et de variable (addition de chaîne de caractères).
On utilise le signe "**+**", utilisé également pour additionner, JS fait la différence en fonction du type de valeurs qui entourent le +.
**S'il s' agit de nombres: addition, s'il s'agit de textes : concatène**.

Exemples:

    let nom = "chat";
    let prenom = "bahamut";
    console.log(nom + prenom);
    ->affichage : chatbahamut
               
                   Attention aux espaces!

    let nom = "chat ";
    ->espace après le nom => affichage : chat bahamut

    let prenom = "anne-so", espace = "", nom = "vand";
    let moi = prenom + espace + nom;
    ->concaténation de variable

    let moi = "anneso" + " " + "paul";
    ->concaténation de valeur

    let sport = "courir";
    let hobby = "j' aime le" + " " + sport;

    alert("Bonjour" + \nsport);

    let x = 4 + 2 + "1"; => 4 et 2 s'additionne puis concaténation avec 1: 61.
    let y = "1" + 2 + 4; => 124.
    let z = 2 + "un" + 4; => 2un4.
    ->distinction + addition et + concaténation.Addition nombre et chaîne de caractère, tout ce qui sera après la chaîne de caractère sera considéré commme une chapine de caractère = > pas d'addition mais concaténation!
    
    alert("variable x :" + typeof(x)); => string.



##Calculs sur variables

Il est possible de faire des calculs sur des variables de type number:

|Opération|Symbole|
|:-------|:------|
|Addition|+|
|Soustraction|-|
|Multiplication|*|
|Division|/|
|Modulo (entier reste division euclidienne)|%|
|Incrémenter var de 1|++|
|Décrementer var de 1|--|
|Incrémenter une var de la valeur d'une seconde var|+=|
|Décrémenter une var de la valeur d'une seconde var|-=|
|Multiplier l'ancienne valeur de la variable| *=|
|Diviser l'ancienne valeur de la variable| /=|
|Modulo l'ancienne valeur de la variable| %=|

Exemples:

    let x = 6;
    let y = 7;
    let addition = x + y;

    let x = 5;
    x = x + 5; (10)
    x = x + 3; (13)

    var mod = 13 % 3;

    var x =2;
    x += 2; => x = x+2;
    x -= 3; => x = x-3;

    y *= x; => y = y*x;
**Attention à bien respecter les priorités de calcul comme en mathématiques!**

##Prompt

**Fonction** qui permet de demander à l' utilisateur une information.
Va ouvrir une boîte de dialogue qui contiendra une question et un champ vide de réponse.

Exemple:

    let age = window.prompt("Quel âge avez-vous?");
Pour stocker la valeur saisie par l'User dans une variable, il faut attribuer ce prompt à une variable.
La valeur saisie sera enregistrée dans la variable age.

**Attention, le prompt, renvoie toujours une chaîne de caractères.Ce qui signifie que pour faire des calculs avec cette variable, il va falloir modifier le type de la variable obtenue avec le prompt**.


##Conversion

Les fonctions **parentInt** et **parseFloat** servent à convertir une chaîne de caractères en nombre entier pour le premier, et à virgule pour le second.

exemple :

    age = parseInt(age);
    age ++;
conversion de la var age en type number, et incrémentation possible.

##Les tableaux : l'objet array

![tableaux](img/tableaux.png)

###Les propriétés

|Propriété|Description|
|:--------|:----------|
|lenght|contient le nombre d' éléments du tableau|
|input|permet de faire une recherche dans le tableau à l'aide d'un expression régulière|
|prototype|permet d' ajouter des propriétés personnalisées à l'objet|

###Les méthodes standards

|Méthode|Description|
|:--------|:----------|
|concat(tab1,tab2[,tab3,...])|permet de concaténer plusieurs tableaux, créer un tableau à partir de plusieurs tableaux|
|tableau.join(",")|renvoie une chaîne de caractères contenant tous les éléments du tableau séparé par le séparateur mis en paramètre : vat tab=newArray("pommes","poires")document.write(tab.join(",")renvoie pommes,poires)|
|tableau.pop()|supprime le dernier élément du tableau et retourne sa valeur|
|tableau.shift()|supprime le premier élément du tableau |
|tableau.push(valeur1,valeur2,...)|ajoute un ou plusieurs éléments  en fin de tableau et retourne la nouvelle taille du tableau|
|tableau.unshift()|supprime le premier élément du tableau|
|tableau.splice(debut,nbr_elements,"new_1","new-2")|Ajoute/retire des éléments d'un tableau en fonction de la position indiqué.Paramètres: **début**L'indice à partir duquel commencer à changer le tableau (l'indice du premier élement étant 0). Si sa valeur est supérieure à la longueur du tableau array.length, début est ramené à la longueur du tableau array.length. S'il est négatif, le changement commencera d'autant d'éléments à partir de la fin du tableau, c'est à dire à partir de l'index array.length + début. Si array.length + début est inférieur à 0, le changement commencera à l'index 0.**nbASupprimer**Un entier indiquant le nombre d'anciens éléments à remplacer. Si ce paramètre est absent ou si sa valeur est supérieure ou égale à array.length - début, alors les éléments entre début et la fin du tableau seront supprimés. Si nbASupprimer vaut 0, aucun élément ne sera supprimé. Dans ce cas, il est nécessaire de spécifier au moins un nouvel élément.**élemN**Les éléments à ajouter au tableau à partir de début. Si vous ne spécifiez pas de nouvel élément, les anciens éléments seront simplement supprimés du tableau.|
|tableau.slice(debut,fin)|Renvoie un tableau contenant une partie extraction) des éléments d'un tableau.Le paramètre fin est exclu|
|Tableau.sort() |trie les éléments d'un tableau.|
|Tableau.includes(valeur recherché,position)|Permet de savoir si un élément se trouve dans un le tableau elle recoit en paramètre l'element recherché et la position dans le tableau a partir de laquelle la recherche commence, elle retourne true ou false.|
|Tableau.toString()|Renvoie la chaîne de caractères correspond à l'instruction qui a permis de créer l'objet Array|
|Tableau.indexOf(valeur,position) |Retourne la position de l'élément mis en paramètre la recherche commence en fonction du deuxième paramètre si ce deuxième paramètre est omis la recherche commence en début de tableau si l'élément n'est pas trouvé elle retourne -1.|
|Tableau.lastIndexOf(valeur,position)|similaire a indexOf la recherche se faisant à partir de la dernière position.|
|Tableau.valueOf |Retourne tout simplement la valeur de l'objet Array auquel elle fait référence.|
|Tableau.reverse()|Inverse l'ordre des éléments du tableau|

Exemples :

    let array3 = ["Javascript", "Php", "Python"];
    let array4 = ["Ruby", "Solidity"];

concat():

    let newArray = array3.concat(array4);

join() :  

    console.log(array3.join(' -> '));
->Javascript -> Php -> Python

    console.log(array3.join(' '));
->Javascript Php Python

.slice():

    console.log(array3.slice(1));
    ["Php", "Python"]
->l’extraction commence à l’index 1 jusqu’au dernier index inclus

    console.log(newArray.slice(1, 4));
->l’extraction commence à l’index 1 et
s’arrete à l’index 4 (index 4 exclu)

.indexOf() et .forEach():

    console.log(array3.indexOf("Python"));
->donne l’index de « python » soit 2

    array3.forEach((languages) => console.log(languages));
->applique un forEach au tableau 3 et renvoi les valeurs de
chaque index

.every() et .some():

    console.log(array3.every((language) => language == "Php"));
->renvoie false car tous les index ne sont pas « php »

    console.log(array3.some((language) => language == "Php"));
->renvoie true car aux moins un index contient « php »

.shift():

    let shift = array3.shift();
->supprime le premier element du tableau

.pop():

    console.log(array3.pop());
->supprime le dernier element du tableau et renvoie sa valeur

.splice():
.splice(index de depart, nb à supprimer, element à ajouter)

    var mesPoissons = ["scalaire", "clown","mandarin","chirurgien"]; 

    var enleves = mesPoissons.splice(2, 0, "tambour");
    // supprime 0 élément à partir de l'index 2, et insère "tambour"
    // mesPoissons est ["scalaire", "clown", "tambour", "mandarin", "chirurgien"]
    // enleves est 0, aucun élément supprimé

    enleves = mesPoissons.splice(3, 1);
    // supprime 1 élément à partir de l'index 3
    // mesPoissons est ["scalaire", "clown", "tambour","chirurgien"]
    // enleves est ["mandarin"]
    
    enleves = mesPoissons.splice(2, 1, "trompette");
    // supprime 1 élément à partir de l'index 2, et insère "trompette"

    enleves = mesPoissons.splice(0, 2, "perroquet", "anémone", "bleu");
    // mesPoissons est ["perroquet", "anémone", "bleu", "trompette", "chirurgien"]
    // enleves est ["scalaire", "clown"]

    enleves = mesPoissons.splice(mesPoissons.length - 3, 2);
    // supprime 2 éléments à partir de l'indice 2
    // mesPoissons est ["perroquet", "anémone","chirurgien"]
    // enleves est ["bleu", "trompette"]

    var mesPoissons = ["perroquet", "anémone", "bleu", "trompette", "chirurgien"];
    enleves = mesPoissons.splice(2);
    // on retire les éléments à partir de l'indice 2
    // mesPoissons vaut ["perroquet", "anémone"]
    // enleves vaut ["bleu", "trompette", "chirurgien"]

    var mesAnimaux = ["cheval", "chien", "chat", "dauphin"];
    enleves = mesAnimaux.splice(-2, 1);
    // mesAnimaux vaut ["cheval", "chien", "dauphin"]
    // enleves vaut ["chat"]

.reduce():
Reduce permet de calculer toutes les valeurs du tableau

   let arrayNumber = [4, 74, 28, 12, 1];
    arrayNumber.reduce((x, y) => x + y);
->donne 119
 
filter():
permet de filtrer les éléments d’un tableau

    let arrayNumber = [4, 74, 28, 12, 1, 17 , 8];
    arrayNumber.filter((number) => number > 10);
->donne (4) [74, 28, 12, 17]

sort():
permet de trier les éléments d’un tableau

    arrayNumber.sort();
sans autre précision la méthode tri selon la dizaine ce qui donne :
->(7) [1, 12, 17, 28, 4, 74, 8]

    arrayNumber.sort((a, b) => a - b);
->en passant deux paramètres a et b et en indiquant a – b , le tri se fera
par ordre croissant
(7) [1, 4, 8, 12, 17, 28, 74]

  arrayNumber.sort((a, b) => b - a);
->en passant deux paramètres a et b et en indiquant b – a , le tri se fera
par ordre décroissant
(7) [74, 28, 17, 12, 8, 4, 1]

##Les objets

![objet](img/objets.png)

Tout comme les tableaux, les objets permettent de stocker beaucoup d'informations dans une seule et même variable.
Mais contrairement aux tableaux, on ne va pas utiliser un index.

###Création d'un objet

Prenons un tableau qui contient les informations concernant une personne:

    const client = ["jean","pierre","0687440005,"vandingenenannesophie@gmail.com"];

Toutes les informations sont enregistrées dans une seule et même variable,mais ça n'est pas clair.

Pour pouvoir donner une étiquette aux données présentes dans une variable, nous allons utiliser un objet:

    const client= {
        prenom : "jean",
        nom : "pierre",
        telephone : "0687440005",
        mail : "vandingenenannesophie@gmail.com
    };
**Un objet s'ouvre avec des accolades, le nom des propriétés sera suivi de  :puis d'une valeur.**

####Ajout d'une propriété à un objet existant:

Ajoutons la ville ->

    const client = {
        prenom:"",
        nom : "",
        telephone : "",
        mail :""
    };
    cleint.ville = "Lille";
**Pour ajouter un champ, une nouvelle instruction, le nom de la variable qui contient l'objet, un "." est égal à une valeur.**

####Modification d'une valeur d'une propriété existante:

**On appelle la clé dont nous souhaitons changer la valeur, puis nous lui affectons une nouvelle valeur.**

    client.telephone = "nvl val";

###Lire un objet

Pour accèder à la valeur d'une des étiquettes, il suffit de faire ceci :

    console.log(client.nom);
nomvar.propriété de la valeur souhaitée.
>console.log() est une méthode de l’objet console en JavaScript qui est utilisée pour afficher tout type de variables ou bien des messages devant être affichés à l’utilisateur dans la console d’un navigateur ou dans le terminal.Pour afficher le contenu des variables en JavaScript, on utilise la méthode console.log en passant autant de variables qu’on veut en paramètres : console.log(permiere_variable, deuxieme_variable, ...).

##Les boucles

Faire répèter à l'ordinateur une série d'instructions tant qu'une condition est respectée.

- while
- for
- ...
  
###While

Exemple:
Demander à l'user de saisir son âge

    let age = window.prompt("Quel est votre âge?");

    while (isNaN(age)) {
        age = window.prompt("Merci de répondre un nombre. Quel est votre âge?);
    }

    console.log("vous avez " + age + " ans.");
Age demandé, puis :
"tant que l' âge n'est pas un nombre (is NaN),alors on demande l'âge de nouveau.
La boucle ne s'arrêtera qu'une fois que la condition, dans parenthèse du while, n'est plus respectée : âge sera un nombre.

Exemple :
Exécuter la boucle un nombre défini de fois.

    let cpt = 0;

    while(cpt<=20){
        cpt++;
        console.log(cpt);
    }
La boucle s' exécute tant que le compteur est plus petit que 20.On incrémente le compteur de 1 à chaque tour.

**Attention à bien penser à incrémenter,sion boucle infinie!**.

###For

![for](img/for.png)

Cette boucle est un peu particulière, elle a dans ses paramètres un **index, une condition,et une incrémentation**.
C'est la boucle utilisée pour parcourir un tableau bien souvent.

    for(let i=0; i<liste.lenght ; i++){
        console.log(liste[i]);
    }
->initialisation : let i=0 = initialisation de l'index qui va être incrémenté.
->condition : i<liste.lenght = condition qui doit être respectée pour que la boucle continue.
->incrémentation : i++ = incrémentaiton de l'index.
Cette boucle passe par chaque case du tableau liste et afficher ce qu'il contient en console.

####Portée de la variable ou scope:

Dans l'exemple précédent nous déclarons la variable i dans la boucle for.Les variables déclarées avec let ne sont utilisables que dans la structure dans laquelle elles sont déclarées.

Exemple:

    for(let i=0; i<liste.lenght ; i++){
        console.log(liste[i]);
    }
    console.log(i);
->console va retourner une erreur! "i is not defined"
**Elle ne connaît pas i car déclarée dans for donc non utilisable en dehors.**
**Valable pour tous les blocs, if, while,...**

##Les conditions

![if](img/if.png)

![if else](img/else_if.png)

![switch](img/switch.png)

Structures de contrôle, qui permettent de contrôler les instructions en fonction de l'évolution du programme.
Permet d' effectuer des actions en fonction de paramètres, afin de dynamiser le site et ajouter des intéractions.

Il en existe deux sortes : **conditions et boucles**.

Une condition est un test que va effectuer le programme, et nous allons lui indiquer ce qu'il doit faire si cette condition est vraie,ou faire si fausse.

###Comment JavaScript compare différentes valeurs?

Le JS saît comparer différentes valeurs entre elles. A chaque fois que l'on compare différentes valeurs, le JS renvoie un booléen:  soit valeur true ou soit false.

Exemples:
Si l'user a plus de 18 ans, on va lui dire qu'il est majeur, sinon, on lui dira qu'il est mineur.

    let age = window.prompt("Quel âge avez-vous?");
    console.log(age);

    age = parseInt(age);
    ->on parse l' age pour le considérer comme un nombre.

    if(age === 18){
        console.log("vous êtes majeur);
    }
    else{
        console.log("vous êtes mineur");
    }
    ->dans ce cas, si age=19, le programme nous dira que nous sommes mineur,il faut utiliser un autre opérateur(=== sécurité pour nombre, pas de parse si == mais risque de NaN).

    var x = 7, y = 14;
    var vrai = x < y;
    var faux = 14 <= 7;
    var egalVal = 4 == "4"; => true
    var egalVaType = 4 === "4"; => false
    var difValType = 4 !== "4"; => true

Pour effectuer un test à l' intérieur d'une condition, nous aurons besoin d' **opérateurs de comparaison**.

###Les opérateurs

Voici les différents opérateurs possibles pour effectuer une comparaison entre deux variables :

|Opérateurs|Signification|
|:------|:------|
|==|égal à (en valeur)|
|!=|différent de (en valeur)|
|===|strictement égal à (en valeur ou en type)|
|!==|strictement différent (en valeur ou en type)|
|>|supérieur|
|>=|supérieur ou égal|
|<|inférieur|
|<=|inférieur ou égal|

Exemples:

    4 == "4" => true car même valeur.
    4 === "4" => false, valeur ok mais type différents.

###If Else

Structure conditionnelle qui va permettre de tester une condition et de réaliser des instructions différentes selon qu'elle est vraie ou fausse.

    if(condition){
        instruction si vraie;
    }
    else{
        instruction si fausse;
    };

    var heure = 18;
    if(heure <= 20 == true){
        alert("Bonjour");
    };
    ->comparaison 18 à 20=>envoie valeur true ou false puis si JS renvoie bien true ( == true)=> exécution alert

    if(typeof(heure) == "number" == true){
        alert("c'est le matin");
    } => true
Le programme effectuera les instructions présentes entre les accolades du if si la condition entre parenthèse retourne true,inon du else si retourne false.

Else non obligatoire.

L'on peut enchaîner les if:

    if(age >= 100){
        console.log();
    }
    else if(age >= 18){
        console.log();
    }
    else{
        console.log();
    }

###Conditions multiples et opérateurs logiques

Les conditions dans les structure de contrôle peuvent être multiples.
C'est là qu'interviennent les **ET, OU et CONTRAIRE ou NON**.
Cela permet d' effectuer plusieurs comparaisons.

#### &&  AND

Permet d' avoir un intervalle de comparaisopn pour une variable.

Exemple:

    let prenom = "paul";
    if(age >= 100 && prenom === "paul"){
        console.log("Bonjour paul");
    };
**&& = et**: Il faut que les deux conditions retournent true pour que les instructions puissent être exécutées.

#### || OR

    let prenom = "paul";
    if(age >= 100 || prenom === "paul"){
        ;
    };
**|| = ou**: Il faut que l'une des deux conditions retourne true pour l'exécution.

#### Contraire, NON

Permet de lier le résultat des comparaisons, ainsi les comparaisons évaluées de base à false, vont être évaluée à true et inversement. 

Exemple :

    let heure = 18;
    if(!(heure <= 16) == true ){
        alert("il est plus de 16h");
    };
    ->on lie le résultat envoyé par Js, qui est: false car 18>16, on lie donc, le résultat renvoyé devient true => true = true

### Switch

Permet de comparer la valeur d'une variable avec une multitude de valeurs possibles et d'agir en fonction.
Pratique lors de la comparaison d'une variable à plusieurs valeurs.
**Elle ne teste que l'égalité**.

Exemple:

    let nombre = window.prompt("choississez un nombre entier entre 1 et 8");
    nombre = parseInt(nombre);

    switch(nombre){
        case 1 :
        console.log("");
        break;
        case 2 :
        console.log("");
        break;
        default :
        ;
        break;
    }
->Chaque valeur possible se trouve avec un case, ici comparaison var nombre à des chiffres donc pas de "", si chaîne de caractères ne pas les oublier.

**Default permet de définir une action si aucune des valeurs des case ne correspond au contenu de la variable.Il est optionnel**.

L'on peut définir une même action pour plusieurs valeurs différentes :

    switch(){
        case : case :
        ;
        break;
    }

##Les fonctions

![fonctions](img/fonctions.png)

Lorsque le code devient trop long et répétitif, il est possible de l'organiser en petites unités appelées **fonctions**, qui vont s'occuper d'une tâche précise.

Leurs avantages:
- Raccourcir le code en évitant de répéter des lignes de code identiques
- Appeler une fonction suite à une action de l'user
- ...
  
Exemple:

    function sayHello(nom,prenom){
        const hello = "bonjour ${prenom} ${nom};
        returnhello;
    }
->cette fonction retourne une chaîne de caractère
**function**: création de fonction
sayHello: nom de la fonction
(nom,prenom): **arguments**,permettent de spécifier que pour utiliser notre fonction,il faudra lui apporter ces deux arguments, ces deux données
**return**hello: la fonction va répondre quelque chose

###Les arguments

Optionnels,une fonction peut ne pas avoir besoin de données d'entrée.La parenthèse sera vide.
Il peut y avoir autant que nécessaire.

###Le retour

**Return** optionnel.
Permet aussi de stopper une fonction,si un bout de code est écrit après il ne sera pas exécuté.

###Réutiliser la fonction

Exemple:

      function sayHello(nom,prenom){
        const hello = "bonjour ${prenom} ${nom};
        returnhello;
    }
    console.log(sayHello("vilport","cecile"));

###Valeurs par défaut

Il est possible de spécifier des valeurs par défaut pour nos arguments, aisni si un user oublie  ou ne connaît pas un des arguments demandés,une valeur par défaut lui sera attribuée.
De ce fait, ceci permet également, de rendre cet argument optionnel:

      function sayHello(nom,prenom = "M/Me"){
        const hello = "bonjour ${prenom} ${nom};
        returnhello;
    }
    console.log sayHello("vilport");
-> M/Me vilport

##Le DOM

###Window

L'objet window est l'objet global qui représente votre fenêtre.Tout code JS qui est exécuté sur une page à accès à cet objet.
On peut avoir accès à des informations de l'historique window.history de l'onglet, ainsi que différentes informations comme la largeur window.interface...

test : console.log(window);

###Le DOM

![DOM](img/DOM.png)

Document Object Model, structure du fichier HTML, il nous permet d'atteindre les différents éléments et de pouvoir agir dessus.

###La sélection d'éléments

Il existe plusieurs façon de sélectionner des éléments:

####getElementById

Sélection par l'id

Exemple:

    let divUne = document.getElementById("id");
On peut ainsi agir dessus pour lui apporter des modifications:

    divUne.style.backgroundColor = "color";
    divUne.style.padding = "1em";

Remarque: les propriétés CSS qui sont habituellement en plusieurs mots sont transformés en camelCase pour la manipulation JS.

####QuerySelector

Sélecteur plus souple, il permet de sélectionner n' importe quel élément du DOM avec un simple sélecteur CSS.

exemple:

    let divUne = document.querySelector("#id");

    let divUne = document.querySelector("div:nth-child(1)");

####QuerySelectorAll

Sélection de plusieurs éléments en même temps.

Exemple :

    let divs = document.querySelectorAll("div");
Sélection de toutes les div du doc.

###AddEventListener

Sert à ajouter un événement à un élément du DOM.**Un événement est une action de l'user ou du programme**.

    monElement.addEventListener("evenement",functionALancer);

####DOMContentLoaded

Evénement qui se produit quand la page web est chargée, et qui indique que tous les éléments sont prêts, et donc que l'on peut agir sur la page avec  le code JS.

    document.addEventListener('DOMcontentLoaded",function()){
    action
    }   

####Exemple sur les boutons 

    function onClick2(){
    alert("coucou");
    }

    function onClick1(){
        let titre = document.querySelectorAll("h2");
        for(i=0;i<=titre.lenght;i++){
            titre[i].classList.toggle("blue");
        }
    }

    function changerDeCouleur(){
        var maDiv = document.getElementById("id");
        maDiv.classList.toggle("backgroundfonce");
    }

    document.addEventListener("DOMcontentLoaded",function(){
        let button2 = querySelector("#idbutton");
        let button1 = document.getElementById("changerBackground");

        button2.addEventListener("click",onClick1);
        button1.addEventListener("click",changerCouleur);
    })

####RemoveEventListener

Retirer un événement, par exemple désactiver un bouton.

button1.removeEventListener("click",changerCouleur);

Il est important que la fonction de **callback** ainsi que l' événement soient les mêmes que lors de l'ajout.
>En Javascript (est comme c’est le cas dans d’autres langage de programmation), les fonctions sont des entités d’ordre supérieur ou de classe supérieure. De telles fonctions permettent d’abstraire les valeurs et les actions, c’est-à-dire qu’elles peuvent accepter des fonctions en guise d’arguments au même titre que les variables et elles peuvent aussi retourner des fonctions. Une fonctions passée en argument d’une autre fonction est appelée fonction de rappel ou callback function.

###classList

La propriété classList sert à gérer les classes des balises Html
.
Voici quelques-unes de ses méthodes :

- monElement.classList.add("maClasse) -> ajoute une classe
- monElement.classList.remove("maClasse) -> retire une classe
- monElement.classList.toggle("maClasse) -> ajoute ou enlève une classe
- monElement.classList.lenght("maClasse) -> retourne le nombre de classe que l'élément contient  

###Variable this

Dans un gestionnaire d'événement; la variable **this** représente l'objet DOM qui a déclenché l'événement.

Exemple :
On passe la souris sur une div du DOM, le bakground va changer de couleur.
On commence par sélectionner les divs et par leur affecter un événement:

    let divs = document.querySelectorAll("div");
    divs.addEventListener("mouseover",changerText);

Puis on crée la fonction :

    function changerText(){
    this.classList.add("green");
    }
Au sein de la fonction, this représentera uniquement la div sur laquelle nous avons passé la souris,celle qui a déclénché l'événement.

###TextContent

Modifie le contexte textuel d'un noeud du DOM.

Exemple :

    <div id="maDiv">Hello</div>

    let maDiv = document.getElementById("maDiv");
    alert(maDiv.textContent);
->renvoie hello

    maDiv.textContent = "Bonjour";
->modifie contenu de la div

###InnerHTML

Equivalent de textContent en HTML:
**monElement.innerHTML**.
Contrairement à textContent, il va interpréter le code HTML compris dans la variable.

Exemple:

    monElement.textContent = "<strong>Coucou</strong>
->retourne une valeur qui ne sera pas en gras alors qu'avec innerHTML si.

##Les timers

JavaScript s' exécute sur le navigateur du client et permet d' intéragir vec lui.
Il va donc pouvoir détecter les événements éventuels qui se produisent sur la page.

L'on a vu deux types d' événements : 
- Evénements lancés par la navigateur lui-même:
- - j'ai fini de charger et de lire le HTML (DOMContentLoaded)
- - j'ai fini de charger toute la page et ses dépendances (load)
- Evénements lancés par le client (user):
- - click
- - mouseover...

Nous pouvons intéragir facilement avec ce qu'il se passe sur la page.Mais il manque une notion importante pour compléter ce panel d' événements:
-> comment déterminer le temps qui passe et s' en servie pour lancer des actions?

La gestion du temps en JS, va nous servr à gérer les animations, temporiser des actions...

###SetTimeout et clearTimeout

###setTimeout

Cette méthode va nous permettre de définir un intervalle en millisecondes avant le déclenchement d'une action.

    let timeoutld = window.setTimeout(callBackFunction[,delay,param1,param2,...]);
->paramètres:
- callBackFunction : fonction appelée lors du dépassement de délai. On peut soit fournir une fonction définie ailleurs dans notre code ou une fonction anonyme.
- delay(optionnel) : le délai en millisecondes avant que la fonction callBack soit appelée.Par défaut, vaut 0.**1000ms = 1s**.
- param1,param2 (optionnels) : les paramètres(valeurs) qui seront passés à la fonction callBack.
  
Valeur de retour :
timeoutld : identifiant unique founi par JS?.Si vous souhaitez retrouver et arrêter le timer avant son exécution.

####clearTimeout

Cette méthode permet d' arrêter le timer s'il n'a pas été encore déclenché.

    window.clearTimeout(timeoutld);
->paramètres:
timeoutld

###SetINterval et clearInterval

####setInterval

Méthode qui permet de définir une action qui sera exécutée à intervalles réguliers.

    let intervalID window.setInterval(callbackFunction[,delay,param1,pram2?...]);
->paramètres
- callBackFunction : c'est la fonction qui sera appelée à tous les intervalles déterminés. On peut ici
fournir un nom de fonction défini ailleurs dans notre code ou directement une fonction anonyme
(comme pour toutes les fonctions évènementielles JavaScript qui appellent une fonction de callBack),
- delay (optionnel) : le délai en millisecondes entre chaque intervalles d’exécution de la fonction de
callBack. Par défaut, ce paramètre vaut 0, la fonction est exécutée dès que possible et
continuellement.
- param1, param2... (optionnels) : les paramètres (valeurs) qui seront passés à la fonction de callBack.

Valeur de retour:
timeoutID : un identifiant unique fourni par Javascript si vous souhaitez retrouver et arrêter votre "timer" à tout moment.

####clearInterval

Cette méthode va nous permettre d'arrêter le "timer" à tout moment.

    window.clearInterval(intervalID);


###RequestAnimationFrame et CancelAnimationFrame

####requestAnimationFrame

Cette méthode va nous permettre de définir une action qui sera exécutée au rafraichissement de l'écran.

    let animationID = window.requestAnimationFrame(callBackFunction);
->paramètres:
- callBackFunction : c'est la fonction qui sera appelée au prochain rafraichissement de l'écran. On peut
ici fournir un nom de fonction défini ailleurs dans notre code ou directement une fonction anonyme (comme pour toutes les fonctions évènementielles JavaScript qui appellent une fonction de callBack),

valeur de retour:
animationID : un identifiant unique fourni par Javascript si vous souhaitez retrouver et arrêter votre
demande de rafraichissement à tout moment.

####cancelAnimationFrame

Cette méthode va nous permettre d'arrêter l’exécution du rafraichissement à tout moment.

    window.cancelAnimationFrame(animationID);

>**Mieux comprendre le fonctionnement : les FPS
Alors que setInterval et setTimeout fonctionnent avec un délai en millisecondes, requestAnimationFrame lui va
être exécute à chaque fois que le navigateur fait appel au rafraichissement de l'écran auprès de la machine du
client (rafraichissement assuré en grande parti par le processeur graphique).
Cela signifie que :
• la méthode requestAnimationFrame est plus adapté à la création d'animations fluides,
• le rafraichissement va dépendre de la machine client, en général un écran est rafraichi 60 fois par
seconde, on dit que l'on affiche 60 FPS (frames par seconde),
• le rafraichissement va dépendre aussi du travail demandé au navigateur mais aussi de sa capacité à ce
moment là d'assurer le travail (capacité de l'ordinateur, navigateur plus ou moins utilisé et nombre
d'onglets ouverts), les FPS sont donc variables comme dans les jeux vidéos, mais le rafraichissement
sera effectué quoi qu'il arrive,
• le navigateur va optimiser et préparer le rafraichissement, contrairement à un setInterval, il sait ce
qu'il a à faire au prochain rafraichissement et va le prioriser et l'optimiser,
• le navigateur ne fera l'action de rafraichissement que si l'onglet du navigateur comportant le script est
actif, contrairement à setInterval et setTimeout qui continuerons à être exécutés même si un autre
onglet est actif (donc on optimise la charge du navigateur).
Alors tout ça à l'air magique mais il y a ici une chose que nous ne maitrisons pas c'est le nombre de frames par
seconde (FPS). Il nous faudra ralentir le taux de rafraichissement si nous en avons besoin.**

##Ajax

Ajax (Asynchonous Javascript and XML) est méthode qui permet de rafraîchir une partie de page Web
sans recharger la page complète. Il permet aussi d’afficher dynamiquement des données obtenues en PHP
(exemple des données issues d’une base de données).
Un exemple : Facebook !
Lorsque vous créez une publication, il faut un système qui enregistre votre publication et en même temps
l’affiche sur votre fil d’actualité. Ajax fait ça !
Pour mettre à jour une base de données, de quoi a-t-on besoin ? D’un langage côté serveur (donc php) et
pour rafraîchir la page : d’un langage côté client. Ajax met en relation ces 2 langages !

###Comment fonctionne un appel Ajax :

- L’utilisateur créé un évènement (un clic ou autre)
- Le navigateur envoie sa requête ajax(en jquery) à un script PHP
- Le script PHP fait ce qu’il a à faire (insertion ou consultation de bdd, envoi de mail…)
- Le script PHP renvoie une réponse à l’appli Jquery
- Jquery traite la réponse et l’affiche

###Renvoi d'un appel

Un appel AJAX va renvoyer différents types de données :
- Des données simples (chaînes de texte)  Dans le fichier PHP, nous aurons soit juste du
texte, soit une fonction qui renvoie du texte
- Du html  Du code HTML dans le fichier PHP
- Du Json  Le fichier php renvoie un JSON avec la fonction json_encode()

###Comment fait-on?

Il y a plusieurs façons d’écrire une requête Ajax, la syntaxe en JavaScript pur est assez complexe, la voici :

[OpenClassroom code](https://openclassrooms.com/fr/courses/245710-ajax-et-lechange-de-donnees-en-javascript/244798-lobjet-xmlhttprequest)

##Exercices (voir dossier exercicesMM) :

- Afficher "Hello World" dans la console du navigateur.
- Déclarer une variable avec le mot-clé let ayant comme nom « color ».Puis, sur la ligne suivante, lui assigner la valeur « rouge ».
- Déclarer une variable « msg » avec le mot-clé `const` en lui assignant une valeur de votre choix, telle qu'un message ou un nombre.Afficher la valeur de cette variable dans la console du navigateur.
- Déclarer une variable ayant pour type String.Afficher la valeur de cette variable dans la console du navigateur.
- Déclarer une variable `x` dont la valeur est égale à `66`. Déclarer une variable `y` dont la valeur est égale à `12`.Déclarer une variable `result` dont la valeur est égale à la somme de `x`et `y`.Afficher la valeur de la variable `result` dans la console du navigateur.
- projet - hello you Hello You
Nous allons construire ensemble un programme capable de vous saluer avec votre prénom. Pour cela, nous allons d'aboir devoir apprendre à interagir avec l'utilisateur.
window.prompt. Jusqu'à maintenant, nous ne connaissons qu'une seule fonction : console.log. Apprenons-en une deuxième : const userAge = window.prompt("Quel âge avez-vous ?");
console.log(userAge);
Si vous exécutez cette instruction, votre navigateur va ouvrir une petite fenêtre avec un champ de texte en vous posant cette question « Quel âge avez-vous ? » Vous allez entrer par exemple « 22 » dans le champ, valider, et la console affichera alors "22".window.prompt a pour fonction de demander quelque chose à l'utilisateur, et de renvoyer la réponse ainsi reccueillie sous forme de String. Ici nous stockons directement cette valeur de retour dans la variable userAge pour ensuite l'afficher.
window.prompt renvoie toujours, toujours une String. Même si l'utilisateur entre le nombre 12, window.prompt renverra en fait la chaîne "12".
Cette information aura son importance en temps voulu. Vous n'en aurez pas besoin pour cet exercice.
Nous voulons un programme qui demande à l'utilisateur son prénom, disons par exemple « Jacques », pour ensuite afficher dynamiquement dans la console "Salut Jacques !".
Petit indice : vous allez avoir besoin de concaténer des Strings.
Bonus 1:
Notre programme va désormais demander à l'utiliseur son prénom, son nom de famille et son année de naissance. Nous afficherons ensuite dans la console la phrase suivante : "Salut Jacques Dumont, cette année tu 42 ans !"
Afin de calculer l'âge de l'utilisateur, vous allez avoir besoin d'effectuer un calcul à partir de l'année. Pour ce bonus, vous êtes autorisés à la spécifier en dur dans le code, sans forcément chercher à la dynamiser. Par exemple, en 2021, vous pourrez simplement déclarer une variable const currentYear = 2023;.
- Date du jour. Afficher dynamiquement la date du jour en Html sous la forme de nous sommes le mardi 23 évrier 2023.
- L' user saisit un montant HT, le résultat TTC s'affiche en HTML.
Il faut réaffciher toutes les informations.Le montant HT est à virgules.
- Énoncé: Créer puis afficher en HTML un objet représentant une voiture :
La marque de la voiture
Son année de fabrication
Sa date d'achat
La liste des passagers (au moins 2), avec le prénom de chacun des passagers
Détails: Afficher les propriétés de l'objet voiture sous la forme d'une liste HTML
On peut représenter n'importe quelle date en JavaScript en donnant une
chaîne de caractères à la création d'une instance de la classe Date :
Représente la date du 5 avril 2014, format américain YYYY-MM-DD. var
myBirthday = new Date('2014-04-05');
Rappels: On peut stocker un objet dans un tableau tout comme on peut stocker un tableau dans un objet...
- Déclarer une variable « colors » contenant les valeurs "Rouge" et "Bleu".Afficher "Bleu" dans la console. En utilisant le tableau, hein!
- Déclarer une variable « colors » contenant un tableau vide.
Puis un second temps, ajouter "Rouge" et "Bleu" à ce tableau.
Enfin, afficher "Rouge" sur la page web, toujours en utilisant le tableau.
- Calculaprompt:
Comment fonctionne une calculatrice ?
On appuie sur des boutons pour construire un calcul, puis on valide, puis la machine nous affiche le résultat du calcul.
On va devoir cliquer sur des boutons ? Non, pas encore. Notre première calculatrice ne sera pas aussi pratique et jolie. Elle sera un peu bancale et malade, mais on va l'aimer quand même, parce qu'elle fonctionnera.
Comment va fonctionner la calculaprompt ?
En demandant à l'utilisateur trois choses d'affilée :
Un premier nombre ;
Un opérateur arithmétique (+, /, +, -) ;
Un second nombre.
Puis, dans la console du navigateur, on affiche un rappel du calcul complet, par exemple 23 / 100.
Puis, toujours dans la console, on affiche le résultat du calcul.
Un exemple pour récapituler le fonctionnement :
L'utilisateur arrive sur la page ;
L'utilisateur entre 6 dans un premier window.prompt ;
L'utilisateur entre * dans un deuxième window.prompt ;
L'utilisateur entre 10 dans un troisième window.prompt ;
La console affiche le calcul 6 * 10 ;
La console affiche le résultat 60 ;

stop : chifoumi , exo3

##Main.js:

- alert
- window.prompt
- elementToString
- objet date
- typeof


 




    



















