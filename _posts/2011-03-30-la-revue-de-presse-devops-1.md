---
layout: post
title: La revue de presse devops n°1
published: true
categories: [devops, revue-presse]
---

Donc voilà, on va essayer de faire une **revue de presse hebdomadaire**, sur le thème **devops**. Et le grand jour de sortie sera le **mercredi**.
Et là je vous vois venir, “pourquoi le mercredi ?”. Et bien tout simplement parce qu’on a commencé à organiser les [meetups](/meetups.html) du *Paris DevOps* les mercredi (mais pas tous les mercredi hein), donc à partir de maintenant le mercredi c’est le jour devops ;-)

Au minimum on va essayer de noter les articles qui nous ont semblé intéressants, les sorties d’outils catégorisés “devops”, etc. Et si on est en forme, vous aurez le droit à quelques commentaires voir pourquoi pas une analyse plus poussée par-ci ou par-là.

Allez, on envoie la première !

-   [Un SI propre avec iTop, RunDeck, Puppet, FusionInventory](#si)
-   [Frameworks maison de monitoring applicatif](#monitoring)
-   [Utilisation de Vagrant dans une équipe](#vagrant)
-   [Donner du style à Puppet](#puppet)
-   [Nouvelle version de Foreman : 0.2](#foreman)
-   [Le troll devops de la semaine](#troll)

Un SI propre avec iTop, RunDeck, Puppet, FusionInventory
--------------------------------------------------------

[Asyd](http://blog.asyd.net/) nous présente sa vision d’un SI “propre”, en mettant en place les différents types d’outils qu’on voit habituellement dans des déploiements devops : une CMDB (Configuration Management DataBase), un outil de gestion de la configuration, un outil de gestion des jobs, et enfin un outil de gestion d’inventaire.
Que des outils open-source, qui ont assez de points d’extension pour communiquer les uns avec les autres.
Bref, un article à lire ! <http://blog.asyd.net/2011/03/un-si-propre-avec-itop-rundeck-puppet-fusioninventory/>

Frameworks maison de monitoring applicatif
------------------------------------------

Suite au très bon post d’ [Etsy](http://codeascraft.etsy.com/) sur leur solution interne de monitoring applicatif [Measure Anything, Measure Everything](http://codeascraft.etsy.com/2011/02/15/measure-anything-measure-everything/), il semble que pas mal de personnes s’intéressent à la mise en place de frameworks maison de monitoring applicatif assez poussés :

-   [Hi My Name is John…](http://railstips.org/blog/archives/2011/03/21/hi-my-name-is-john/) (…and I am addicted to analytics)
-   [Thinking about monitoring frameworks](http://www.devco.net/archives/2011/03/19/thinking_about_monitoring_frameworks.php) et la suite [Monitoring Framework: Event Correlation](http://www.devco.net/archives/2011/03/25/monitoring_framework_event_correlation.php)
-   Et nous également, mais on a pas encore écrit de billet sur le sujet ;-)

L’idée à retenir, c’est un framework très simple à utiliser, et très léger, qui fonctionne en mode asynchrone. Cela permet d’enregistrer beaucoup d’évènements, et ensuite de monter une solution de graph pour visualiser ce qui se passe en temps réel. Puis un petit dashboard par dessus tout ça, quelques alertes en cas de dépassement de seuils, et vous serez déjà beaucoup plus serein quand au fonctionnement de votre application en production.
Attention il ne s’agit pas de reprendre ce qui existe déjà côté ops (cpu, mémoire, etc), mais bien de données applicatives (logins, achats, commentaires, clicks sur certains bouttons, etc). Quelque chose qui puisse faire référence à la fois pour les devs, les ops, mais aussi les gens du business (le client). Mais c’est un sujet qui nécessiterai un meetup ;-)

Utilisation de Vagrant dans une équipe (par Patrick Debois)
-----------------------------------------------------------

Vous le savez tous, Patrick Debois c’est un peu le papa de devops (oui le petit devops à un papa, mais pas de maman. C’est une histoire pour un prochain post ![]()
Donc quand Patrick nous présente son utilisation de "Vagrant":http://vagrantup.com/, couplé au fait qu'on viens de faire une "présentation Vagrant au dernier meetup":/meetups.html#meetup-3... et bien ça nous a semblé intéressant )
L’article en anglais : <http://jedi.be/blog/2011/03/28/using-vagrant-as-a-team/>

La majeure partie de l’article est consacrée à la mise en place de Vagrant, et l’utilisation d’un “provisioner”. Reste le retour d’expérience, tout à la fin du billet : dans l’équipe de développeurs qui utilise Vagrant, tous les devs ne participent pas à l’écriture de recettes/manifests. Cette tâche est uniquement accomplie par quelques devs, plus orientés ops. Peut-être une question de temps ?

Autre remarque plus “étonnante” : la panoplie de technologies différentes utilisées dans le même projet : nodejs, grails, rails, perl, redis, mysql, hadoop. Rien que ça ! Ca mériterait un billet pour détailler les raisons d’utilisation d’autant de technos différentes (en tout cas moi ça m’intrigue…)

Donner du style à Puppet
------------------------

Les p’tits gars de [Puppet Labs](http://www.puppetlabs.com/) nous ont pondu une convention de style pour écrire des modules/classes/ressources pour Puppet :

-   [L’annonce sur le blog de Puppet Labs](http://www.puppetlabs.com/blog/a-question-of-style/)
-   [La convention de style](http://docs.puppetlabs.com/guides/style_guide.html)

Un des objectifs de Puppet étant de documenter votre infrastructure, l’idée d’avoir un style commun prend beaucoup de sens. A défaut d’être utilisé partout (on sait comment ça marche), ça peut déjà vous donner des idées en interne : est-ce que vos modules sont propre ? Ne serait-il pas temps d’en profiter pour faire un petit ménage de printemps ? ;-)

Nouvelle version de Foreman : 0.2
---------------------------------

Tant qu’on est dans l’univers Puppet : [Foreman](http://theforeman.org/) viens de sortir en version 0.2, qui est d’après les développeurs “une version majeure”.
L’objectif de Foreman est de servir de point d’entrée dans la gestion des serveurs, notamment en fournissant une interface web à Puppet, mais également en gérant le provisioning avant l’entrée en scène de Puppet.
Les principales nouveautés de cette version : nouveau look & feel, API REST étendue, support du nouveau format des rapports Puppet, etc.

-   [L’annonce de la version 0.2](http://theforeman.org/blogs/show/14)
-   [Les ‘release notes’ complètes](http://theforeman.org/projects/foreman/wiki/ReleaseNotes)

Le troll devops de la semaine
-----------------------------

Pour finir en beauté !

-   Le billet d’origine : [Devops Is a Poorly Executed Scam](http://teddziuba.com/2011/03/devops-scam.html)
-   La réponse : [Devops Isn’t A Methodology](http://morethanseven.net/2011/03/26/Devops-isnt-a-methodology.html)

Pour ma part, je ne retiendrais qu’une seule chose : *“The Devops people have a bit of traction, and they’re failing to capitalize on it. You’ve got a good thing going here, profit from that shit. Books, training, conferences, the whole bit. Get down to it.”*
C’est donc officiel, à partir de maintenant l’accès aux meetups sera payant ! 5 000 euros la soirée, c’est raisonnable, non ? ;-)

Et voilà, c’est fini pour cette semaine, RDV mercredi prochain. Et pensez à vous abonner au [flux RSS](http://feeds.feedburner.com/parisdevops) du blog !
