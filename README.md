# spanning-tree-protocol
Approfondissement du protocole spanning-tree (Norme IEEE 802.1D)

Le Spanning Tree Protocol (aussi appelé STP) est un protocole réseau de niveau 2 permettant de déterminer une topologie réseau sans boucle dans les LAN avec ponts. Il est défini dans la norme IEEE 802.1D et est basé sur un algorithme décrit par Radia Perlman en 1985

L'algorithme du spanning tree procède en plusieurs phases.

* D’abord il va élire le commutateur racine
* Ensuite il va déterminer les ports racines de chaque commutateur.
* Après, il va sélectionner les ports désignés sur chaque segment.
* Et pour finir, il va bloquer les autres ports, pour éviter les boucles.
Tout ce processus se fait à l’aide des messages BPDU que s’échangent les commutateurs

Les BPDU’s sont des trames qui sont échangées régulièrement, à peu près environ toutes les 2 secondes, et permettent aux switches de garder une trace des changements sur le réseau afin d’activer ou de désactiver les ports des équipements

![image](https://user-images.githubusercontent.com/83721477/163803182-89b02ada-d7f2-47f6-979a-4feb68bfb33b.png)
