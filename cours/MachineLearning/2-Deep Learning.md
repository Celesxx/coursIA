# <span class="h1">Deep Learning</span>

#cours #MachineLearning 


> [!summary] 
> *Le deep learning, ou apprentissage profond, est une sous-discipline du machine learning qui repose sur l'utilisation de réseaux de neurones artificiels composés de plusieurs couches. Cette approche permet de modéliser des relations complexes dans les données, et est particulièrement efficace pour les tâches qui impliquent de grandes quantités de données non structurées telles que des images, des sons et des textes. *

### <span class="h2">Neurone Artificiel (Perceptron)</span>

> [!summary] 
> Les neurones artificiels sont les unités fondamentales des réseaux de neurones en deep learning, inspirés par la structure et le fonctionnement des neurones biologiques. Ces neurones sont les éléments de base qui, en se combinant en couches et en réseaux, permettent aux modèles de deep learning de réaliser des tâches complexes d'apprentissage automatique. 

## <span class="h3">Théorème d'Approximation Universelle</span>

- Le théorème d'approximation universelle, formulé par Cybenko en 1989, stipule qu'un réseau de neurones avec une seule couche cachée de neurones sigmoïdes peut approximer toute fonction continue définie sur un ensemble borné avec une précision arbitraire, à condition que le nombre de neurones soit suffisant.

- Ce théorème a été renforcé par Sussman en 1992, qui a démontré que les réseaux à une couche cachée sont des approximateurs parsimonieux, capables d'approcher correctement plus de fonctions qu'un polynôme avec un nombre égal de paramètres. 


### <span class="h3">Fonctionnement</span>

> [!info] 
> Chaque neurone prend une combinaison linéaire des entrées pondérées et applique une fonction d'activation pour produire une sortie non linéaire. 


![[neural.excalidraw | 600]]



#### <span class="h4">Composants d'un Neurone Artificiel</span>

1. <u>Entrées (Inputs) :</u> Les neurones reçoivent des signaux d'entrée $x_1\dots x_n$ provenant de la couche précédente (ou des données d'entrée initiales pour les neurones de la première couche) et chaque entrée est associée à un poids

2. <u>Poids (Weights) :</u>Les poids $w_1 \dots w_n​$ modulent la force de chaque signal d'entrée. Ils sont ajustés pendant le processus d'apprentissage pour minimiser l'erreur de prédiction du modèle.

3. <u>Biais (Bias) :</u> Un neurone possède également un biais $b$ qui est ajouté à la combinaison pondérée des entrées. Le biais permet de décaler la fonction d'activation, ce qui permet au modèle de mieux s'ajuster aux données.

4. <u>Combinaison Linéaire :</u>Le neurone calcule une somme pondérée des entrées et du biais
$$\sum\limits_{k=0}^x w_k x_k + b$$
5. <u>Fonction d'Activation (Activation Function) :</u> La combinaison linéaire $z$ est ensuite passée à travers une fonction d'activation non linéaire ($sigmoide, tanh, relu$) pour produire la sortie du neurone.

6. <u>Sortie (Output) :</u> La sortie du neurone après application de la fonction d'activation est transmise soit à la couche suivante (dans les réseaux multicouches), soit utilisée comme sortie finale du réseau (dans la dernière couche).



### <span class="h3">Caractéristiques des Neurones en Deep Learning</span>

> [!info] 
> Les neurones artificiels constituent les éléments fondamentaux des réseaux de neurones en deep learning. En se combinant en couches et en réseaux, les neurones permettent de modéliser des relations complexes dans les données, facilitant ainsi la résolution de problèmes complexes d'apprentissage automatique. 

- <u>Non-Linéarité :</u> Les fonctions d'activation introduisent de la non-linéarité, permettant au réseau de modéliser des relations complexes entre les entrées et les sorties.

- <u>Apprentissage Hiérarchique :</u> Dans les réseaux profonds, les neurones des couches supérieures peuvent apprendre des représentations hiérarchiques des données, où chaque couche extrait des caractéristiques de plus en plus abstraites.

- <u>Robustesse et Capacité de Généralisation :</u> En ajustant les poids et les biais, les neurones permettent au modèle de s'adapter aux données d'entraînement et de généraliser à de nouvelles données non vues.

- <u>Interconnectivité :</u> Les neurones sont fortement interconnectés, chaque neurone d'une couche étant connecté à chaque neurone de la couche suivante dans un réseau de neurones dense


### <span class="h3">Types de Neurones et Réseaux</span>

> [!info] 
> En deep learning, les neurones artificiels sont les éléments de base des réseaux de neurones, et ils se déclinent en plusieurs types adaptés à différentes tâches. Ces types de neurones, avec leurs architectures spécifiques, permettent de résoudre des problèmes complexes dans des domaines variés tels que la vision par ordinateur et le traitement du langage naturel. 

[[2.2-Regression linéaire]]
[[2.3-Perceptron multi couche]]
[[2.4-Radial Basis Function]]
