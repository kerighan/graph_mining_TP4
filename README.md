L'ensemble de données Cora comprend 2708 publications scientifiques classées dans l'une des sept classes. Le réseau de citations comprend 5429 liens. Chaque publication de l'ensemble de données est décrite par un vecteur de mots à valeur 0/1 indiquant l'absence/présence du mot correspondant dans le dictionnaire.

Exercice 1 - Baseline
==========

Dans datasets, vous trouverez features.npy, une matrice numpy (n_nodes, n_features) qui représente les features des noeuds du graphe.
Vous trouverez également labels.npy, la matrice binaire (n_nodes, n_labels) qui décrit le label des noeuds.
* créer un modèle simple avec Keras (ou n'importe quel autre librairie) permettant la classification des labels à partir des features
* calculer la précision sur un split de taille 0.2


Exercice 2 - GCN
==========

Le graphe correspondant est le fichier G.gexf. L'ordre des noeuds dans G.nodes correspond à l'ordre des matrices de features et de labels.
* créer un simple GCN (fonction d'activation : tanh) à un seul layer
* en annulant les labels à certains noeuds aléatoires, calculer la précision sur un split de taille 0.2
* étendre le GCN à 2 layers et calculer sa précision
