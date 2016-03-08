---
layout: post
title: La revue de presse devops n°2
published: true
categories: [devops, revue-presse]
---

Ah enfin mercredi, et la tant attendue revue de presse devops !
Au sommaire de cette 2ème édition :

-   [Date du prochain meetup : 4 mai](#meetup)
-   [Les résultats de l’enquête devops 2011](#enquete)
-   [Slides de la présentation devops à la conférence MIX-IT](#mixit)
-   [Vidéo de la conférence ‘Moving Fast at Scale’](#etsy)
-   [Utiliser Chef pour gérer des postes client](#chef)
-   [La vérité sur devops](#verite)
-   [La chanson devops](#imagine)
-   [La minute people](#people)
-   [Le teasing de la semaine](#teasing)
-   [Les citations de la semaine](#citations)

Date du prochain meetup : 4 mai
-------------------------------

On commence par un peu d’auto-promo : la date du prochain meetup du *Paris DevOps* à été annoncée hier, il s’agit du mercredi 4 mai.
Je vous laisse lire [l’annonce officielle](/blog/2011/04/05/prochain-meetup-le-mercredi-4-mai.html), puis filez vous [inscrire](http://lanyrd.com/2011/paris-devops-meetup-4/) ! Vous pourrez revenir lire la revue de presse plus tard…

Les résultats de l’enquête devops 2011
--------------------------------------

[Replay Solutions](http://replaysolutions.com/) viens de publier [les résultats de l’enquête devops](http://replaysolutions.com/2011-DevOpsSurveyResults) qu’ils ont réalisé en janvier 2011, avec 1 200 participants provenant de diverses entreprises.

D’après [le communiqué de presse](http://replaysolutions.com/company/news/59), la moitié des répondants ont un “process devops” actif : 25% avec une équipe dédiée, et 25% avec une équipe partagée. Sachant que les grosses entreprises ont plutôt tendance à avoir des équipes devops dédiée, et les petites entreprises des équipes partagées.
D’autre part, 60% disent utiliser des méthodes agiles. Devops, dans la continuité de l’agilité…
Autre point intéressant : 90% des répondants estiment que les outils sont “importants” ou “plutôt importants” au succès de devops. Quand on vous dit que devops c’est culture et outils…
Enfin, les 3 bénéfices majeurs de devops : réduction du temps pour corriger un bug (en production), meilleure communication, mises à jour plus faciles.

Les résultats de l’enquête (format PDF) :

-   [avec analyse et des graphs](http://replaysolutions.com/downloads/DevOps-2011-TrendsOverview.pdf)
-   [resultats ‘brut’](http://replaysolutions.com/downloads/DevOps-2011-TrendsSurvey.pdf)

Slides de la présentation devops à la conférence MIX-IT
-------------------------------------------------------

La conférence [MIX-IT](http://www.mix-it.fr/) a eu lieu hier à Lyon, et au programme il y avait entre autres une [présentation sur le mouvement devops](http://www.mix-it.fr/sessions#session_39003) par [Gildas Le Nadan](http://www.mix-it.fr/speakers#speaker_40007).
[Les slides sont disponibles](http://devops.fr/mixit/slides.pdf) (allez-y, pour une fois c’est en français ;-)

Vidéo de la conférence “Moving Fast at Scale”
---------------------------------------------

Une autre conférence, mais un peu plus loin cette fois-ci (USA) : [Moving Fast at Scale](http://codeascraft.etsy.com/2011/03/19/moving-fast-at-scale-slides-and-reprise/), organisée par [Etsy](http://codeascraft.etsy.com). [La vidéo de la conférence est disponible](http://livestre.am/GXi0), mais attention c’est long : 2 heures ! (en anglais). Au programme :

-   [Scaling Startups](http://www.slideshare.net/chaddickerson/scaling-startups/)
-   [Déploiement continu](http://www.slideshare.net/kellan/continuous-deployment-7300057)
-   [‘Deployinator’](http://www.slideshare.net/kastner1/deployinator-turning-the-fear-into-the-fear) (outil de déploiement interne)
-   [Metrics-driven Development](http://www.slideshare.net/mikebrittain/metrics-driven-engineering-at-etsy) (monitoring)

Utiliser Chef pour gérer des postes client
------------------------------------------

Les outils de “gestion de configuration” type Puppet/Chef/Cfengine sont généralement utilisés pour gérer des serveurs. Mais pourquoi ne pas les utiliser pour gérer des postes clients ? Après tout, [Google utilise bien Puppet pour des milliers de desktop Mac](http://www.redmonk.com/cote/2008/06/11/puppet-at-google-redmonk-radio-episode-48/).

Voilà donc un billet sous forme de tutoriel qui explique simplement comment utiliser Chef pour gérer 3 Macbook : [Managing My Workstations with Chef](http://jtimberman.posterous.com/managing-my-workstations-with-chef) (en anglais).

La vérité sur devops
--------------------

Encore un billet de blog à la recherche de la définition ultime de “devops” : [The Truth about DevOps](http://lunatractor.com/2011/03/31/the-truth-about-devops/) (en anglais). Il semble que les gens passent plus de temps à essayer de définir devops qu’autre chose ;-)
Bref, ici l’auteur définit devops par les 4 points suivants :

-   les développeurs s’intéressent / s’investissent dans le déploiement applicatif et l’environnement de production
-   les admin système s’intéressent / s’investissent dans le développement de nouvelles fonctionnalités
-   les développeurs ont accès à l’environnement de production, au système de monitoring et aux process de déploiement
-   les admin système sont impliqués dans le développement des nouvelles fonctionnalités dès le départ

L’auteur écrit en anglais “to care about”, je pense vraiment que le bon mot est “s’investir” : les devs s’investissent dans le travail des ops, et inversement.
Dommage qu’il n’ait pas mentionné la finalité de devops (gestion plus fluide/souple de l’infrastructure et des applications, meilleure “expérience utilisateur”)

La chanson devops
-----------------

Oui on sait, on est un peu en retard. Mais comme on a oublié de vous le mettre dans la revue de presse précédente… Bref, voilà un énième massacre de “Imagine” de John Lennon. Mais bon c’est sur le thème devops, donc on lui pardonne !

-   [Imagine DevOps](http://www.youtube.com/watch?v=iYLxw6OsZug) (vidéo de la chanson sur youtube)

A voir en mettant le son à fond dans le bureau, pour attirer vos collègues !
Remarque : *Paris DevOps* décline toute responsabilité en cas de problème avec vos collègues suite au visionnage de cette vidéo ;-)

La minute people
----------------

La communauté Java à eu droit à sa “minute people” cette semaine avec [l’embauche de James Gosling chez Google](http://nighthacks.com/roller/jag/entry/next_step_on_the_road), maintenant c’est au tour de la communauté devops !

[John Willis](http://www.johnmwillis.com/about/) (l’une des références devops) à annoncé qu’il quittait [Opscode](http://www.opscode.com/) (la boite derrière [Chef](http://opscode.com/chef/)) pour [DTO Solutions](http://www.dtosolutions.com/) (la boite derrière [ControlTier](http://controltier.org/) et [RunDeck](http://rundeck.org/)).
Rien de très étonnant finalement, vu que le boss de DTO Solutions est [Damon Edwards](http://twitter.com/damonedwards), qui n’est autre que le [co-animateur](http://devopscafe.org/display/ShowImage?imageUrl=/storage/IMG_2540.jpg) du podcast [DevOps Cafe](http://devopscafe.org/) avec [John](http://twitter.com/botchagalupe). Bref, devops c’est un peu comme Dallas ;-)
[L’annonce sur Twitter](http://twitter.com/botchagalupe/status/53973034335342592) (en anglais)

J’en profite quand même pour vous inciter à écouter le podcast [DevOps Cafe](http://devopscafe.org/), histoire que cette section “minute people” ne soit pas totalement inutile !

Le teasing de la semaine
------------------------

Le teasing devops de la semaine, c’est [DevOps as a service](http://doaas.com/).
Comme c’est du teasing, on a pas plus d’informations à vous donner, mais vous pouvez jouer avec “whois” pour en savoir plus (ça, c’est l’exercice de la semaine ;-)

Les citations de la semaine
---------------------------

-   [`puppetmasterd":http://twitter.com/puppetmasterd : ""_#devops is the belief that sysadmins deserve and should always use the best tools, and that most of those tools look like dev tools_"":http://twitter.com/puppetmasterd/status/53534064682074114
    * "`DEVOPS\_BORAT](http://twitter.com/DEVOPS_BORAT) : “”*Is true DevOps is first culture then technology. Is why in startup we interview candidate in literature, classical music and ballet.*“”:http://twitter.com/DEVOPS\_BORAT/statuses/55312363431276545

Voilà, c’est tout pour cette semaine !
