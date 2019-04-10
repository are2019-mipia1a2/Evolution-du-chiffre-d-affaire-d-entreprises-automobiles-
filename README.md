## Bienvenue chez le groupe projet ECAEA...lisez la suite vous comprendrez

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

[Notre presentation du projet](ARE.pdf)

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

Nous avons décider de déterminer un prix de production de la voiture. Pour cela, on a fait divers recherches, sur différent sites pour avoir le prix des composantes essentielles, tel que le capot, l'alternateur...etc. A partir de ces prix, que l'on sommera, on mettra en place un prix de production de voiture, qui ne variera qu'en fonction des trois critères, déjà énumérés. On fera évoluer ce prix de production, en prenant en compte les salariés.
Puis, avec ce prix de production, il en découlera un prix de vente, calculé selon le taux de marge choisi.
Nous avons décidé, qu'au début les clients acheteront quel que soit le prix, mais avec les critères qu'ils veulent. Enquite, le prix de vente sera l'unique critère pris en compte (un budget fixe). Et enfin on regroupera les deux. 
On a aussi commencé à regrouper les réponses du sondage, qui s'élévent à 84, pour détérminer des statistiques de préférence et commencer à faire fonctionner la fonction "score_de_première_période" (Code de CA), qui correspond au nombre de clients potentiels pour chaque entreprise, à une première génération. (cette fonction n'est, probablement, pas tout à fait au point).


### Bilan 4:
Mercredi 27/03/2019

Nous avons commencé à prendre en compte la descendance de la population dans nos fonctions, et donc par conséquent la démographie. Cela nous permettra de calculer le nombre de voitures vendus par l'entreprise par rapport à la population à une génération donnée. 
Nous avons aussi créé une fonction qui permet de calculer le prix de vente d'une voiture, en fonction du prix des composantes, en séparant les critères variables et fixes, ainsi que la marge choisie par l'entreprise.
Nous avons par ailleurs collecté les résultats du sondage. Nous avons décidé d'établir un coefficient entier entre 3 et 1, qui représente le classement des critères par les "clients". Ceci nous menera vers une exploitation plus pratique et simple des données. Nous remplirons ainsi le dictionnaire des "préférences" en établissant des probabilités adaptées.

### Bilan 5:
Mercredi 3/04/2019

Nous avons rempli le dictionnaire des "préférence", alors nous avons pu tester la fonction score_première_période, qui présentait
certaines incohérences; heureusement nous avons réglé le problème, en s'inspirant des fractions égyptiennes pour détérminer un coefficient de préférence, pour chaque critère, inférieur à 1 dont la somme donne 1: 1/2 pour le premier choix, 1/3 pour le second, 1/6 pour le dernier. Ainsi, on arrive à obtenir le nombre de clients (le score) potentiel pour chaque entreprise, pour un seul modèle de voiture. Pour affiner l'étude, nous avons mis en place une fonction score_n_période, qui rend la liste des clients (score) pour chaque période, au bout de laquelle la génération et la voiture changent. Celle-ci ne fonctionne toujours pas, suite à une erreur que nous ne comprenons pas. Nous travaillons donc dessus. Une fois, qu'elle sera mise en point, nous ferons varier le prix selon ces nouvelles voitures (en créant une liste pour chaque période également). Nous calculerons par conséquent le chiffre d'affaire : nombre client X prix. Il suffira alors de tracer le graph correspondant. Nous envisageons de le comparer aux courbes du score et prix.
Par la suite nous chercherons à prendre en compte l'influence du prix, en précisons un intervalle de budget pour chaque catégorie de client. Un nouveau score devra être établi. Comparer les courbes du CA et prix sera plus intéressant à ce stade. 

### Bilan final :
Mercredi 10/04/2019

Nous avons finaliser la fonction score_et_prix_n_periode, nous avons également décider de tracer des barres. Nous obtenons ainsi des barres du nombre de clients (score), ainsi que ceux du prix. Nous finalisons la fonction chiffre d'affaire et nous allons obtenir son graph également. 
Nous avons aussi obtenu des intervalles de budget pour chacune des catégories de client, nous allons les diviser en trois sous-intervalles, en leur fixant un coefficient, de sorte que plus le prix de la voiture est élevée, moins il y aura de clients, donc moins le score sera grand. Ainsi, il y-aura dépendance entre "préférence et prix". Nous essayons de mettre en place les fonctions correspondantes. Nous traçerons ensuite ses nouvelles fonctions sous forme de bar également.

## Bibliographie

#### [Sondage du ECAEA](sondage.pdf)

#### Sites internet divers, pour le prix des composantes : 
l'internaute, Automoto, Caradisiac, Cost-Helper, Mecathecnic, Autoservicecosts.com, idgrages.com, monmecanicien.com, goodmecano.com, Itstillruns, glassusa.com, marijouls.fr, numbeo, carmagazine. 

#### Sites internet divers, pour le budget :
csa.eu //
capital.fr


