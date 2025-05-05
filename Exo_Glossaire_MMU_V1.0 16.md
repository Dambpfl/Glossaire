# GLOSSAIRE

- [Général](#général)
- [Front-end](#front-end)
- [UX / UI](#ux-ui)
- [Architecture](#architecture)
- [Modélisation / Base de données](#modélisation---base-de-données)
- [Symfony](#symfony)
- [Sécurité](#sécurité)
- [RGPD](#rgpd)
- [SEO](#seo)
- [Gestion de projets / DevOps](#gestion-de-projets---devops)
- [English](#english)

## Général
1.	Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte

Laragon et MAMP(sur mac)


2.	Qu’est-ce qu’un algorithme ?  

C'est la logique qui est utiliser pour concevoir le code


3.	Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?

C'est une valeur (chaine de caractères ou un nombre) que je peux changer a tout moment dans mon programme (php = $)


4.	Qu’est-ce que la portée d’une variable ?

C'est la façon dont elle est utilisée, soit dans une fonction ou soit dans tout le programme


5.	Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?

C'est une valeur qui n'est pas vouée à changer contrairement à une variable


6.	Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation 

C'est une variable pré définie comme $_GET,$_POST et $_SESSION en PHP


7.	Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ? Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur)

Int (entier), Float (Nb à virgule), String (Chaine de caractères), Boolean (Vrai/Faux)


8.	Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?

Tableau indexé, associatif, d'objets


9.	Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles

Condition : If/else - Boucle: for/while/foreach - (action unique)switch/case


10.	Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?

strlen($variable)


11.	Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP


Une session est une manière de garder des informations sur un utilisateur pendant qu'il navigue sur un site web (exemple : le panier)


12.	Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP

C'est un fichier que le serveur envoie au navigateur pour stocker les informations sur l'ordinateur ou le téléphone
Cela permet de se souvenir de l'utilisateur entre ces visite sur un site (nom,prenom,panier)


13.	Quelle est la différence entre les instructions « require » et « include » en PHP

Require : Necessaire, si le fichier est introuvable PHP arrête l'éxécution du script

Include : Optionnel, continue le script meme si le fichier est manquant


14.	Comment effectuer une redirection en PHP ?

En utilisant header('Location: page_redirection.php');


15.	Définir la partie « front-end » et « back-end » d’une application

Front-end = Partie que l'utilisateur voit et utilise

Back-end = toute les fonctions/redirections que l'utilisateur ne voit pas


16.	Définir le contrôle de version ? Qu’est-ce que Git ?

Le contrôle de version permet de garder toutes les versions précédentes d'un projet en mémoire, de les rappeler en cas de besoin et de travailler en équipe sans écraser le travail des autres.

Git est un système de contrôle de version qui permet à chaque développeur d'avoir son propre espace de travail sans impacter le code principal et de fusionner les modifications proprement à la fin.

17.	Qu’est-ce qu’un CMS ? Citer au moins 2 exemples

CMS = Content Management System(Systeme de gestion de contenu), c'est un logiciel qui permet de créer,gérer et modifier le contenu d'un site web sans compétences en programmation

Exemple : WordPress, Drupal


## Front-end
18.	Définir HTML

Language de balisage pour structurer et organiser le contenu

19.	Définir CSS

Language de programmation de mise en page

20.	Définir Javascript

Language de programmation pour créer des interactions dynamiques

21.	Définir JSON. Dans quel contexte ce format est-il utilisé ? 

JSON = JavaScript Object Notation

Il est utilisé pour stocker des informations et échanger les données entre un client et un serveur


22.	Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?

Oui, avec Node.js qui est une plateforme baséé sur le moteur V8 de chrome

23.	Qu’est-ce qu’un sélecteur CSS ?

c'est ce qui sert à selectionner un bouton par son id(#) ou sa class(.) par exemple


24.	Quelle balise HTML permet de créer un lien hypertexte ?

la balise <a href="mon lien"></a>


25.	Qu’est-ce qu’une requête AJAX ?

AJAX (Asynchronous JavaScript and XML) c'est une méhode qui permet de charger des données en arriere plan sans recharger la page, ça rends l'application web plus réactive

26.	Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?

class(.) / id (#)

27.	Définir le responsive design

C'est le format téléphone/tablette selon la taille de l'écran

28.	Qu’est-ce que le templating ?

C'est une méthode qui consiste à utiliser des modèles pour générer du contenu dynamique en y injectant des données. On ecrit du code dans une template qui se répete dans les autres vues.

29.	Qu’est-ce qu’une fonction anonyme en Javascript ?

C'est une fonction qui n'a pas de nom

30.	Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?

on utilise push()

31.	Qu’est-ce qu’un « media query » ?

C'est pour définir une taille d'écran en CSS (@media screen and (max-width: 500px))

32.	Qu’est-ce qu’un pseudo élément en CSS ?

C'est pour cibler et styliser un element HTML, qui n'existe pas explicitement, c'est un peu une 'déco magique' (:hover(au passage de la souris l'élément va changer))

33.	Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalent

C'est un framework CSS concu par twitter, il y a Tailwind,Foundation,Bulma qui sont également des frameworks CSS

34.	Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes

GET = Les données sont envoyées dans l'URL sous forme de parametres, affiche les données dans l'URL 

POST = Les données sont soumis via un formulaire principalement (envoyées dans le corps de la requete HTTP), envoie les données discretement


## UX UI
35.	Quelle est la différence entre UX Design et UI Design ?

UI = Interface utilisateur et UX = Experience utilisateur

36.	Qu’est-ce qu’un wireframe ? 

C'est une maquette du site web avec un visuel simple (sans image, couleur,typographie)

37.	Qu’est-ce qu’un prototype ? 

C'est une maquette interactive ou on peux tester la navigation et l'UI

38.	Qu’est-ce que la hiérarchie visuelle en UI Design ?

C'est l'organisation des éléments d'une interface pour guider l'utilisateur en mettant en avant les éléments importants.

39.	Qu’est-ce que l’accessibilité en UX Design ?

rendre une interface utilisable par tout le monde, handicap compris

40.	Qu’est-ce qu’une grille de mise en page ?

C'est un ensemble de lignes/colonnes qui permet d'aligner les éléments de façon correcte

41.	Qu’est-ce que la notion d’affordance en UX Design ?

C'est la façon dont un élément est compréhensible sans explication

42.	Qu’est-ce qu’un « mobile first design » ?

C'est de crée le design pour le mobile avant la version deskop

## Programmation orientée objet (POO)
43.	Donner une définition de la programmation orientée objet 

c'est une façon de coder ou l'on crée des objets qui mélangent des données et des actions(fonction)


44.	Qu’est-ce qu’une classe ? Comment la déclare-t-on ?

C'est un plan qui sert a crée des objets => Class NomDeLaClasse


45.	Qu’est-ce qu’un objet ?

C'est une instance d'une classe avec ses propres attributs

$instance = new Classe('attribut1', 'attribut2'); <=== Ceci est un objet


46.	Définir la notion de propriété / attribut / méthode

Propriété = Permet d'accéder et de modifier un attribut

Attribut = Variable qui stocke l'information de l'objet (ex : Voiture(Marque/Couleur))

Méthode = Fonction définie dans la class (démarrer/accelerer)


47.	Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité

Private/Protected(heritage) et Public


48.	Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?

$voiture = New Voiture("attribut 1" etc..)


49.	Qu’est-ce que l’encapsulation ?

Proteger les données (private)


50.	Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple

L'héritage (Parent Protected //class extend parent// construct::parent)


51.	Définir l’opérateur de résolution de portée

L’opérateur de résolution de portée :: permet d’accéder aux méthodes et propriétés statiques, aux constantes d’une classe, et aux méthodes héritées d’une classe parente

52.	Définir une méthode / propriété statique

C'est une propriété que tout le monde peut lire et modifier sans devoir créer un nouvel objet à chaque fois

53.	Définir le polymorphisme en POO

Le polymorphisme permet d’utiliser un même nom de méthode, mais avec un comportement différent selon l’objet (exemple: function crier() => change selon l'animal(class))

54.	Définir une méthode / classe abstraite ?

Classe abstraite :
C’est une base qui pose des règles générales pour d’autres classes, mais elle ne peut pas être utilisée directement. Les classes qui l’héritent doivent compléter les détails
C'est le livre de recettes -> donne les instructions générales

Méthode abstraite:
C’est une instruction qui ne fait rien toute seule, mais qui définit une action à réaliser dans les classes enfants. Ces dernières doivent ajouter leur propre comportement pour que ça fonctionne
C'est une recette à completer -> chaque chef doit ajouter sa propre façon de faire

55.	Définir le chaînage de méthodes

C'est quand un objet a plusieurs méthodes et qu'on veut toutes les appeler une après l'autre, sans appeler l'objet à chaque fois

56.	Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »

le __toString() c'est pour donner des infos légère a une variable sans passer par une fonction(ex:nom,prenom) - Methode magique = fonction native de php


57.	Qu’est-ce qu’un « autoload » ?

C'est une fonction qui permet de charger automatiquement les fichiers d'une classes sans avoir a le faire manuellement avec include ou require

58.	Comment appelle-t-on en français les « getters » et les « setters » ?

Getter = Accesseur (Lire valeur attribut ou objet)

Setter = Mutateur (Modifier valeur attribut ou objet)

59.	Qu’est-ce que la sérialisation en PHP ? 

ça permet de convertir un objet en string pour pouvoir le sauvegarder et le réutiliser plus tard en tant qu'objet

## Architecture 
60.	Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence

Le client envoie les requete de l'utilisateur et le serveur lui reponds avec les données stocker dans la bdd

Requete => GET,POST,PUT,DELETE

HTTP = HyperText Transfer Protocol => le client communique avec le serveur

HTTPS = HyperText Transfer Protocol Secure => chiffre la communication entre le client et le serveur


61.	Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern

C'est un ensemble de méthodes déja créer qui peuvent etre réutiliser

Singleton, Factory Method, Observer

62.	Qu’est-ce que l’architecture MVC ?

Model-View-Controller c'est une façon d'organiser son code en triant les informations/vues dans des dossiers pour s'y retrouver plus facilement

63.	Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?

Model => gere les données et la logique métier (Manager => requete SQL)

View => affiche les données et les boutons d'interactions

Controller => on y ecrit les méthodes qui vont gerer les interactions de l'utilisateur

64.	Quels sont les avantages de l’architecture MVC ?

ça facilite la compréhension du code, car chaque dossier a une fonction c'est donc plus facile de s'y retrouver

65.	Existe-t-il des variantes à l’architecture MVC ?

Oui, MVP (Model View Presenter), MVU (Model Update View)

66.	Qu’est-ce qu’une API ? Définir l’architecture REST (Representational State Transfer)

permet la communication entre un site web et un serveur dans le cloud // on envoie une requete dans une opération http et lui renvoie une reponse

requete --> CRUD = POST(CREATE), GET(READ), PUT(Update), DELETE(Delete)

## Modélisation - Base de données
67.	Qu’est-ce que la modélisation de données ? Définir la méthode Merise

C'est structurer et organiser les informations - La méthode Merise est une approche en 3 etapes

68.	Quelles sont les 3 étapes principales de la méthode Merise ? 
a.	Analyse, conception et réalisation <-------->
b.	Planification, exécution et contrôle
c.	Création, modification et suppression

69.	Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?

C'est une carte qui montre les objets importants d'un système (client, produit) et comment ils sont liés.

70.	Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?

Il montre comment sont organisées et structurées les informations.

71.	Donner la définition des mots suivants :

a.	Entité 

 L'objet important (client, produit)

b.	Relation 

 Comment deux objet sont liés entre eux (Client peut passer Commande)

c.	Cardinalité 

 Le nombre de fois ou les objets sont liés entre eux (0,n / 1,n / 1,1 / 0,1) valeur min,max(n = plusieurs)

d.	Clé primaire / clé étrangère

Primaire => c'est un identifiant unique pour chaque objet/element

Etrangere => C'est le lien qui relie deux tables ensemble


72.	Que devient une relation de type « Many To Many » dans le modèle logique de données ?

Elle devient une relation OneToMany avec une table associatif

73.	Qu’est-ce qu’une base de données ?

C'est l'endroit où l'on stocke toutes les informations.

74.	Définir les notions suivantes : 

a.	SQL (Structured Query Language)

SQL est un language de programmation 

b.	MySQL

MySQL est un systeme de gestion de bases de données relationnelles

c.	SGBD (donner 2 exemples de SGBD)

Systeme de gestion de bases de données -> MySQL et PostgreSQL

75.	Dans une base de données, les données sont stockées dans des _tables.
Celles-ci sont constituées de lignes appelées _enregistrements/tuples et de colonnes appelées _champs/attributs.

76.	Quelle est la différence entre une base de données relationnelle et non relationnelle ?

Relationnelle = SQL -> stocke les données sous forme de tables(relation entre les données)

Non relationnelle = NoSQL -> ne stocke pas les données sous forme de tables(pas de relation entre les données)

77.	Qu’est-ce qu’une jointure dans une base de données ? En existe-t-il plusieurs ? Si oui lesquelles ?

C'est une opération SQL pour combiner les données de plusieurs tables suivant une condition commune, il en existe 6 types principaux
INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN, CROSS JOIN, SELF JOIN

78.	A quoi sert une vue dans une base de données ?

C'est une table virtuelle qui stocke une requete SQL(pas de données) qui est éxécutée chaque fois que la vue est utilisée

79.	Qu’est-ce que l’intégrité référentielle dans une base de données ?

L'intégrité référentielle garantit qu'une information liée entre deux tables reste toujours cohérente : on ne peut pas avoir une commande associée à un client qui n'existe pas

80.	Quelles sont les fonctions d’agrégation en SQL ?

COUNT(), SUM(), AVG(), MIN(), MAX()

81.	Qu’est-ce qu’un CRUD dans le contexte d’une base de données ?

Create -> Ajouter une nouvelle donnée
Read -> Récupérer des données
Update -> Modifier une donnée
Delete -> Supprimer une donnée

82.	Quelles sont les clauses qui permettent de :
a.	Insérer un nouvel enregistrement dans une table

INSERT INTO

b.	Modifier un enregistrement dans une table

UPDATE SET 

c.	Supprimer un enregistrement dans une table

DELETE FROM

d.	Supprimer la base de données

DROP DATABASE

e.	Filtrer les résultats d’une requête SQL

WHERE

f.	Trier les résultats d’une requête SELECT

ORDER BY

g.	Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique

GROUP BY

h.	Concaténer 2 chaînes de caractères 

CONCAT(nom, ' ', prenom) AS nom_complet

83.	Comment se connecter à une base de données en PHP ? Quelle est la classe native utilisée ?

Avec la classe native PDO (PHP Data Objects)

$pdo = new PDO("mysql:host=$host;dbname=$dbname;charset=utf8", $username, $password)



## Symfony
84.	Qu’est-ce que Symfony ?

C'est un framework PHP open-source, architecture MVC (Model-View-Controller)

85.	Sur quel langage de programmation et design pattern repose Symfony ? 

PHP -> MVC(Model-View-Controller)

86.	Quelle est la dernière version en date de Symfony ?

Version 7.2.3 de novembre 2024

87.	Qu’est-ce qu’un bundle ? 

C'est un ensemble de functionnalités réutilisables, qui peut etre ajouté à une application

88.	Quel est le moteur de template utilisé par défaut dans Symfony ?

c'est Twig

89.	Qu’est-ce qu’un ORM ? Quel est son utilité et comment s’appelle-t-il au sein de Symfony ?

ORM(Object-Relational Mapping) technique pour manipuler des BDD en utilisant des objets (crée automatiquement les requetes SQL, CRUD)

90.	Qu’est-ce que l’injection de dépendances ? Quel est l’outil utilisé dans ce contexte et quel fichier contient l’intégralité des dépendances du projet ?

L'injection de dépendances permet de fournir des objet necessaires à une classe via le conteneur de services dans symfony

les dépendances sont dans le ficher services.yaml

91.	Que permet le bundle Maker au sein de Symfony ? 

Ce sont des commandes à rentrée dans la console qui permet de generer automatiquement des composant de base, Entity, Controllers, FormType

92.	Quel est le langage de requêtage exploité au sein d’un projet Symfony ?

DQL (Doctrine Query Language) -> version orientée objet de SQL

93.	Quel est le composant qui garantit l’authentification et l’autorisation des utilisateurs ?

Le Security Component configuré dans le fichier security.yaml

## Sécurité
94.	Qu’est-ce que l’injection SQL ? Comment s’en prémunir ?

C'est une attaque où l'on insère des requêtes SQL. On s'en prémunit en utilisant des requêtes préparées

95.	Qu’est-ce que la faille XSS ? Comment s’en prémunir ?

XSS = Cross-Site Scripting (Injection de code via un formulaire ou le DevTool)

Une des façons de s'en prémunir est d'utiliser des filtres en PHP (ex :FILTER_SANITIZE_STRING)

96.	Qu’est-ce que la faille CSRF ? Comment s’en prémunir ?

Cross-Site Request Forgery c'est une attaque qui consiste à piéger une action d'un autre utilisateur connecter à son insu

exemple: il clique sur un lien piéger qui execute une requete sans son consentement 

Contre -> Utiliser un token CSRF pour s'assurer que la demande viens bien de l'utilisateur légitime

97.	Définir l’attaque par force brute et l’attaque par dictionnaire

Force brute -> Tester toute les combinaisons possible à l'aide d'un programme jusqu'à trouver la bonne

dictionnaire -> Test une liste de mots couramment utilisés comme mot de passe


98.	Existe-t-il d’autres failles de sécurité ? Citer celles-ci et expliquer simplement leur comportement

RCE (Remote Code Execution) -> Exécution de commandes sur le serveur.

MITM (Man-In-The-Middle) -> Espionner/modifier les échanges entre client et serveur.

Clickjacking -> Tromper un utilisateur en cachant des actions sous un faux bouton.

DDoS (Déni de service) -> Saturer un serveur avec des requêtes.

Credential Stuffing -> Utiliser des mots de passe volés sur d’autres sites.

99.	A quoi servent l’authentification et l’autorisation dans un contexte d’application web ?

authentification -> Vérifie l'identité de l'utilisateur

autorisation -> Definie les permissions de l'utilisateur (admin, utilisateur)

100.	Définir la notion de hachage d’un mot de passe et citer des algorithmes de hachage

Le hachage transforme un mot de passe en une chaîne fixe et irréversible, permettant de le stocker de façon sécurisée sans le récupérer.

Hachage fort : Bcrypt et Argon2

Hachage faible : SHA-256 et MD5


101.	Qu’est-ce qu’une politique de mots de passe forts ?

Elle impose que les mot de passe soient long, complexes et difficiles à deviner

102.	Qu’est-ce que l’hameçonnage ?

L'attaquant ce fait passer pour une organisation légitime (banque,service en ligne etc..) afin de tromper l'utilisateur et de récupérer des informations sensible

103.	Définir la « validation des entrées »

Ce sont des filtres qui s'assure que les caracteres entrée dans un formulaire soit bien comforme à ce qui est demandé 

## RGPD
104.	Qu’est-ce que le RGPD ?

Reglementation generale sur la protection des données

105.	Quel est son objectif principal ?

Fixe les conditions de collecte/conservation/exploitation des données

106.	Quelle est la date d’entrée en vigueur du RGPD ?

25 mai 2018

107.	Quelles sont les sanctions possibles en cas de non-respect du RGPD ?

Mise en demeure/amande administrative/Rappel à l'ordre ou formation restreinte

108.	En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ?

CNIL (Commission nationale de l'informatique et des libertés)

109.	Quel est le consentement valide selon le RPGD ?

Explicite et éclairée

110.	Qu’est-ce qu’une politique de confidentialité ?

Un document expliquant en détail les modalités de traitement des données personnelles dans le cadre d’une relation commerciale

111.	Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?

3ans (36mois)

112.	Quels sont les droits des utilisateurs selon le RGPD ?

 droits d'information
       - droit d'acces
       - droit de rectification
       - droit d'opposition  (1mois pour répondre)
       - droit à l'effacement (à l'oubli)

nouveaux droits:
       - droit à la portabilité
       - droit à la limitation du traitement
       - droit lié a la prise de decision automatisée

113.	Qu’est-ce que le principe de minimisation des données selon le RGPD ?

De collecter le minimum de données possible et de justifier chaque collecte

## SEO
114.	Qu’est-ce que le SEO ? 

Search Engine Optimization (Optimisation pour les moteurs de recherche)

115.	Quel est l’objectif principal du SEO ?

Améliorer le référencement d'un site web

116.	Existe-t-il plusieurs types de référencement ? Lesquels ?

SEO -> référencement naturel (Vocal, mobile, vidéo, local)

SEA -> référencement payant (ex: publicité)

117.	Qu’est-ce que la densité de mots-clés en SEO ?

c'est le pourcentage de fois qu'un mot-clé apparaît dans un texte par rapport au nombre total de mots

118.	Qu’est-ce qu’une balise « alt » ?

c'est une description textuelle ajoutée aux images pour les comprendres si elle ne se charge pas

119.	Qu’est-ce que la balise « meta description » ?

c'est une courte description HTML d'une page web, elle résume le contenu de la page et incite les utilisateurs à cliquer sur le lien

120.	Qu’est-ce que le « nofollow » en SEO ?

c'est une façon de rediriger des utilisateurs avec un lien payant ou non fiable sans perdre de valeur de referencement

121.	Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?

Un contenu bien conçu et utile permet aux moteurs de recherche de mieux comprendre le site, d'améliorer sa visibilité et de d'attirer plus de visiteurs

122.	Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?

Les balises de titre permettent de structurer et de hiérarchiser le contenu pour le rendre plus lisible, à la fois pour les utilisateurs et les moteurs de recherche afin d'améliorer le référencement et l'accessibilité

123.	Quelle est la recommandation pour les URL d'un site web bien référencé ?

être courtes, descriptives, inclure des mots-clés pertinents

124.	Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?

c'est l'ensemble des liens hypertextes qui relient les pages d'un même site

125.	Qu'est-ce que l'optimisation des images pour le référencement ?

reduire la taille, adaptés le format et ajouter des attributs alt

126.	Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?

c'est un fichier XML qui liste toutes les pages importantes d'un site web,  il aide les moteurs de recherche à explorer et indexer efficacement le contenu du site

## Gestion de projets - DevOps
127.	Qu’est-ce que la gestion de projet ?	

 Planifier, organiser, coordonner et superviser les ressources et les tâches

128.	Qu’est-ce qu’une méthode Agile de gestion de projet ? 

Collaboration continue avec le client, adaptation aux changement

129.	Expliquer la méthode MoSCoW en quelques lignes et citer ses avantages

c'est une technique de gestion des priorités qui classe les exigences d'un projet en quatre catégories : Must have (indispensables), Should have (souhaitables), Could have (facultatives), et Won't have (non prioritaires pour l'instant).

130.	A quoi sert la méthodologie MVP ? Citer les caractéristiques clés

MVP (Minimum Viable Product) sert à développer un produit avec les fonctionnalités minimales nécessaires pour répondre aux besoins de base des utilisateurs

developpement rapide, produit simplifié, focus fonctionnalités essentielles

131.	Qu’est-ce que la planification itérative ?

ça consiste à diviser un projet en cycles, permettant d'ajuster et d'améliorer le produit à chaque étape en fonction des retours et des évolutions

132.	Citer 3 méthodes Agiles dans le cadre d’un projet informatique

SCRUM, Kanban, XP (extreme programming)

133.	Qu’est-ce qu’une réunion de revue de projet ?

Un moment formel où l'équipe présente l'avancement du projet

134.	Qu’est-ce qu’un livrable dans un projet ? 

produit à la fin d'une étape (document, maquette etc)

135.	Quels sont les 3 piliers SCRUM ? Définir chacun d’entre eux

Transparence : Visibilité sur le travail, etat du projet etc

Inspection : examiner le produit et les résultats, détecter des problèmes

Adaptation : ajustement son plan par rapport à l'inspection

136.	Qu’est-ce que le DevOps et quel est son objectif principal ?

c'est une méthode de travail qui réunit les développeurs et les équipes techniques pour automatiser et améliorer la création, le test et le déploiement des applications, afin de livrer plus vite et avec moins d’erreurs.

137.	Qu’est-ce que l’intégration continue ? 

c'est une pratique qui consiste a fusionner fréquemment le code des développeurs dans un dépôt central ou il est testé pour détecter les erreurs rapidement

138.	Qu’est-ce que Docker ? Et en quoi est-il utile dans le cadre du DevOps ?

Docker est un outil qui permet de créer, déployer et exécuter des applications dans des conteneurs légers, il garantit que les applications fonctionnent de manière identique dans tous les environnements,

139.	Qu’est-ce qu’un test unitaire ? 

c'est un test automatisé qui vérifie qu’une petite partie d’un programme

140.	Quelle est l'unité de code testée lors d'un test unitaire ?

une fonction, une méthode ou un composant isolé(classe,module etc)

141.	Quelles sont les caractéristiques d'un bon test unitaire ?

Indépendant, rapide, précis, répétable, et facile à comprendre

142.	Qu'est-ce qu'une assertion dans un test unitaire ?

C'est une instruction qui vérifie si le résultat d'une opération ou d'une fonction correspond à la valeur attendue.
 
## English
1)	What does JavaScript enable you to do on a website ?
a.	Add interactive behavior and dynamic content   <----------->
b.	Define the layout and design of web pages
c.	Handle server-side operations

2)	Which programming language is primarily used for server-side web development ?
a.	PHP <------>
b.	JavaScript
c.	HTML

3)	What is the purpose of a web browser ?
a.	To render and display web pages <----->
b.	To execute serve-side code
c.	To manage databases

4)	What is the difference between GET and POST methods in HTTP ?
a.	GET retrieves data from a server, while POST submits data to a server  <---->
b.	GET submits data to a server, while POST retrieves data from a server
c.	GET and POST methods are interchangeable

5)	What is the purpose of version control systems (e.g., Git) in web development ?
a.	To track changes and manage collaborative development <---->
b.	To optimize website loading speed
c.	To handle server-side scripting

6)	What is the purpose of a framework in web development ?
a.	To provide a structured environment for building web applications <----->
b.	To handle network protocols and data transfer
c.	To create visual designs and layouts for websites

7)	What does NoSQL stand for ?
a.	Not Only SQL <---->
b.	Non-Structured Query Language
c.	New Object-Oriented Language

8)	Which of the following is a characteristic of NoSQL databases ?
a.	Strict schema enforcement
b.	Support for complex transactions
c.	Scalability and flexible data models <------>
