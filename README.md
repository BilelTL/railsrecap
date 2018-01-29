<h1 align="center">Ruby on Rails </h1><br>
<p align="center">
	<img alt="Ruby on Rails" src="https://i.imgur.com/4mijNkg.jpg" width="450">
</p> 

## Table des matières
- [Differences](#differences)
- [MVC](#mvc)
- [Routes](#routes)
- [Base de données](#base-de-données)
- [GET POST](#get-post)
- [CRUD](#crud)
- [Les relations dans les BDD](#les-relations-dans-les-bdd)
-[Migration](#migration)


## Differences
 	
Un site **statique** c'est :
* une seule page pour tout le monde (.html)

Un site **dynamique** c'est :
* plusieurs pages (.php ou .html.erb)
* possibilité d'adapter le contenu à l'utilisateur (ex thp , facebook, e commerces )
* necessite un serveur afin de recevoir des requetes (base de données) = plus "lent"

## MVC 

ou **Modèle-vue-contrôleur** et Model-view-controller chez nos amis anglosaxons

Le MVC est un exemple d'architecture logicielle mais il en existe pleins d'autres !! En gros pour faire un site web tu peux utiliser différentes architectures pour ton app
exemple : Une cathedrale peut être Romane ou gothique etc. 

Plus concrètement le MVC est basé sur les relations entre: 
le **modèle** (le coeur de ton site) qui peut contenir, interroger et écrire une base de données;

la **vue** qui retranscrit graphiquement ton site donc notre HTML (ici nom.html.erb);

le **contrôleur** qui va traiter les actions des utilisateurs, il va aussi modifier les données du modèle, il est l'intermédiaire de toutes les interactions entre la vue et la base de données
	
1. Le navigateur envoie une requete (pour acceder au site) via la route (cf Les Routes(link))
	
2. Le contrôleur reçoit et retransmets la requete vers le modèle

3. Le modèle interroge la base de données

4. Le modèle envoie le resultat au controleur qui récupère la vue associée au resultat sous forme page
	
5. Le controleur renvoie la page à l'utilisateur.


## Routes 

Les **routes** permettent de "lire" et "comprendre" les URL
afin de d'indiquer au controleur les bonnes actions
Bref c'est un peu un GPS qui dit au controlleur quel route prendre. 


##Base de données 

Centralise l'information (comme un gros excel avec pleins de feuilles)
<img alt ="GIF papier" src="https://media.giphy.com/media/I77zvnnh76jug/giphy.gif">
*NB: malheuresement ça ne sera pas aussi joli*


## GET POST 

GET quand on va chercher une information
POST quand on va écrire une information


## CRUD (Create Read Update Destroy)

Ce sont des actions de bases pour une ressource (POST GET PUT DELETE)


##Les relations dans les BDD

Dans une base de données nos tables peuvent être liées entre elles. Ces liaisons peuvent avoir un sens particulier.
	*par exemple: un père peut avoir plusieurs enfants mais un enfant ne peut pas avoir plusieurs pères)*.


##Migration 

On crée un fichier contenant les instructions qui servent à modifier notre base de données (ajouter des valeurs ,supprimme des colones etc).

