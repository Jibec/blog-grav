---
title: 'Comment Zanata est-il arrivé dans la communauté Fedora ?'
date: '2016-09-02'
taxonomy:
    category:
        - Régionalisation
    tag:
        - fedora-fr
        - flock
        - planet-libre
author: 'Jean-Baptiste Holcroft'
---

Le projet de plate-forme de traduction débuta vers 2008, le nom interne était Fly et rendu open-source probablement vers cette année, puis sous le nom de [Zanata](http://zanata.org) vers 2010.
 
À cette époque, [Transifex](https://www.transifex.com) était encore open-source mais les besoins internes de [Red Hat](http://redhat.com) n’était pas vraiment couvert par Transifex et visiblement les deux projets prenaient des orientations différentes.
La branche asiatique de Red Hat qui menait le projet de plate-forme de traduction a essayé d’inciter les équipes Red Hat à utiliser leur outil en lieu et place de Transifex, mais cela s’est heurté à une résistance importante, notamment des équipes américaines.

À cette époque, Red Hat a tenté de recruter le producteur de Transifex mais apparemment pas pour s’assure que l’outil Transifex resterait open-source, mais pour ses compétences techniques.

Quand le logiciel utilisé par Transifex a cessé d’être publié sous une licence open-source et que cela a été officialisé. Le code sous-jacent avait déjà bien évolué depuis la dernière publication de sources. Il n’était déjà plus possible d’envisager de lancer une instance de Transifex facilement et de migrer les données. La communauté était face à un dilemme.

Conformément à ses choix d’indépendance technologique, Red Hat souhaite avoir une indépendance à long-terme et a choisi de miser massivement sur Zanata plutôt sur de collaborer avec Transifex.   
Le transfert a été massif et unilatéral, mais il n’est probablement pas vraiment terminé car même en interne du projet Fedora de nombreux développeurs n’y étaient pas favorables.

C’est ainsi qu’un outil dédié aux besoins interne d’outillage Red Hat est désormais utilisé pour la traduction de plusieurs plates-formes.

Je regrette qu’il n’y ait pas eu de période transitoire permettant de trouver une solution pérenne permettant d’analyser calmement quelle est la meilleure option de sortie pour répondre aux besoins de pilotage et de coordination de centaines de personnes plutôt que de se jeter par défaut sur cet outil.

Aucun contributeur que j’ai rencontré ne m’a transmis un retour d’expérience positif tant sur le processus de décision, sur le processus de migration et sur le nouvel outil. Quelques anciens m’ont également fait part de leur sensation d’avoir perdu beaucoup, tant en termes de pilotage que de contribution.

On m’a également indiqué que c’est probablement l’un des rares, voire peut-être le seul outil développé en Java dans Red Hat…
