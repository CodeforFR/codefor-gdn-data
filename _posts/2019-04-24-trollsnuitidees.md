---
layout: post
title:  "Trouver les trolls"
# author
# date : 31 janvier 2019 
categories: [granddebat]
# tags: [red, yellow]
# tags = categories, n'en garder qu'un
image: assets/images/projets/mattisg.png
description: "Détecter les trolls dans les réponses au Grand Débat National"
featured: false
hidden: false
# rating: 4.5
---

Lors du hackathon de la Nuit des Idées au Liberté Living Lab le 31 janvier 2019, nous avons travaillé sur la détection de réponses spécifiques. Pour tester la recherche dans le corpus de réponses pouvant signaler un troll, nous avons choisi plusieurs expressions ou formats dans le titre: titre en majuscules (ALL CAPS), trois points d'exclamation à la suite (!!!), URL dans le titre de la contribution, expression "Benalla" (nous travaillions sur les contributions de la catégorie "écologie"). L'analyse permet d'attribuer une pondération à chaque contribution ("score de troll").

*A noter: L'objectif n'était pas de prouver que la présence de "Benalla" dans le texte indiquait forcément un troll, mais de tester la réutilisabilité des données et les scripts de recherche d'expressions ciblées au sein du corpus. Les résultats ne sont pas toujours [pertinents](https://github.com/MattiSG/grand-debat-trolling/blob/master/resultats-ecologie.csv#L810) et on peut considérer que la conclusion est qu'il est très difficile de détecter les trolls. L'intérêt principal est qu'une base est codée, sur laquelle il est trivial de rajouter des [détecteurs]( https://github.com/MattiSG/grand-debat-trolling/tree/master/troll-detectors).
Si un groupe souhaitait pousser l'idée plus loin il faudrait évaluer la pertinence de chacun d'entre eux pour modifier la pondération, actuellement attribuée arbitrairement.*

Lors du même hackathon, Alexis Thual a développé un script pour identifier des clusters de contributions similaires. Le résultat est disponible [ici](https://github.com/alexis-thual/debat-ouvert/blob/master/notebook.ipynb).  

#### Sources

* [Code pour détecter les trolls de MattiSG](https://github.com/MattiSG/grand-debat-trolling)
