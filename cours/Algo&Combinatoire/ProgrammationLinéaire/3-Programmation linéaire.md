#cours #combinatoire


# Définition 







$$ Z = C1.X1 + C2.X2 + ... + Cn.Xn $$




**exemple** 

Un fleuriste dispose de 50 lys, 80 roses et 80 jonquilles. Il réalise ou  bien des bouquets  qu'il vend 40 euros comprenant 10 lys, 10 roses et jonquilles, ou bien des bouquets dont il tire un prix de 50 euros qui comprennent 10 lys, 20 roses et 10 jonquilles. Comment le fleuriste doit il former les bouquets pour réaliser une recette maximale ? 


**solution**

1. trouver les variables de décisions
	 - Choisir de ne rien faire
	 - Choisir combien de bouquet de chaque type il peut faire
		autrement dit les variables de décisions sont
	 - Nb40 -> nombre de bouquet à 40 euros
	 - Nb50 -> nombre de bouquet à 50 euros
	   
2. exprimer la fonction objectif  
	 $$Z  = nb40 * 40 + nb50 * 50$$
		!! attention au unités lors de l'expression de la fonction objectif !!

3. les contraintes de décision
	- 10Nb40 + 10Nb50 < 50
	- 10Nb40 + 20Nb50 < 80
	- 20Nb40 + 10Nb50 <80
	- Nb40 >= 0 
	- Nb50 >= 0

4. résolution de la solution
		
		


![[exempleProgrammationLineaire | 2048]]


[[3.1-algorithme du simplexe]]