## Bienvenue chez le groupe projet EEA...lisez la suite vous comprendrez

**Membres :**

Azrou Razane

Rashid Osama

Billon Martin

Saadoun Lirone

**Le Projet:**

Notre projet correspondera à la modélisation de l'évolution du chiffre d'affaire d'entreprises automobiles, comme le titre de notre répéretoire l'indique.
Nous chercherons le moyen d'obtenir le meilleur CA possible, en se basant sur la concurrence d'entreprises aux stratégies commerciales différentes.
Bien évidemment, le flux des autres paramètres (clients, salariés..etc) indiquera laquelle suit la meilleure stratégie pour un CA positif à long terme.
Nous envisagerons entre autre des scénarios, favorables ou défavorables, au bon développement des entreprises.

Le premier, que l'on envisage, correspondera à la concurrence entre deux entreprises uniquement, qui vendent deux catégories de voitures différentes par trois critères.
On posera ainsi un score quant aux préférence des clients.

Pour les autres scénarios, nous prendrons en compte plus de paramètres pour obtenir une modélisation plus réaliste.

[Notre presentation](ARE.pdf)

### Bilan 1 : 
Pour le mercredi 6 mars 2019, nous avons créé une clé github et suivi les étapes indiquées par le professeur. 
Entre temps, nous avons discuté de notre projet, en décidant des trois critères à faire varier : la taille, consommation en carburant et le moteur (en terme de chevaux) des voitures concurrentes. Nous avons, par conséquent, cherché des statistiques sur la préférences des clients, qui ne varient que par leur âge et sexe. Puisque, nous n'avons "rien" trouvé, nous avons décidé de faire un sondage nous-même, qui sera ainsi notre source.
Ce jour-là, un intervenant nous a aussi expliqué comment faire une bonne recherche bibliographique, qui nous sera très utile pour la suite.

### Bilan 2:
Mercredi 13/03/2019

Nous avons mis en place le sondage,comme prévu. Et pour le moment nous avons reçu 4 réponses.
En attendant d'obtenir plus de réponses, nous avons créé une première fonction qui permet de calculer le score de chaque entreprise. Pour cela, nous avons également fait une petite recherche sur la population selon le sexe et les tranches d'âge. 
Ainsi, la fonction permet de comparer les deux entreprises, en terme de préférence, selon le client, pour une première génération.
Nous l'utiliserons donc pour étendre l'estimation à plusieurs générations et en variant les voitures "construites".

### Bilan 3 :
Mercredi 20/03/2019

Nous avons décider de déterminer un prix de production de la voiture. Pour cela, on a fait divers recherches, sur différent sites pour avoir le prix des composantes essentielles, tel que le capot, l'alternateur...etc. A partir de ces prix, que l'on sommera, on mettra en place un prix de production de voiture, qui ne variera qu'en fonction des trois critères, déjà énumérés.
Puis, avec ce prix de production, il en découlera un prix de vente, calculé selon le taux de marge choisi.
Nous avons décidé, qu'au début les clients acheterons quel que soit le prix, mais avec les critères qu'ils veulent. Puis, le prix ce l'unique critère pris en compte (un budget fixe). Et enfin on regroupera les deux. 
On a aussi commencé à regrouper les réponses de sondage, pour obtenir les pourcentage de "préférence" et faire fonctionner la fonction Code CA.
