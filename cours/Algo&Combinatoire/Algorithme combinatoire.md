
#cours #combinatoire
# Technique d'Optimisation pour la résolution de Problèmes Combinatoires


*La Technique d'Optimisation pour la résolution de Problèmes Combinatoires impliquent la recherche d'une solution optimale parmi un ensemble fini mais souvent très grand de possibilités. Ils sont caractérisés par la nécessité de combiner des éléments selon certaines règles pour atteindre un objectif spécifié.*


### Caractéristiques des Problèmes Combinatoires

* **Ensemble Discret :** Les solutions possibles forment un ensemble discret, souvent de taille exponentielle en fonction de la taille de l'entrée.

 * **Optimisation :** L'objectif est de trouver la meilleure solution selon un critère donné (par exemple, le coût le plus bas, la distance la plus courte, le profit le plus élevé).

 * **Complexité :** Beaucoup de ces problèmes sont NP-difficiles, ce qui signifie qu'il n'existe pas, à ce jour, d'algorithme connu pour les résoudre efficacement (en temps polynomial) dans tous les cas.


   **Exemple** :  trouver la couleur préférée d'une personne choisie au hasard
   On part donc du principe que dans sa tête, l'individu à une fonction qui note les différentes couleurs et sa préféré aurait donc la note la plus haute.
   

![[DrawCombinatoire1]]

première conclusion, on ce rend compte que le référentiel des réponses sont assez flou. Il faut donc changer de méthodes en demandant cette fois de noter de 0 à 1 

![[DrawCombinatoire2]]

Dans cette exemple nous sommes partie d'une hypothèse, on à supposé qu'il n'yavait qu'une seule couleur préféré. L'objectif est donc de trouver des valeur hautes au dépend des valeur minimum. Cet exemple peut donc être représenter par une courbe. 

![[DrawCombinatoire3]]

### Techniques d'Optimisation

1. **Méthodes Exactes :**
    - **Programmation Linéaire :** Pour les problèmes pouvant être formulés comme des ensembles de contraintes linéaires.
    - **Branch and Bound :** Technique qui divise le problème en sous-problèmes plus petits et gère ces sous-problèmes de manière systématique.
	 [[3-Programmation linéaire]]
    
2. **Heuristiques :**
    - Approches qui trouvent de bonnes solutions en un temps raisonnable mais sans garantie d'optimalité.
    - Exemples : algorithme glouton, heuristique de construction.
    [[2-Heuristique]]

3. **Métaheuristiques :**
    - Techniques plus générales comme l'optimisation par essaim de particules, les algorithmes génétiques, etc.
    - Bonnes pour trouver des solutions de haute qualité dans des espaces de recherche complexes.
    [[1-Métaheuristique]]