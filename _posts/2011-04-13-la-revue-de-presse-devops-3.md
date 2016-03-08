---
layout: post
title: La revue de presse devops n°3
published: true
categories: [devops, revue-presse]
---

Bienvenue dans cette 3ème revue de presse devops, avec au sommaire :

-   [Facebook open-source son nouveau data-center](#fb-open-compute)
-   [Il est temps de revoir votre système de monitoring](#monitoring)
-   [Les sorties de la semaine](#sorties)
-   [Quelques liens](#liens)

Facebook open-source son nouveau data-center
--------------------------------------------

La nouvelle de la semaine, c’est bien sur l’annonce de Facebook : [Open Compute](http://opencompute.org/).
Après avoir mis en place leur propre data-center, ils ont décidé de mettre en open-source toutes les specs, que ce soit pour les serveurs (chassis, cartes-mères, etc) ou le data-center en lui-même (électricité, racks, etc). Et annoncent travailler avec différents partenaires (Rackspace, Dell, HP, Intel, AMD, etc) pour continuer à développer le projet.

[Jesse Robbins](http://twitter.com/jesserobbins) fait une [analyse intéressante de cette annonce](http://radar.oreilly.com/2011/04/facebook-open-compute-ops.html) (en anglais) : les constructeurs sont encore obstinés par les serveurs individuels, alors que pour faire du web il faut bosser au niveau de l’infrastructure dans son ensemble, avec des solutions automatisées de reprise sur incident lorsqu’un serveur ne répond plus.

D’où le nombre grandissant d’acteurs qui développent leur propre infrastructure en interne. Et si facebook n’est pas le premier à construire son propre data-center pour ses propres besoins, c’est en revanche le premier à dévoiller son fonctionnement et ses spécifications détaillées. Peut-être que le projet Open Compute permettra d’impliquer les constructeurs dans une logique infrastructure plutôt que serveur.
Et penser infrastructure, en permettant au software de provisionner automatiquement le hardware, c’est penser devops ;-)

Il est temps de revoir votre système de monitoring
--------------------------------------------------

Quelle est la flexibilité de votre système de monitoring actuel ? Est-il est capable de gérer à la fois votre infrastructure, vos services, la partie business de vos applications ?

[R.I. Pienaar](http://www.devco.net/) propose une approche intéressante dans son billet [Monitoring Framework: Composable Architectures](http://www.devco.net/archives/2011/04/04/monitoring_framework_composable_architectures.php) (en anglais) : un système faiblement couplé avec une brique de routage au milieu, qui fait transiter des évènements en JSON.
L’idée est de composer votre système de monitoring comme vous l’entendez, notament en laissant la possibilité aux développeurs de s’intégrer facilement dedans, et de pousser des évènements business depuis les applications.

Dans le même genre, un article titré [Logs Are Streams, Not Files](http://adam.heroku.com/past/2011/4/1/logs_are_streams_not_files/), où pourquoi il faut traiter ses logs comme un flux, plutôt que de les entasser dans un fichier avant de les analyser. Ce qui rejoint l’idée d’un système de monitoring ouvert, où les logs sont traités comme des évènements.
Bref, il y a matière à réflexion.

Les sorties de la semaine
-------------------------

-   [Puppet MCollective 1.1.4](http://docs.puppetlabs.com/mcollective/releasenotes.html#1_1_4) : une nouvelle version de la branche de développement (1.1.x), mais avec une nouvelle fonctionnalité de taille : la possibilité d’écrire des actions dans des langages autre que Ruby.

<!-- -->

-   [Installable Vagrant Boxes](http://jedi.be/blog/2011/03/31/installable-vagrant-boxes/) : Patrick Debois a publier une méthode pour “bundlé” des boxes vagrant avec vagrant integré dans l’executable, plus besoin d’installer vagrant sur la machine, juste besoin d’une JVM et … de JRuby, malheureusement moins frequent. Le but de cet outils est donc de faire rapidement de demos de Vagrant, dans la lignée du dernier meetup !

Quelques liens
--------------

-   <http://www.slideshare.net/arosien/scaling-at-wealthfront>
-   <http://www.kitchensoap.com/2011/04/07/resilience-engineering-part-i/>
-   <http://teddziuba.com/2011/03/devops-scam.html> , une controverse du mouvement devops, article fort interessant, qui explique que le mouvement devops n’est pas clair, en effet, il soulève des problèmes mais ne propose pas (encore) de solutions clair.
-   <http://groups.google.com/group/lille-devops/browse_thread/thread/73880cc9650bc75e> , un petit post de nos amis de Lille, sur le monitoring “L’Hypervision : la Supervision Open Source 2.0” , pour preparer le prochain meetup …

Voilà, c’est tout pour cette semaine !
