---
title: 'Factory 2.0 et la traduction ?'
date: '2016-10-21'
taxonomy:
    category:
        - Régionalisation
    tag:
        - fedora-fr
        - traduction
        - planet-libre
author: 'Jean-Baptiste Holcroft'
---

Un article intéressant sur la « [Factory 2.0](https://communityblog.fedoraproject.org/factory-2-0-mean-modularity/) » a été publié sur le blog communautaire (j’ai couvert la conférence sur le même sujet cet été au Flock dans [cet article](https://jibecfed.fedorapeople.org/blog/transcription-de-ma-2eme-journee-au-flock-cracovie.html)) 

Les problèmes que cette démarche souhaite adresser sont les suivants :

1. les interventions humaines rendent lents les traitements _#1 Repetitive human intervention makes the pipeline slow   _;
2. les sérialisations inutiles rendent lents les traitements _#2 Unnecessary serialization makes the pipeline slow_;
3. l’acheminement impose une cadence rigide et inflexible aux produits _#3 The pipeline imposes a rigid and inflexible cadence on products_;
4. l’acheminement fait des assomptions sur le contenu qui sera livré _#4 The pipeline makes assumptions about the content being shipped_;
5. la distribution est définie par paquet, pas par fonctionnalité (modularité) _#5 The distro is defined by packages, not “features” (Modularity)_;
6. il n’y a pas de façon simple de tracer les dépendances des produits sources _#6 There’s no easy way to trace deps from upstream to product_.

Une partie significative des problèmes adressés sont rencontrés au quotidien par les traducteurs :

1. nous demandons des actualisations des chaînes à traduire, demandons pour les intégrer au projet source, demandons à les intégrer à la distribution ;
2. pour atteindre l’utilisateur, toutes les étapes de production et validation de paquet sont obligatoires alors que le code est inchangé ;
3. nécessité de produire des nouvelles versions, impose le lancement de nombreuses règles et vérifications inutiles ;
4. il faut un RPM contenant d’ailleurs toutes les langues par opposition à un simple fichier po ;
5. quand on s’accorde sur un nouveau terme ou qu’on détecte un mésusage, on doit faire nos corrections en envayant toutes les phrases du paquet, plutôt que simplement la phrase corrigée du sous-périmètre du logiciel concerné.
6. de nombreux logiciels renvoient des chaînes d’autres logiciels, Fedora Media Writer utilise des phrases du site internet, dnf utilise des phrases de rpm mais aussi de dnf-plugin-system-upgrade, dnf-plugins-core, dnf-plugins-extras ; tandis qu’abrt utilise aussi abrt-gnome, libreport, retrace-server et des phrases du noyau !

Je vois donc beaucoup de points communs entre les défis que l’équipe infrastructure tente d’affronter, avec ceux que nous subissons au quotidien. Ils s’intéressent logiquement à leurs points de douleurs, sans adresser les nôtres, qu’ils ne subissent pas au quotidien.

Les traducteurs sont très rarement des développeurs, je doute que le problème soit résolu sans aide. Quand est-ce qu’une équipe spécialisée en internationalisation s’attaquera au problème ?
