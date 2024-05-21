# <span class="h1">Dénombrement</span>

#mathematique #cours

## <span class="h2">Définitions</span>

- Une <span class="bold">p-liste</span> d'un ensemble E à $n_{element}$, c'est une suite de $p_{element} \in E$ distinct ou non. C'est une pioche aléatoire avec remise donc **répétition** et un **arrangement** dont la formule est $P_{liste} \in E = n^p$
	- <span class="bold">Exemple</span> E = {a, b, c, d, e} alors {a, b, c}, {a, a, b}, {e, e, e} sont 3 p-liste d'élément p et il y'en à $5^3 = 125$ 
	![[denombrementCours4.excalidraw| 150]]

- Un <span class="bold">Arrangement</span>  d'un ensemble E à $n_{element}$, c'est une suite ordonnée de $p_{element} \in E$ distinct ou $p \le n$. C'est donc une pioche **aléatoire** mais **sans remise** dont la formule est $E_{n}^p = \frac{n!}{n - p} = n(n-1)...(n-p+1)$ 
	- Exemple E = {a, b, c, d, e} alors {a, b, c}, {a, c, b}, {c, d, e} sont des arrangements à 3 éléments de E et il y'a $A_{n}^p = \frac{n!}{(n-p)!} = \frac{n * (n-1) * ...* (n - p + 1)(n-p)!}{(n-p)!}$
	![[denombrementCours1.excalidraw| center | 150]]
- Une <span class="bold">Permutation</span> d'un ensemble E à $n_{element}$ est un arrangement à $n_{element}$ . C'est un cas particulier de l'arrangement toujours sans remise dont la formule est $E_{n}^n = !n$
	- Exemple E = {a, b, c, d, e}, alors {a, b, c, d, e}, {b, c, a, e, d}, {c, a, b, d, e} sont des permutation de E et il y'a $5! = 120$
	![[denombrementCours3.excalidraw | 250]]
	

- Une <span class="bold">combinaison</span> de $p_{éléments}$ d'un ensemble E à $n_{éléments}$ toute partie de E à p éléments. On a obligatoirement $p \le n$. Une combinaison n'est donc pas ordonné c'est aussi sans remise. Pour chaque combinaison il y'a $p_{!arrangement}$ ce qui implique donc qu'il y'a $p!$ fois plus d'arrangement que de combinaisons. La formule de combinaison de $p_{éléments} pris parmi n est $C_{p}^n = \frac{A_{p}^n}{p!} = \frac{n!}{p!(n-p)!}$
	- <span class="bold">Exemple</span> E = {a, b, c, d, e} alors {a, b, c}, {a, b, d}, {a, b, e} sont des combinaisons à 3 éléments de E et il y'a $C_{5}^3 = \frac{60}{3!} = 10$ 
	![[denombrementCours2.excalidraw| 300]]

### <span class="h3">Propriétés</span>

Soit $(n, p) \in N^2$ tel que $p \le n$ on a :
	- $C_{n}^p = C_{n}^{n - p}$
	- avec $n,p != 0$, $C_{n}^p = C_{n-1}^{p} + C_{n-1}^{p- 1}$
	- avec $n,p != 0$, $pC_{n}^p = nC_{n-1}^{p- 1}$

## <span class="h2">Exercice</span>

### <span class="h3">Exercice 1</span>

1. <span class="bold">Sujet :</span> Combien de chaînes de n lettres peut-on construire avec des lettres prises dans l'alphabet E = {a, b, c} ? 
   
   - <span class="bold">Correction :</span> Il s'agit ici d'une pioche aléatoire et avec remise, c'est donc une **p-liste** et il y'a donc $3^n$ **p-liste** possible
    

2. <span class="bold">Sujet :</span> Etant donné un ensemble de n lettres différentes, combien peut-on construire de sous-ensembles ? 
   
   - <span class="bold">Correction :</span> le nombre de sous-ensemble dans un $n_{ensemble}$ c'est $2^n$
	 
   
3. <span class="bold">Sujet :</span> Etant donné une chaîne de n de 5 lettres différentes, combien peut-on construire de sous-chaînes de 5 lettres ? Rq : une sous-chaîne hérite de la chaîne principale, donc conserve les mêmes caractéristiques. 
   
   - <span class="bold">Correction :</span> c'est une pioche aléatoire mais sans remise, c'est donc un arrangement donc $2^n$ 
    
4. <span class="bold">Sujet : </span>Donner le nombre d'anagrammes du mot FACILE, puis du mot DIFFICILE. Ici, les anagrammes sont considérés comme des mots quelconques obtenus par permutation de lettres.
   
   - <span class="bold">Correction :</span> C'est une permutation car c'est une pioche aléatoire de taille à $n_{element}$ donc :
	   - Pour le mot **Facile** $A_{n}^n = n!$
	   - Pour le mot **Difficile** c'est $C_{9}^3 * C_{6}^2 * 4! = \frac{9*8*7}{3!} * \frac{6*5}{2!} * 4! = \frac{9!}{3!*2!} = \frac{9!}{12}$
	![[denombrementExo1part4.excalidraw 1 | 300]]



### <span class="h3">Exercice 2</span>

**Sujet** : Le digicode ci-dessous se trouve à l'entrée d'un immeuble. Pour ouvrir, il faut composer un code formé d'abord de deux lettres, puis de trois chiffres. Par exemple : CB445.

|  A  |  B  |  C  |
| :-: | :-: | :-: |
|  1  |  2  |  3  |
|  4  |  5  |  6  |
|  7  |  8  |  9  |

1. Déterminer le nombre total de codes possibles
2. Parmi ces codes, combien y'en a-t'il qui :
	- Ont leur trois chiffres pairs ?
	- Ont trois chiffres distincts ? 
	- Ont deux lettres distinctes et trois chiffres distincts, sans que les chiffres ne soient ordonnés ?
3. A l'aide du même digicode, déterminer le nombre total de codes en composant 2 lettres et 3 chiffres quelconques sans contrainte d'ordre d'apparition. Par exemple B44C5 et 445CB deviennent possibles

**Correction :**
1. Le nombre de 



1 - Le nombre total de code possible c'est $3^2 * 9^3 = 9 * 729 = 6561$ 

2.a - Il y'a 4 chiffre pair donc $3^2 * 4^3$ 
2.b - Il y'a  $3^2 * A_{9}^3 = 3^2 * \frac{9!}{6!} = 9 * 9 * 8 * 7$
2.c - Il y'a $A_{3}^2 * C_{9}^3 = 3! * \frac{{9*8*7}}{3!} = 9*8*7$

3- 


Exo 3 

1- C'est un n-list parce que l'on peut mettre dans le même tiroir donc $p^n$

2 - C'est un arrangement donc $A_{20}^{10} = \frac{20!}{10!} = 20 * 19 * 18 * 17 * 16 * 15 * 14 * 13 * 12 * 11$

3 - C'est une permutation de 5 donc $5! = 60$

4 - C'est une combinaison $C_{32}^2$

Exo 5 

Soit 
32 carte avec 4 couleur et 8 figures allant de 7 à l'as

1 - Le nombre de main est de $C_{4}^2 * C_{28}^{3}$

2 - Le nombre de main est de $C_{8}^1 * C_{28}^1$

3 - Le nombre de main est de $C_{8}^1 * C_{4}^3 * C_{7}^1 * C_{4}^2$

4 - Le nombre de main est de $C_{4}^2 * C_{8}^1 * \frac{C_{28}^1 * C_{24}^1 * C_{20}^1}{3!} = C_{4}^2 * C_{8}^1 * \frac{28*24*20}{3!}$

5- Le nombre de main est de 

$C_{8}^2 * C_{4}^2 * C_{4}^2 * C_{24}^1$



