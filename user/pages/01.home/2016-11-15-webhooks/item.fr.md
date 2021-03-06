---
title: 'Comment avons-nous traduit Webhooks ?'
date: '2016-11-16'
taxonomy:
    category:
        - Régionalisation
    tag:
        - fedora-fr
        - traduction
        - planet-libre
author: 'Jean-Baptiste Holcroft'
---

Pendant notre traduction de la future version de l’outil Zanata, nous avons choisi de traduire « Webhooks » en « URL de rappel » et je vais vous écrire pourquoi et comment.

Nos amis anglophones brillent parfois par leur capacité à inventer des mots pour décrire les fonctionnalités ou mécanismes de leurs logiciels. La difficulté, c’est que cette volonté de donner un petit nom réducteur et spécifique à chaque fonctionnalité amène souvent le traducteur à un dilemme à multiples facettes :

* traduire est-il un gain dans la compréhension ou le terme est-il déjà trop utilisé ?
* ma compréhension du terme est-elle suffisante pour apporter un mot/une phrase cohérente avec le contexte ?
* ma langue a-t-elle des mots adaptés et clairs pour y répondre ?
* comment s’assurer que mon remplacement soit cohérent avec la pratique des autres traducteurs ?

### À quoi cela correspond ?

Un webhooks est l’URL d’une interface REST que sera appelée lors d’un évènement sur une application.
On peut traduire sans régionaliser, cela nous mènerait à parler de crochet ou d’hameçon web… Correct mais probablement peu compréhensible.

### Notre approche

Il y a donc eu plusieurs cas présentés par Jérôme :
— méthode web ou méthode HTTP
— rappel web ou rappel HTTP
— voire méthode de rappel HTTP ?

Une approche pourrait aller vers une définition beaucoup plus détaillée et auto-porteuse, comme en parle José : « fonction de rappel HTTP définie par l’utilisateur (webhook) qui correspond d’ailleurs à la définition qu’en donne Wikipédia (user-defined HTTP callback). ».
Cependant, pour connaître la direction à suivre, c’est le contexte que nous devons l’analyser.

Le problème c’est que cette fonction n’est accessible qu’à une population spécifique sur un logiciel non publié, pour voir le contexte c’est compliqué… Heureusement, Zanata a une documentation tout à fait honorable qui parle de ce sujet : [http://docs.zanata.org/en/release/user-guide/projects/project-settings/#webhooks](http://docs.zanata.org/en/release/user-guide/projects/project-settings/#webhooks)

Finalement, nous tendons vers une « URL de rappel », qui signifie : l’URL qui sera rappelée quand l’évènement surviendra.

### Propager la pratique

Voilà, un mot de plus de couvert, j’espère que les autres groupes de traducteurs viendront nous confirmer qu’ils partagent cette traduction. À ma connaissance, traduc.org n’est plus actif, j’ai donc du mal à trouver un lieu pour échanger avec nos semblables d’autres communautés de traduction.

Références :

* [https://lists.fedoraproject.org/archives/list/trans-fr@lists.fedoraproject.org/message/2HZHA2OT2UPE2R2XBYQKP243ZFCOTXRC/](Le lieu de la discussion publique initiée par Jérôme)
* [http://docs.zanata.org/en/release/user-guide/projects/project-settings/#webhooks](documentation de Zanata concernant la fonction Webhooks)
