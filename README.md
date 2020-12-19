# sh-doc-fr-norme_ksh

### Document

[Norme_ksh-1.1-d1.docx](Norme_ksh-1.1-d1.docx)

### Résumé

[FR] Norme d'écriture des scripts ksh

NB : uniquement ksh88, la version ksh93 n'est pas traitée.

### Dates

* Rédaction initiale : 2011 - 2012
* Modifications mineures : 2013, 2015

### Description

Ce document représente ma vision concernant la façon de bien utiliser le langage ksh (Korn shell) pour écrire des scripts fiables, simples, faciles à maintenir (et performants si possible) – telle qu'elle était quand j'ai entrepris sa rédaction en 2011.

Important : ce document n'est pas maintenu (je fais beaucoup moins de shell depuis quelques années) ; il n'est présenté ici qu'à titre d'information.

### Pourquoi ksh93 n'est-il pas traité ?

Plusieurs raisons :

* En 2011, quand j'ai entrepris la rédaction de cette norme, j'évoluais dans un environnement technique mixte avec ksh88 sous Solaris 10 et ksh93 sous Linux ; ksh88 était donc le "plus petit dénominateur commun" qu'il convenait d'utiliser afin que les scripts puissent s'exécuter à la fois sous Solaris et sous Linux, moyennant quelques précautions pour contourner certaines différences, marginales mais réelles, de comportement entre les 2 versions.

* ksh93 est beaucoup plus complexe que ksh88, et offre une richesse de fonctionnalités si étendue que je n'ai toujours pas fini d'en faire le tour ! Et dont une grande partie est très peu utilisée car soit ces nouvelles fonctionnalités sont ignorées, soit les programmeurs qui auraient pu les utiliser se sont tournés vers d'autres langages plus robustes ou plus adéquats (Perl, Python, etc.) pour accomplir les tâches auxquelles ces fonctionnalités étaient destinées.

* Enfin, les différences de comportement, souvent subtiles, mais cependant multiples, entre ksh88 et ksh93 font qu'essayer de traiter des 2 versions simultanément dans le même document promettait d'aboutir à un résultat difficile à lire. 

### Liens

#### ksh93

* Page [Enhanced Korn Shell (ksh93)](https://www.ibm.com/support/knowledgecenter/ssw_aix_72/osmanagement/korn_shell_enhanced.html) dans la documentation de IBM AIX 7.2
* [Principales différences](https://markmail.org/message/6xijgi35pqmjw37t#query:+page:1+mid:m7jkcvb6tm5ffktb+state:results) entre ksh88 et ksh93, telles que documentées initialement 
* [David Korn Tells All](https://news.slashdot.org/story/01/02/06/2030205/david-korn-tells-all) : interview de David Korn sur Slashdot – voir notamment la question « 1) Comparison »

#### Perspective historique

* [Introduction to the Unix shell history](http://www.softpanorama.org/People/Shell_giants/introduction.shtml) sur le site Softpanorama.org
