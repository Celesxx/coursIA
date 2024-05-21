
# <span class="h1">Machine Learning</span>
#cours  #MachineLearning 

> [!summary] 
>  
*Le machine learning, est une sous-discipline de l'intelligence artificielle qui se concentre sur le développement d'algorithmes permettant aux ordinateurs d'apprendre à partir de données et de faire des prédictions ou des décisions sans être explicitement programmés pour effectuer ces tâches. Le machine learning repose sur des techniques statistiques et des méthodes d'optimisation pour ajuster des modèles mathématiques aux données observées.*

## <span class="h2">Introduction</span>


Le machine learning englobe diverses catégories, chacune possédant ses propres niveaux de complexité et étant adaptée à des cas d'utilisation spécifiques. Ces catégories permettent de répondre à des besoins variés allant de la simple classification et régression à des tâches plus complexes telles que la reconnaissance d'images ou la génération de textes.

![[ML-intro.excalidraw| 230 ]]

- <u>Apprentissage Supervisé : </u>Le modèle est entraîné sur des données étiquetées, c'est-à-dire des paires d'entrées et de sorties correctes. L'objectif est de prédire les sorties pour de nouvelles entrées. 
  <u>Exemples :</u> régression linéaire, arbres de décision, réseaux de neurones.
 
 - <u>Apprentissage Non Supervisé :</u> Le modèle est entraîné sur des données sans étiquettes. L'objectif est de découvrir des structures cachées ou des motifs dans les données. 
   <u>Exemples :</u> clustering, réduction de dimension, autoencodeurs.
    
- <u>Apprentissage par Renforcement :</u> Un agent apprend à prendre des décisions en interagissant avec un environnement et en recevant des récompenses ou des punitions en fonction de ses actions. 
  <u>Exemples :</u> Q-learning, Deep Q Networks (DQN).




## <span class="h2">Les caractéristiques du Machine Learning</span>


> [!summary] 
> *Le machine learning, est caractérisé par divers concepts fondamentaux comme le sous-apprentissage (underfitting) et le sur-apprentissage (overfitting) sont deux défis majeurs qui peuvent grandement affecter la performance d'un modèle. Comprendre et maîtriser ces concepts est crucial pour tout praticien du machine learning souhaitant construire des modèles précis et généralisables.* 


### <span class="h3">Sous-apprentissage</span>

Le sous-apprentissage, ou underfitting, se produit lorsque le modèle de machine learning est trop simple pour capturer les motifs et les tendances sous-jacents dans les données d'entraînement. Un modèle sous appris présente une erreur élevée à la fois sur les données d'entraînement et sur les données de test, car il n'a pas réussi à apprendre suffisamment d'informations pertinentes à partir des données.

<u>Signes de Sous-apprentissage :</u>

- Haute erreur de prédiction sur l'ensemble d'entraînement.
- Haute erreur de prédiction sur l'ensemble de test.
- Le modèle ne s'améliore pas même après une longue période d'entraînement.

<u>Solutions pour Éviter le Sous-apprentissage :</u>

- Utiliser un modèle plus complexe.
- Ajouter plus de caractéristiques pertinentes aux données d'entrée.
- Augmenter le temps d'entraînement ou utiliser un algorithme d'optimisation plus efficace.


### <span class="h3">Sur-apprentissage</span>

Le sur-apprentissage, ou overfitting, se produit lorsque le modèle de machine learning est trop complexe et s'ajuste trop étroitement aux données d'entraînement, y compris le bruit et les anomalies. Un modèle sur-appris performe très bien sur les données d'entraînement mais échoue à généraliser sur de nouvelles données, montrant une erreur élevée sur l'ensemble de test.

<u>Signes de Sur-apprentissage :</u>

- Très faible erreur de prédiction sur l'ensemble d'entraînement.
- Erreur de prédiction significativement plus élevée sur l'ensemble de test.
- Le modèle montre une grande variance lorsque de nouvelles données sont introduites.

<u>Solutions pour Éviter le Sur-apprentissage :</u>

- Utiliser la validation croisée pour évaluer la performance du modèle.
- Ajouter une régularisation (L1, L2) pour pénaliser les poids élevés.
- Simplifier le modèle en réduisant le nombre de paramètres ou de couches.
- Augmenter la taille de l'ensemble de données d'entraînement.


[[1.1-Modèle Linéaire]]