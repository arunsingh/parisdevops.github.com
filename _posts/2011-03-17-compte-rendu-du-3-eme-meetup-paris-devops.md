---
layout: post
title: Compte-rendu du 3ème meetup Paris DevOps
published: true
categories: [meetup, compte-rendu]
---

Il y avait **30 personnes** le mercredi 16 mars 2011 vers 19h chez Octo, pour le 3ème meetup du *Paris DevOps*. Au programme de la soirée : **3 présentations, sur RunDeck, Puppet et Vagrant**. Soirée présentations et démonstration d’outils orientés devops, donc, mais avec un accent sur le retour d’expérience.

Après quelques discussions et l’annonce rapide du planning de la soirée, on attaque avec la présentation **RunDeck**, par Bruno et Vincent, de RTL.
RunDeck est un outil d’automatisation des tâches d’administration de serveurs, qui rentre dans la catégorie “ad hoc control tools” (à l’opposé des outils type Puppet et Chef qui sont des “configuration management tools”). En 2 mots il s’agit d’une webapp java (grails) qui permet des définir des jobs qui seront exécutés via SSH sur plusieurs machines.
RunDeck est utilisé à RTL pour déployer des applications web java sur des serveurs d’applications Tomcat, dans des environnements différents : dans un environnement de pre-prod, de manière automatique (via un plugin Jenkins) ; et dans l’environnement de production. Cela permet de faire du “déploiment continu” en utilisant le même outil dans les différents environnements.
La présentation se termine par une démonstration de l’intégration de RunDeck dans la chaîne de déploiment : connexion avec le serveur d’intégration continue Jenkins, connexion avec le “repository manager” Nexus, et déploiement sur Tomcat.

Après une petite pause histoire de profiter du buffet offert par Octo, on reprend avec 2 présentations liées : Puppet et Vagrant.
Samuel commence par présenter **Puppet** de manière assez générique : qu’est ce que c’est, à quoi ça sert, qui s’en sert, quelques exemples de configuration, etc. Donc Puppet est un outil de gestion de configuration de serveurs : on définit des “classes” de serveurs via un DSL, puis on assigne ces classes à nos serveurs. Par exemple les serveurs “appserv-1” et “appserv-2” sont de classe “appserv”, c’est à dire qu’ils doivent avoir une JVM et Tomcat installé (toujours pratique pour des serveurs d’application ;-)
Petit débat sur la lisibilité du DSL de Puppet comme documentation de l’infrastructure, puis on enchaîne sur la présentation **Vagrant** de Fabrice. Vagrant est un outil qui permet de configurer des machines virtuelles VirtualBox, en utilisant Puppet ou Chef. Ici on se focalise sur Puppet, pour faire le lien avec la présentation précédente. En gros l’idée est de générer une VM ayant la même configuration que les serveurs de production, et de l’utiliser en développement afin de réduire le gap entre les différents environnements (32bits vs 64bits, etc).
Theodo a une grosse utilisation de Vagrant, avec des langages de script (ruby, python, php, etc). Cela leur permet d’avoir une VM par client, chacune représentant l’environnement de production dudit client. Une autre utilisation est la mise en place rapide de nouveaux environnements de démonstration, sans avoir à installer de nouveaux serveurs.
Cette idée d’avoir une VM contenant les applications utilisées en production dans le poste de chaque développeur laisse les “java-istes” présents assez perplexe (pour cause de ressources nécessaires à faire tourner un WebSphere ou WebLogic), ce qui ne manquera pas de déclencher un nouveau débat !

22h, on profite que tout le monde soit encore assis pour faire le point sur le *Paris DevOps*. D’abord, open-spaces ou présentations ? Visiblement les présentations ont eu du succès, mais les participants regrettent d’avoir été un peu trop “passif”. A l’avenir, l’idée est d’essayer de faire des présentations plus courtes, et de garder plus de temps pour des questions/débats (pourquoi pas en déplacant les chaises, afin d’avoir une configuration plus favorable à un échange).
Pas vraiment de décision pour la prochaine date. Un délai de 1 ou 2 mois entre chaque meetup fait l’unanimité. Bref RDV en avril/mai.

22h30, fin “officielle” du meetup, c’est là que la partie la plus intéressante commence : les discussions entre les participants, autour du buffet. Puis les gens partent progressivement, les derniers finissant tard dans la nuit…

Un grand merci à Octo pour les locaux, aux organisateurs, orateurs et participants. RDV dans 1 ou 2 mois pour le prochain meetup !

Les slides des présentations sont disponibles sur la page des [meetups](/meetups.html#meetup-3).
