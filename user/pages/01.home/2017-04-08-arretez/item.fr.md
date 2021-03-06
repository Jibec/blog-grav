---
title: 'Arrêtez de traduire !'
date: '2017-04-08'
taxonomy:
    category:
        - Régionalisation
    tag:
        - fedora-fr
        - traduction
        - planet-libre
author: 'Jean-Baptiste Holcroft'
---

Amis de la langue et du logiciel libre, quand vous êtes sur une traduction et qu’une phrase vous semble étrange, arrêtez-vous, posez des questions et demandez des corrections. Voici un cas d’école sur ce projet passionnant qu’est YunoHost.

Arriver à 100 % de traduction n’a aucun sens si ce que voit l’utilisateur n’est pas bien écrit, ou s’il y a des bugs dans les logiciels que vous ne signalez pas.

Depuis peu, Bram, un des développeurs a [développé le nécessaire](https://github.com/YunoHost/apps/pull/123) pour pouvoir traduire de façon centralisée la description et les questions posées par les applications installables par l’utilisateur sur son serveur [YunoHost](http://yunohost.org) . Debian fait la même chose avec [ddtp]() et [debconf](https://www.debian.org/international/french/po-debconf) (respectivement la description des paquets et les questions posées à l’utilisateur).

J’ai remarqué plusieurs choses étranges, des [phrases vides](https://dev.yunohost.org/issues/888), des [phrases sources écrites en français](https://dev.yunohost.org/issues/887) au lieu de l’anglais, des [phrases perfectibles](https://dev.yunohost.org/issues/895), énormément de redondance et… un [bug supposé dans Weblate](https://github.com/WeblateOrg/weblate/issues/1429).

Après coup, quand je vois ce qui est à traduire, il y a un souci supplémentaire. Avoir 127 phrases à traduire « Choose a domain for %%% » où %%% correspond au nom du paquet YunoHost, ce n’est pas utile à traduire ! Et ce n’est que le début… 20 phrases à traduire « Choose a domain name for %%% »… Cela se poursuit avec 136 phrases « Choose a path %%% » et 22 phrases pour le choix de l’administrateur, 74 pour le caractère public ou privé de l’application. Autant traduire n’est pas compliqué avec un peu de motivation et de rigueur, autant quand le contenu est fortement redondant on a l’impression de se transformer en robot…

Voici la demande d’évolution que j’ai [formulée sur l’outil de suivi](https://dev.yunohost.org/issues/896).

Deux pistes me semblent possibles :

* proposer des méthodes aux paquets pour les questions génériques (complexe ?),
* ajouter une règle de contrôle automatique pour éviter que les applications renseignent leur nom dans les questions pour au moins réduire les phrases proches.

La conclusion de tout ceci, c’est qu’il faut aller plus loin dans nos travaux que simplement traduire, il faut coconstruire le logiciel avec les développeurs, dès qu’une phrase nous paraît étrange, il faut s’interroger sur la cause, voire la pertinence de la phrase que vous traduisez. Notre temps de traducteur est précieux (tout comme celui de chaque contributeur), il faut poser la question au mainteneur du projet et obtenir une correction.
