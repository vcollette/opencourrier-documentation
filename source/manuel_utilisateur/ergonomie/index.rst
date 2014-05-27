.. _ergonomie:

#########
Ergonomie
#########

Cette partie vise à présenter l'ergonomie du logiciel c'est-à-dire à décrire la
connexion à l'application, la structure de l'application, la navigation et
l'utilisation du menu, ainsi que la présentation et la description des
principaux icônes. Cette rubrique peut s'appliquer à toute application métier
développée avec OpenMairie.


.. contents::


*************************************
Connexion, déconnexion et permissions
*************************************


Connexion
#########

.. note::

   Pour réaliser cette étape, votre administrateur doit vous fournir une
   adresse Web pour accéder à l'application, un identifiant utilisateur ainsi
   qu'un mot de passe. Ces éléments auront été préalablement configuré dans
   le logiciel.


==============
Navigateur Web
==============

L'application est accessible via un navigateur Web, pour y accéder il faut
saisir l'adresse Web fournie par votre administrateur dans la barre d'adresse.

.. image:: opencourrier--ergonomie-navigateur.png


.. note::

    Ce logiciel est développé principalement sous le navigateur Mozilla Firefox,
    il est donc conseillé d'utiliser ce navigateur pour une efficacité optimale.


====================================
Saisie des informations de connexion
====================================

Cet écran de connexion est composé de deux zones de texte et d'un bouton.

.. image:: opencourrier--ergonomie-formulaire-connexion.png

Dans l'écran d'identification, il faut saisir son identifiant et son mot de
passe puis cliquer sur le bouton « Se connecter ».

.. note::

    L'identifiant et le mot de passe doivent être saisis en respectant la
    casse, c'est-à-dire les minuscules et majuscules.


Connexion échouée
-----------------

Si les identifiants saisis sont incorrects, un message d'erreur apparaît et il
faut ressaisir les informations de connexion.

.. image:: opencourrier--ergonomie-connexion-message-erreur.png


Connexion réussie
-----------------

Si les identifiants sont corrects, vous êtes redirigé vers la page demandée sur
laquelle le message suivant doit d'afficher.

.. image:: opencourrier--ergonomie-connexion-message-ok.png




Déconnexion
###########

Pour une question de sécurité évidente, il est important de se déconnecter de
l'application pour qu'un autre utilisateur ne puisse pas accéder au logiciel
via votre compte utilisateur.

L'action "Déconnexion" est disponible à tout moment dans les actions
personnelles en haut à droite de l'écran.

.. image:: opencourrier--ergonomie-deconnexion-action.png


Une fois déconnecté, c'est le formulaire de donnexion qui s'affiche avec un
message expliquant la réussite de la déconnexion.

.. image:: opencourrier--ergonomie-deconnexion-message-ok.png




Les droits et profils des utilisateurs
######################################

Les droits et profils des utilisateurs permettent de limiter l'accès aux
informations et aux actions uniquement aux personnes autorisées. Chaque
utilisateur est associé à un profil. Le profil correspond à un ensemble
de permissions de l'utilisateur. Les profils sont hiérarchiques et listés de façon
croissante, c'est à dire que les permissions d'un profil son valable pour les
suivants, par défaut il existe cinq profils :

#. Consultation :
    peut visualiser les courriers arrivées/départs, les courriers archivés et les tâches non soldées de son service, ainsi que les courriers recherchés de chaque service.
#. Utilisateur limité :
    peut modifier les tâches non soldées de son service.
#. Utilisateur :
    peut ajouter ou modifier les courriers arrivées/départs de son service et les objets liés à celui-ci. Il peut aussi paramétrer l'application : ajouter/modifier/supprimer les émetteurs/destinataires, la bible, les civilités, les types de correspondants et les courriers types.
#. Super utilisateur :
    peut faire les traitements concernant le registre et l'archivage, les exports des éditions et des requêtes mémorisées, le paramétrage des services, des états, des sous-états et des lettres type.
#. Administrateur :
    peut paramétrer les collectivités, les paramètres de l'application, les profils, les droits, les utilisateurs, les widgets, importer des tables et utiliser le générateur.

Chaque page de l'application est associée à un profil. Pour chaque accès à une
page, l'application vérifie si l'utilisateur a un profil supérieur ou égal au
profil de la page consultée, si c'est le cas l'utilisateur à donc le droit
d'accéder aux informations.

Les profils ainsi que leurs permissions associées sont modifiables par
l'administrateur.


******************
Ergonomie générale
******************

L'application, sur la grande majorité des écrans, conserve ses composants
disposés exactement au même endroit. Nous allons décrire ici le fonctionnement
et l'objectif de chacun de ces composants. Cette structuration de l'application
permet donc à l’utilisateur de toujours trouver les outils au même endroit
et de se repérer rapidement.

.. image:: opencourrier--ergonomie-generale-detail.png

.. note::

    Les actions et affichages de l'application diffèrent en fonction du profil
    de l'utilisateur. Il se peut donc que dans les paragraphes qui suivent
    des actions soient décrites et n'apparaissent pas sur votre interface
    ou inversement que des actions ne soient pas décrites mais apparaissent sur
    votre interface.

Le logo
#######

C'est le logo de l'application, il vous permet en un seul clic de revenir
rapidement au tableau de bord.


Les actions personnelles
########################

Cet élément affiche plusieurs informations importantes.

La première information est l'identifiant de l'utilisateur actuellement
connecté ce qui permet de savoir à tout moment si nous sommes bien connectés
et avec quel utilisateur. Ensuite est noté le nom de la collectivité sur
laquelle nous sommes en train de travailler. En mode multi, une action est
disponible sur cette information pour permettre de changer de collectivité.
Ensuite la liste sur laquelle nous sommes en train de travailler, une action
est disponible sur cette information pour permettre de changer de liste.
Enfin l'action pour permettre de changer de mot de passe et pour se déconnecter
sont disponibles en permanence.


Les raccourcis
##############

Cet élément permet d'afficher des raccourcis vers des écrans auxquels nous
avons besoin d'accéder très souvent. Par exemple, ici nous avons un 
raccourci direct vers le tableau de bord.


Le menu
#######

Cet élément permet de classer les différents écrans de l'application en
rubriques. En cliquant sur l'entête de rubrique, nous accédons à la liste des
écrans auxquels nous avons accès dans cette rubrique.

Le nombre de rubriques disponibles dans le menu peut varier en fonction du
profil des utilisateurs. Un utilisateur ayant le profil Consultation n'aura
probablement pas accès aux six rubriques présentes sur cette capture. 



Les actions globales
####################

Cet élément permet d'afficher en permanence le numéro de version du logiciel.
Ensuite les différentes actions sont des liens vers le site officiel du
logiciel ou vers la documentation.



*************************
Ergonomie des formulaires
*************************

De manière générale, il y a une règle simple dans les applicatifs openMairie :
on accède d'abord à un listing d'éléments puis depuis ce listing on peut
ajouter un nouvel élément ou modifier un élément existant en accédant au
formulaire dédié à cet élément.

Les listings
############

Un listing est un tableau qui liste des éléments récapitulant des informations
permettant d'identifier un élément parmi les autres.

.. image:: opencourrier--ergonomie-listing.png


===========
Les actions
===========

En haut à gauche
----------------

* Ajouter : cette action représentée par un plus permet d'accéder au formulaire
  de création d'un élément.
  
  |icone-ajouter|

* Autre : il peut y avoir d'autres actions positionnées ici qui représentent
  des actions que l'on peut faire sur un lot d'éléments par exemple.


A gauche devant chaque élément
------------------------------

* Modifier : cette action permet d'accéder au formulaire de modification
  d'un élément.

* Supprimer : cette action permet d'accéder au formulaire de suppression
  d'un élément.

* Autre : il peut y avoir d'autres actions positionnées ici qui permettent
  d'effectuer des actions rapides sur l'élément.


Sur l'élément
-------------

* Modifier : cette action permet d'accéder au formulaire de modification
  d'un élément.


Divers
------

* Afficher les éléments expirés : sur les élements qui possèdent une date de
  validité, par défaut les éléments qui sont dans le passé n'apparaissent pas,
  il est nécessaire de cliquer sur cette action pour les faire apparaître.
  L'action se situe au dessus du tableau.

* Imprimer le listing en PDF : sur les éléments pour lesquels l'édition existe
  une action représentée par une imprimante permet de télécharger un pdf qui
  reflète le contenu du listing sans aucun filtre de recherche. L'action se
  situe au dessus du tableau.
  
  |icone-edition-pdf|


Les formulaires
###############

Un formulaire dans cet applicatif peut soit être soit d'ajout, soit de 
modification, soit de suppression. 

Voici l'exemple d'un formulaire en mode modification.

.. image:: opencourrier--ergonomie-formulaire-modifier.png


Les actions de formulaires :

* Modifier : cette action permet d'accéder au formulaire de
  l'élément en mode modification. Une fois le formulaire de modification validé
  alors un bouton retour nous permet de revenir au listing des éléments.

* Supprimer : cette action permet d'accéder au formulaire de
  l'élément en mode suppression. Une fois le formulaire de suppression validé
  alors un bouton retour nous permet de revenir au listing des éléments.



===========
Les onglets
===========

Sur le formulaire d'un élément, il peut apparaître plusieurs onglets qui
correspondent à des éléments liés à l'élément en cours. Un onglet présente un
listing de ces éléments liés avec des actions qui permettent également d'accéder
à des formulaires sur ces éléments liés.

Par exemple sur l'image suivante, on peut voir sur le "profil" un onglet
"tableau de bord" qui liste les tableaux de bord liés au profil utilisateur.

.. image:: opencourrier--ergonomie-formulaire-onglet-listing.png


.. |icone-edition-pdf| image:: opencourrier--icone-edition-pdf.png
.. |icone-ajouter| image:: opencourrier--icone-ajouter.png
