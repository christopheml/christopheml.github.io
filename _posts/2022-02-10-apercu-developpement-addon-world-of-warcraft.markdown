---
title: "Un aperçu du développement d'addons World of Warcraft"
tags: lua wow addon
---

Gros joueur de World of Warcraft depuis sa sortie et développeur, il était inévitable que finisse par développer des addons, mais ça n'a pas été sans embûche. Je vais essayer avec cet article de fournir quelques raccourcis.

## Un addon vous dites ?

### Un choix pas banal

On est décembre 2002, World of Warcraft en est à sa deuxième alpha interne, et Blizzard va faire quelque chose alors extrêmement rare pour un jeu vidéo et ouvrir très largement l'interface utilisateur du jeu à la modification par les joueurs.

[John Staats] raconte l'arrivée de cette fonctionnalité et la relative incrédulité de l'équipe dans [The Wow Diary] :

> During the slow month of December, programmer Sam Lantinga finished  
> making our user interface customizable via a lightweight programming  
> language called Lua. Despite the fact Sam had explained it to the artists  
> a number of times, the concept of a user-controlled interface didn’t make  
> sense, but the designers and programmers assured us it would be great.  
> Most of us couldn’t understand what was so wrong with the default inter-  
> face that we now wanted to turn control of it over to the general public.  
> Why let users control the interface? How much better could they make it?  
> Wasn’t it clean enough?

Au final, cette décision a payé de façon spectaculaire. Des milliers d'addons ont été créés pour modifier, enrichir voire remplacer complètement l'interface par défaut du jeu, permettant aux joueurs de se fabriquer une expérience sur-mesure.

Régulièrement, Blizzard s'est servi de ce laboratoire géant pour améliorer son interface de base et la faire coller au plus près des besoins des joueur.

[John Staats]: https://twitter.com/JohnStaats_WIR

[The Wow Diary]: https://www.kickstarter.com/projects/whenitsready/the-world-of-warcraft-diary-0

### Des technos simples, basiques

Les addons sont écrits dans le langage [Lua], tandis que les éléments de l'interface graphique peuvent être écrits en [XML]. Le code n'est pas compilé et les addons sont, de fait, open-source.

Ils interagissent avec le jeu au moyen de plusieurs API fournies par Blizzard et s'exécutent dans un interpréteur Lua 5.1 adapté par Blizzard et embarqué dans le moteur de jeu, qui limite les fonctionnalités utilisables afin d'éviter le piratage ou la trinche. 

[Lua]: https://www.lua.org/

[XML]: https://fr.wikipedia.org/wiki/Extensible_Markup_Language 

## L'état des lieux du dévelopmment

Je dois dire que démarrer dans le développement d'addon n'a pas été de tout repos. Quand on bosse dans des écosystèmes de langages un peu matures, la transition est rude. Venant du monde Java, la plupart des choses que nous y tenons pour acquises, à savoir un support IDE complet, pléthore de composants réutilisables, l'accès complet au code source et une documentation riche ne sont clairement pas au rendez-vous, il va falloir s'en passer.

Le support IDE est médiocre, la documentation disponible - malgré les efforts des contributeurs - est lacunaire, il y a des composants réutilisables mais ils sont rares et de qualité inégale. Quant au code source, si on peut s'inspirer du code des addons existants et que Blizzard a ouvert une partie du code de son interface, une large portion reste inaccessible (probablement car faisant directement partie du moteur du jeu et donc codée en C++).

Les pratiques modernes de développement logiciel ont un peu de retard, même si la situation s'est améliorée au fil du temps, notamment du fait des développeurs d'addons massifs et complexes dont le développement et la maintenance ont demandé une plus grande rigueur.

### Documentation ? Quelle documentation ?

Une faible partie de la documentation est fournie par Blizzard, sous deux formes différentes : 

- une documentation d'API sommaire qui liste les fonctions accessibles ainsi que les noms et les types éventuels des paramètres, mais sans expliquer ce que font les fonctions et sans préciser à quoi servent les paramètres.

- la publication du code source de toute l'interface par défaut du jeu, qui comporte beaucoup de composants de base réutilisables et comporte parfois quelques commentaires utiles pour comprendre le fonctionnement de telle ou telle partie.

Le reste de la documentation est géré par la communauté, dont les volontaires l'alimentent par rétro-ingénierie. L'essentiel de cette documentation est hébergé sur [Wowpedia], qui a malheureusement été racheté depuis par Fandom.

On y trouve une présentation générale de l'API Blizzard, des composants d'interface standards, des tutoriels variés et une documentation plus détaillée des fonctions de l'API. Sa qualité est inégale, certains articles sont incomplets ou obsolètes, quand d'autres sont complets et extrêmement précieux pour la compréhension de certains mécanismes.

[Wowpedia]: https://wowpedia.fandom.com/wiki/Wowpedia:Interface_customizationhttps://wowpedia.fandom.com/wiki/Wowpedia:Interface_customization

### L'outillage

Le support IDE pour Lua et XML est tout à fait correct et permet d'avoir un minimum d'assistance pendant le développement. 

Blizzard a publié les schémas XSD relatifs à ses documents XML, ce qui permet de profiter d'une autocomplétion efficace. Pour Lua c'est plus compliqué, puisqu'il faut générer des fichiers ou des plugins d'IDE à partir de l'API du jeu. Il s'agit souvent de projets qui finissent par ne plus être maintenus car le travail à fournir est conséquent.





## Ne pas réinventer la roue
