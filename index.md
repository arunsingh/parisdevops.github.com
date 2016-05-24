---
layout: page
title: Présentation
---

*Paris DevOps* est un groupe de personnes qui partagent la culture [DevOps](http://devops.fr/) et se réunissent régulièrement sur Paris en organisant des [meetups](/meetups.html) : open-spaces, présentations, retours d’expérience, discussions, etc. [Rejoignez-nous !](/communaute.html)

Les dernières infos
-------------------

<ul class="toc">
    {% for post in site.posts limit:3 %}
        <li>
            {{ post.date | date: "%Y/%m/%d" }} : <a href="{{ post.url }}">{{ post.title }}</a>
        </li>
    {% endfor %}

    <li> <a href="/blog">Voir tous les billets</a></li>
</ul>

Les meetups
-----------

-   Prochain meetup : [mardi 7 juin 2016](/meetups.html#meetup-43)
-   Précédent meetup : [mardi 10 mai 2016](/meetups.html#meetup-42)

[Voir tous les meetups](/meetups.html)

<script src="http://widgets.twimg.com/j/2/widget.js"></script>
<script>
    new TWTR.Widget({
        version: 2,
        type: ‘profile’,
        rpp: 3,
        interval: 6000,
        width: ‘auto’,
        height: 300,
        theme: {
        shell: {
        background: ‘\#ffffff’,
        color: ‘\#000000’
        },
        tweets: {
        background: ‘\#ffffff’,
        color: ‘\#000000’,
        links: ‘\#0045b3’
        }
        },
        features: {
        scrollbar: false,
        loop: false,
        live: false,
        hashtags: true,
        timestamp: true,
        avatars: false,
        behavior: ‘all’
        }
    }).render().setUser(‘parisdevops’).start();
</script>
