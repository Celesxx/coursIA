|            | Tableau | Tableau trié | Liste chainé |
| ---------- | ------- | ------------ | ------------ |
| Recherche  | O(N)    | O(LogN)      | O(N)         |
| Ajout      | O(N)    | O(N)         | O(N)         |
| Suppéssion | O(N)    | O(N)         | O(N)         |

![[arbreBinaire.excalidraw]]

- Un noeud sans fils est une feuille (leaf)
	- Un noeud ne peut avoir qu'un seul père
	- le seul noeud sans père est appelé racine
- La taille d'un arbre est son nombre de noeud
- la hauteur d'un arbre est le nombre ma de déplacement entre la racine et une feuille
- Un arbre binaire est un entier si chaque noeud à 0 ou 2 fils



## Taille d'un arbre

###### La classe **Node**

Contient trois champs :

- **leftChild** : Node représentant le fils gauche
- **rightChild** : Node représentant le fils droit
- **value** : valeur du nœud, de type int/li>

```c
int treeSize(Node root)
{
    if(!root) return 0;
    else return treeSize(root->leftChild) + treeSize(root->rightChild) + 1;
}
```




```C
Cell merge(Cell a, Cell b)
{
	if(!a) return b;
	if(!b) return a;
	if(a->value < b-> value)
	{
		a->next = merge(a->next,b)
		return a;
	}
	b->next = merge(a, b->next)
	return b;
}
```


## parcours

![[arbreBinaireParcours.excalidraw 1 | 256]]

Parcours en largeur :
	- Niveau par niveau `G B H A E I C F D`
Parcours en profondeur : 
	- branche par branche de gauche à droite 
		- **Prefixe** : en SAG / SAD `B A E C D F H I`
		- **Suffixe** : SAG, SAD, noeud `A D C F E B I H G`
		- Infixe : SAG, noeud, SAD `A B C D E F G H I`
	