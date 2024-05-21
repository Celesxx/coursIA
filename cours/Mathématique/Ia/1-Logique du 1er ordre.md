

#cours  #mathematique

# Définition 

Une logique du 1er ordre est une proposition qui est soit True soit False, également connue sous le nom de logique des prédicats du premier ordre ou simplement logique des prédicats, est un système de logique formelle qui est utilisé pour décrire des relations entre différents objets, des propriétés des objets, et pour raisonner sur ces objets et leurs relations. Elle étend la logique propositionnelle en incluant des concepts comme les fonctions, les quantificateurs et les variables.


# Les connecteurs logique

Soit <u>P</u> et <u>Q</u> 2 proposition logique du 1er ordre


![[logiqueBinaire | 512]]



# Les propriétés

Ont dit que deux énoncés sont dit équivalent si ils ont une même table de vérité. 
Soient P, Q, R trois proposition, alors ont a les propriétés suivantes.


* **La double négation**
  $$¬(¬p)⇔ p$$
* **La commutativité de ∧ et ∨** 
$$\begin{aligned}
		& (P ∧ Q) ⇔ (Q ∧ P)  \\
		& (P ∨ Q) ⇔ (Q ∨ P)
	\end{aligned}$$
* **L'associativités de ∧ et ∨**
  $$\begin{aligned}
	& (P ∧ (Q ∧ R)) ⇔ ((P ∧ Q) ∧ R)  \\
	& (P ∨ (Q ∨ R)) ⇔ ((P ∨ Q) ∨ R) 
\end{aligned}$$
* **La distributivités de ∧ et ∨**

$$\begin{aligned}
	& (P ∧ (Q ∨ R)) ⇔ ((P ∧ Q) ∨ (P ∧ R) \\
	& (P ∨ (Q ∧ R)) ⇔ ((P ∨ Q) ∧ (P ∨ R)
\end{aligned}$$
* **Loi de De Morgan**        
$$\begin{aligned}
		&  ¬(P ∨ Q) ⇔ (¬P ∧ ¬Q)  \\
		&  ¬(P ∧ Q) ⇔ (¬P ∨ ¬Q) 
	\end{aligned}$$
* **L'implication et sa négation**
$$\begin{aligned}
		&  (P ⇒ Q) ⇔ (¬P ∨ Q) \\
		&  ¬(P ⇒ Q) ⇔ (P ∧ ¬Q)
	\end{aligned}$$
* **L'équivalence et sa négation
$$\begin{aligned}
		&  (P ⇔ Q) ⇔ ((P ⇒ Q) ∧ (Q ⇒ P)) \\
		&   ¬(P ⇔ Q) ⇔ ((P ∧ ¬Q) ∨ (Q ∧ ¬P))
	\end{aligned}$$



# Le calcul des propositions 

Le calcul des propositions est une méthode qui fait abstraction de la structure interne des énoncés simple et se limite à étudier la relation entre la vérité / fausseté d'énoncé simple et élémentaire, avec comme objectif de pouvoir reconnaitre comme valide ou non certains raisonnement 

1. **L'expression propositionnelle**
   
	* C'est un énoncé complexe formé par combinaison d'énoncé élémentaire au moyen de connecteur logique 
	  
	* C'est donc une séquence de symbole pouvant appartenir à 3 groupe
			- les variables propositionnelles
			- les opérateur logique
			- les parenthèse


2. **Règles de syntaxe**
   
   * Une variable propositionnelle équivaut à une expression propositionnelle bien formé 
     
   * Si E est égale à une expression propositionnelle bien formé (EPBF) alors la négation de l'EPBF est égale à une EPBF
     
   * Si E et F sont des EPBF et c un connecteur logique alors E c F équivaut à une EPBF


3. **Construction d'une EPBF**

	* La construction d'une EPBF peut ce visualiser sous forme d'un arbre de graphe arborescent
	  ![[arbreEPBF | center]]
	* Évaluer une EPBF c'est indiquer la valeur de vérité qu'elle prend pour toutes les valeurs possibles 
	  ![[evaluationEPBF | center]]