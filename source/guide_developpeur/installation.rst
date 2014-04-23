.. _installation:

############
Installation
############

**********
Pré-requis
**********

Vous devez avoir installer :

- un serveur web (apache, ...)
- PHP
- le moteur de base de donnees MySQL


Sous windows, il est facuile de trouver de la documentation pour l'installation
de ces éléments en utilisant wamp (http://www.wampserver.com/) ou easyphp 
(http://easyphp.fr/) par exemple.

Sous Linux, il est facile de trouver de la documentation pour l'installation de
ces éléments sur votre distribution.


***********
Déploiement
***********

Installation des fichiers de l'applicatif
=========================================

Télécharger l'archive zip
-------------------------

https://adullact.net/frs/?group_id=297


Décompresser l'archive zip dans le répertoire de votre serveur web
------------------------------------------------------------------

Exemple sous windows dans wamp : wamp/www/opencourrier
Exemple sous linux avec debian : /var/www/opencourrier


Création et initialisation de la base de données
================================================

Créer la base de données
------------------------

Par défaut la base de données s'appelle opencourrier.


Initialiser la base de données
------------------------------

Il faut initialiser les tables, les séquences et données de paramétrage :

- data/mysql/init.sql
- data/mysql/init_metier.sql


Initialiser un jeu de données de démonstration (optionnel)
----------------------------------------------------------

Il est possible d'initialiser un jeu de données pour tester l'applicatif avec
des données de démonstration :

- data/mysql/init_data.sql


Configuration de l'applicatif
=============================

Positionner les permissions nécessaires au serveur web
------------------------------------------------------

Exemple sous linux avec debian : chown -R www-data:www-data /var/www/opencourrier


Configuration de la connexion à la base de données
--------------------------------------------------

La configuration se fait dans le fichier `dyn/database.inc.php` :

.. code-block:: php

   // MySQL
   $conn[1] = array(
        "Courrier MySQL",
        "mysql",
        "",
        "root", // Remplacer ici le login de l'utilisateur MySQL
        "", // Remplacer ici le mot de passe de l'utilisateur MySQL
        "",
        "localhost", 
        "",
        "",
        "opencourrier", // Remplacer ici le nom de la base de données
        "AAAA-MM-JJ",
        "",
        ""
   );


*************************
Connexion à l'application
*************************

Ouverture dans le navigateur
============================

http://localhost/opencourrier/


Login
=====

* Utilisateur "administrateur" : 
   - identifiant : admin
   - mot de passe : admin
* Utilisateur "démonstration" (si le fichier d'initalisation du jeu de données de démonstration a été appliqué) :
   - identifiant : demo
   - mot de passe : demo

Le message de bienvenue doit être affiché "Votre session est maintenant ouverte."


***************
En cas d'erreur
***************

Activer le mode debug
=====================

Il est possible d'activer le mode debug pour visualiser les messages d'erreur
détaillés. Dans le fichier `dyn/debug.inc.php`, il faut commenter le mode
production et décommenter le mode debug.

Mode production :

.. code-block:: php

   //define('DEBUG', VERBOSE_MODE);
   //define('DEBUG', DEBUG_MODE);
   define('DEBUG', PRODUCTION_MODE); 

Mode debug :

.. code-block:: php

   //define('DEBUG', VERBOSE_MODE);
   define('DEBUG', DEBUG_MODE);
   //define('DEBUG', PRODUCTION_MODE); 

