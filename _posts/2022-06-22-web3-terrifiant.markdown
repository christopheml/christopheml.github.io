---

title: "L'horrible dystopie des cryptobros"
summary: "Les technologies de blockchains publiques ."
tags: [crypto, bitcoin, web3, vie privée]

---

Quand une techno se pointe avec une vision de l'avenir, c'est important de lire les petits caractères et de tendre l'oreille aux propos de ses plus ardents défenseurs.

{% include figure image_path="/assets/images/dystopia_by_alex_kristanas.jpg" alt="Une photo nocturne d'un grafiti en lettres rouges épaisses demandant : IS THIS DYSTOPIA?." caption="Photo par [alex kristanas](https://unsplash.com/@devdvr) sur [Unsplash](https://unsplash.com/s/photos/dystopia)." %}

# Une solution en quête d'un problème

## Quelques rappels

Les technologies de blockchains, que je vais résumé sous le terme de "cryptos" dans cet article (bien qu'il ne soit parfait et qu'il couvre des applications assez différentes) ont essaimé un peu partout depuis la création du Bitcoin en 2009.

Une blockchain est une forme de base de données distribuée résistante à la réécriture. Elle peut être publique ou privée, centralisée ou décentralisée.

Je ne reviendrai pas particulièrement les blockchains privées ou centralisées parce qu'elles ont un intérêt relativement limité et un impact sociétal nul (traduction : "on fait pareil avec un PostgreSQL"). Les blockchains publiques décentralisées par contre sont de loin les plus populaires et les plus influentes.

Pour qu'une blockchain soit décentralisée, il faut que les opérations d'écriture (ajout d'un nouveau bloc) fassent l'objet d'un consensus entre les participants au réseau et que personne ne puisse écrire des données arbitraires. Les techniques les plus courantes pour assurer ce consensus sont la [preuve de travail] (proof of work) et la [preuve d'enjeu] (proof of stake). 

On a donc une base de données distribuée, découpée en blocs, qui ne sont plus modifiables après écriture. Très bien. Qu'est-ce qu'on en fait ?

## Le Bitcoin

La première application concrète, le Bitcoin, devait selon les termes exacts de son créateur, être "de l'argent liquide électronique" (le [livre blanc] décrivant la technologie s'appelait "Bitcoin: A Peer-to-Peer Electronic Cash System") : la blockchain fait office de livre de comptes géant où sont stockées toutes les transactions, le consensus se fait par preuve de travail et la validation de bloc est rémunérée en Bitcoins (cette rémunération contre validation s'appelle "le minage", par analogie avec l'extraction de matériaux précieux).

Si l'idée d'utiliser le Bitcoin comme une monnaie était le souhait de son créateur, en pratique elle a foiré de façon spectaculaire. La capacité du réseau est faible, le coût de transaction est élevé, la valeur du Bitcoin est extrêmement instable et sa nature déflationniste incite ses détenteurs à les conserver plutôt qu'à les dépenser. 

13 après son apparition, le Bitcoin n'est utilisé à peu près nulle part comme moyen de paiement de la vie courante. Son introduction au [Salvador] est un échec, malgré les efforts démesurés de son président, Nayib Bukele.

Des projets existent pour rendre le Bitcoin "utilisable", comme le Lightning Network, pour que le réseau s'adapte à un plus grand nombre d'utilisateurs, mais son efficacité est [remise en doute]. 

Face à ces limitations, les partisans du Bitcoin ont adapté leurs discours au fil du temps, jurant sur leur grand-mère que non, le Bitcoin n'a jamais été prévu pour être un moyen de paiement, mais une réserve de valeur (douteux vu la volatilité du prix lié entre autres à son illiquidité) ou encore une protection contre l'inflation (le crash des cryptos en pleine explosion de l'inflation prouve que ça n'est pas le cas).

En l'absence de véritable usage, il ne reste au Bitcoin qu'à être acheté pour être revendu plus cher à un "[greater fool]", on reconnaîtra volontiers que ça n'a strictement rien de révolutionnaire. Et les contraintes techniques et économiques pesant sur le Bitcoin ne laissent pas particulièrement de place à l'émergence d'usages nouveaux qu'on n'aurait pas encore imaginés.

Ce qui n'empêche pas de lire des âneries stratosphériques, comme ce beau [morceau de pipeau de Jack Dorsey], le créateur de Twitter.

{% include figure image_path="/assets/images/cryptos/jack_dorsey_bitcoin_tweet.png" alt="Jack Dorsey (@jack) tweeted in August 9, 2021: '#Bitcoin will unite a deeply divided country. (and eventually: world)'" %}

## Les applications décentralisées

Vous allez me dire que c'est bien gentil tout ça, mais qu'il n'y a pas que le Bitcoin dans la vie. En effet, d'autres blockchains ont pour caractéristique de supporter la rédaction et l'exécution de contrats automatisés, qui sont enregistrés dans la blockchain et qui permettent de développer pas mal de choses.

# Vous en faites pas, tout va bien

C'est toujours un peu compliqué de parler de [Web3], vu que le concept est volontairement flou et mal défini par ceux qui s'en réclament. Mais certains traits communs ressortent et méritent qu'on s'y attarde.

Le Web3 promet notamment de libérer les internautes des griffes des plateformes en décentralisant, de retrouver le contrôle de leur identité numérique, de leur vie privée, de redonner du pouvoir aux utilisateurs et de rémunérer correctement la création de contenus. 

C'est un programme assez ambitieux mais ma modeste description est très en-dessous  de la réalité. Pour le moment, on ne peut pas dire que ça soit une grande réussite, comme le relève [Molly White] sur [Web3 is going just great], cet espace étant gangréné par les problèmes de piratages, d'arnaques, de fraudes et autres spectaculaires faillites.

Je ne vais pas aborder directement ces questions, ni la fâcheuse tendance du Web3 à [ressembler culturellement à du marketing multi-niveaux].

Je voudrais parler deux caractéristiques fondamentales du Web3 qui en font une alternative absolument terrifiante au Web tel que nous le connaissons, tout aussi imparfait qu'il soit.

L'idée du Web3 est d'ajouter aux structures actuelles d'Internet une infrastructure, basée sur des technologies de blockchains publiques, infrastructure sur laquelle seront développés des services décentralisés. Il sera non seulement possible d'accéder à ces services, mais aussi les posséder collectivement et de prendre part à leur gouvernance à travers de [DAO].

# Rien n'échappera à l'avarice

Si l'idée derrière les DAO n'est pas saugrenue et que les blockchains semblent être un use case adapté à une participation financière à une forme d'entreprise décentralisée, ça se gâte sérieusement quand on commence à regarder les autres cas d'utilisation.



# Rien ne s'oubliera


[preuve de travail]: https://fr.wikipedia.org/wiki/Preuve_de_travail
[preuve d'enjeu]: https://fr.wikipedia.org/wiki/Preuve_d%27enjeu
[livre blanc]: https://bitcoin.org/bitcoin.pdf
[Salvador]: https://www.politico.com/news/magazine/2022/05/12/el-salvador-bitcoin-currency-struggles-00030422
[remise en doute]: https://www.coindesk.com/markets/2018/01/20/lightning-network-may-not-solve-bitcoins-scaling-trilemma/
[greater fool]: https://en.wikipedia.org/wiki/Greater_fool_theory
[morceau de pipeau de Jack Dorsey]: https://twitter.com/jack/status/1424854924194729984
[Web3]: https://tante.cc/2021/12/17/the-third-web/
[Molly White]: https://twitter.com/molly0xFFF
[Web3 is going just great]: https://web3isgoinggreat.com/
[ressembler culturellement à du marketing multi-niveaux]: https://noahpinion.substack.com/p/is-web3-culture-similar-to-amway/
[DAOs]: https://fr.wikipedia.org/wiki/Organisation_autonome_d%C3%A9centralis%C3%A9e
