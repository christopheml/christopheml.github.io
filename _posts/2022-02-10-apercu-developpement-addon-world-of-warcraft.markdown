---
title: "Un aperçu du développement d'addons World of Warcraft"
tags: lua wow addon
---

Gros joueur de World of Warcraft depuis sa sortie et développeur, il était inévitable que finisse par développer des addons, mais ça n'a pas été sans embûche. Je vais essayer avec cet article de fournir quelques raccourcis.

## Un addon vous dites ?

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

[John Staats]: https://twitter.com/JohnStaats_WIR

[The Wow Diary]: https://www.kickstarter.com/projects/whenitsready/the-world-of-warcraft-diary-0

## L'état des lieux

Je dois dire que démarrer dans le développement d'addon n'a pas été de tout repos. Quand on bosse dans des écosystèmes de développement un peu matures, la transition est rude. 

Je viens du monde Java et la plupart des choses que nous y tenons pour acquises, à savoir un support IDE complet, pléthore de composants réutilisables, l'accès complet au code source et une documentation riche ne sont clairement pas au rendez-vous, il va falloir s'en passer.

Le support IDE est médiocre, la documentation disponible - malgré les efforts des contributeurs - est lacunaire, il y a des composants réutilisables mais ils sont rares et de qualité inégable. Quant au code source, si chaque addon est de fait distribué en open-source et que Blizzard a ouvert une partie de code de son interface, une large portion reste inaccessible (probablement car faisant partie du moteur du jeu et donc codée en C++).

De même, les pratiques modernes de développement logiciel ont un peu de retard, mais la situation s'est quand même pas mal améliorée, notamment du fait des développeurs de très gros addons dont le développement et la maintenance sont devenus conséquents. 

## Documentation ? Quelle documentation ?

## L'outillage

## Ne pas réinventer la roue
