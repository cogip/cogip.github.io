---
title: 'Moteurs brushless'
---

Salut à tous,

A côté de la coupe, nous expérimentons constamment des nouvelles technologies. Il y a quelques temps, nous nous sommes approvisionné de quelques moteurs brushless et avons dû faire face au problème de leur pilotage. Bien que ces moteurs proposent un couple plus important offrant une meilleure précision, leur contrôle est très différent d'un moteur à courant continu et nécessite un système électronique pour controler le moteur (système triphasé), et ces caractéristiques doivent être adaptées au contexte d'utilisation.

Dans notre cas, le controleur doit être capable de piloter le moteur à basse vitesse, ceci afin que l'algorithme de déplacement et l'asservissement associé puissent s'appliquer. De plus, la commande doit être la plus instantanée possible pour ne pas introduire de délai que l'asservissement ne pourrait rattraper.

N'ayant trouvé de contrôleur à un tarif raisonnable, nous avons réalisé une carte prototype basée sur un chip ST et sommes en train d'effectuer quelques tests en vue de leur installation sur la base roulante.

Voici un aperçu du PCB que nous avons réalisé pour l'occasion:

<img class="image-responsive" src="../img/bldc_ctrl_2017r1__pcb_overview.png" alt="BLDC board" />
<br>

Et voici une vidéo qui montre que les premiers essais du controleur à vide:

<div class="video-responsive">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/if5GEULUZwA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

A ce jour, nous nous interrogeons sur la tenue en charge du controleur, c'est à dire avec une masse importante à déplacer pour le moteur. En effet, on voit sur la vidéo la consommation de courant à faible vitesse qui se traduit par une dissipation de chaleur à prendre en compte.

A suivre...
