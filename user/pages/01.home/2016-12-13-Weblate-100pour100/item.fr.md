---
title: 'Parfois, cent pour cent n’est pas suffisant 😏'
date: '2016-12-13'
taxonomy:
    category:
        - Régionalisation
    tag:
        - fedora-fr
        - traduction
        - planet-libre
author: 'Jean-Baptiste Holcroft'
---

La plateforme de traduction Weblate est un outil de grande qualité ([lire mon article](https://jibecfed.fedorapeople.org/blog/quest-ce-quune-bonne-plateforme-de-traduction.html)), et traduite à 100 %, mais cela ne veut pas dire que c’est parfait !
Récit de mes quelques modifications. 

### Pourquoi suis-je allé y contribuer ?

Le projet [YunoHost](https://yunohost.org) l’utilise comme plateforme de traduction (qu’ils [hébergent eux-mêmes](https://translate.yunohost.org/), fidèles à leurs valeurs), mais utilise une version 2.8 dont l’interface est très peu traduite en français. Comme je trouve l’outil d’une grande qualité, j’ai décidé d’aller aider à la traduction de la nouvelle version pour qu’on puisse avoir une plateforme correctement traduite.

### En arrivant

J’ai constaté que sur les 1 400 phrases, quelques-unes très récentes étaient à traduire, une fois complétées, j’ai débuté un travail de revue, un peu globale pour chasser ces vilaines apostrophes dactylographiques et les remplacer par des typographiques. L’intérêt n’étant qu’esthétique, j’en profite surtout pour identifier des textes entre apostrophes au lieu de guillemets, et sonder la qualité de la traduction.

### Modifications réalisées

Globalement, peu d’erreurs majeures, mais quelques petites corrections nécessaires :

 * des « mail » et « email » non traduits alors que le reste de la traduction parle de « courriel » ;
 * quelques petites phrases qui m’ont semblé un peu ambiguës. Soit il faut décrire ce qu’on fait « on marque la phrase comme étant à vérifier », soit on « passe la phrase au statut « À vérifier » ». Je ne vois pas vraiment l’intérêt de répéter le statut tel quel car la phrase est compréhensible sans, et que ce n’est pas ce qui est fait en anglais ;
 * le mot qu’utilise beaucoup Weblate est « repository » et le glossaire l’indique en tant que « référentiel ». Je ne suis pas sûr que ce soit la meilleure traduction, mais je trouve ça différent et compréhensible, pourquoi pas ;
 * quelques petites « chaines » sont devenues des « chaînes ».
 * Des erreurs manifestes de traduction :
     * corrigé une phrase sous-entendant que l’interlocuteur est un homme ;
     * « traduction machine » en « traduction automatisée » ;
     * “colon” c’est « double-point » et derrière on parle de leur espacement ;
     * « Search and replace completed » était « Traduction automatique terminée » et est devenue « La recherche avec remplacement a été effectuée » ;
     * les apostrophes typographiques.

La majorité des changements est visible via ces commits sur le git de Weblate :

 * [https://github.com/WeblateOrg/weblate/commit/c34f6a237a3d30a94b64710c98793250317f6c21](https://github.com/WeblateOrg/weblate/commit/c34f6a237a3d30a94b64710c98793250317f6c21)
 * [https://github.com/WeblateOrg/weblate/commit/539f182c40b7e71db843a0968ae548835541660c](https://github.com/WeblateOrg/weblate/commit/539f182c40b7e71db843a0968ae548835541660c)
 * [https://github.com/WeblateOrg/website/commit/214043f56238a2be11a791a4135e8a93fc4bca07](https://github.com/WeblateOrg/website/commit/214043f56238a2be11a791a4135e8a93fc4bca07)

### En conclusion

Un projet, même traduit à 100 % peuvent bénéficier d’un regard extérieur qui améliorent la cohérence. Merci également à « ldm » de m’avoir interrogé pour comprendre mes modifications et échanger sur la meilleure façon de faire. Je suis très content de voir que quelques personnes veillent sur des projets !

Si vous cherchez, vous trouverez encore des choses à améliorer, ne vous censurez pas ! Ou mieux encore, adoptez votre projet !
