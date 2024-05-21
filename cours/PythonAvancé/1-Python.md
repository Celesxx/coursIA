
# <span class="h2">Python</span>

#cours #python

*Python est un langage de programmation de haut niveau, interprété et polyvalent, connu pour sa syntaxe claire et lisible. Créé par Guido van Rossum et publié pour la première fois en 1991.*

## <span class="h2">Concepts basiques</span>

Python met l'accent sur la lisibilité du code, ce qui permet aux développeurs de coder plus facilement et plus rapidement. Il possède de nombreuses caractéristiques distinctives :

- <span class="bold">Simplicité</span> : La syntaxe de Python est conçue pour être facile à lire et à écrire. Cela permet aux développeurs de se concentrer sur la résolution des problèmes plutôt que sur la syntaxe complexe.
- <span class="bold">Polyvalence :</span>  Python peut être utilisé pour une variété d'applications, y compris le développement web, l'analyse de données, l'intelligence artificielle, l'automatisation des tâches et plus encore.
- <span class="bold">Grande communauté : </span>Python bénéficie d'une large communauté de développeurs et de nombreuses ressources en ligne, y compris des bibliothèques et des frameworks pour presque tous les besoins.
- <span class="bold">Portabilité : </span>Python fonctionne sur presque toutes les plateformes, y compris Windows, macOS, Linux et même certaines plates-formes mobiles.

Python offre un environnement flexible et puissant pour développer une large gamme d'applications.




### <span class="h3">Définition d'une Classe</span>

Une **classe** en Python est un modèle pour créer des objets. Les classes encapsulent des données pour l'objet et des méthodes pour manipuler ces données. Exemple :

```python
class MyClass:
    pass
```





### <span class="h3">La Méthode `__init__` </span>

La méthode `__init__` initialise l'état de l'objet. Elle est appelée lorsqu'une instance (objet) de la classe est créée. Ici, self.value est une variable d'instance.

```python
class MyClass:     
	def __init__(self, value):         
		self.value = value
```





### <span class="h3">Instance</span>

Les variables d'instance sont des attributs d'une instance. Les méthodes sont des fonctions définies dans une classe.
- `value` est une variable d'instance.
- `display` est une méthode qui affiche la valeur de la variable d'instance.

```python
class MyClass:
    def __init__(self, value):
        self.value = value
    
    def display(self):
        print(self.value)
```







<span class="h3">Variables</span>

En Python, les variables peuvent contenir des données de différents types. Voici les types de variables les plus courants :

#### <span class="h4">Nombres Entiers (`int`)</span>
Les entiers sont des nombres sans virgule décimale.

```python
x = 10
y = -5
```

#### <span class="h4">Nombres à Virgule Flottante (`float`)</span>

Les flottants sont des nombres avec une virgule décimale.

```python
pi = 3.14
g = -9.81
```

#### <span class="h4">Chaînes de Caractères (`str`)</span>

Les chaînes de caractères sont des séquences de caractères.

```python
greeting = "Hello, World!"
name = 'Alice'
```

#### <span class="h4">Booléens (`bool`)</span>

Les booléens représentent des valeurs de vérité.

```python
is_active = True
is_deleted = False
```

#### <span class="h4">Listes (`list`)</span>

Les listes sont des collections ordonnées et modifiables d'éléments.

```python
numbers = [1, 2, 3, 4, 5]
names = ["Alice", "Bob", "Charlie"]
```

#### <span class="h4">Tuples (`tuple`)</span>

Les tuples sont des collections ordonnées et immuables d'éléments.

```python
coordinates = (10.0, 20.0)
colors = ("red", "green", "blue")
```

#### <span class="h4">Ensembles (`set`)</span>

Les ensembles sont des collections non ordonnées et sans doublons.

```python
nique_numbers = {1, 2, 3, 4, 5}
```

#### <span class="h4">Dictionnaires (`dict`)</span>

Les dictionnaires sont des collections non ordonnées de paires clé-valeur.

```python
person = {"name": "Alice", "age": 30, "city": "Paris"}

#exemple 
users = {
    "4e3abc": {
        "name": "John",
        "age": 20,
        "city": "Paris",
    },
    "5d68e7": {
        "name": "James",
        "age": 32,
        "city": "London",
    },
}
```







### <span class="h3">Conversion de Variables</span>

La conversion de variables, ou casting, consiste à changer le type d'une variable en un autre type. En Python, il existe plusieurs fonctions intégrées pour convertir des variables.

#### <span class="h4">Conversion en Entier (`int`)</span>

```python
x = int(3.14)     # x sera 3
y = int("42")     # y sera 42
```

#### <span class="h4">Conversion en Flottant (`float`)</span>

```python
x = float(3)      # x sera 3.0
y = float("42.5") # y sera 42.5
```

#### <span class="h4">Conversion en Chaîne de Caractères (`str`)</span>

```python
x = str(3.14)     # x sera "3.14"
y = str(42)       # y sera "42"
```

#### <span class="h4">Conversion en Booléen (`bool`)</span>

En Python, les valeurs suivantes sont considérées comme `False` : `None`, `False`, les nombres zéro, les séquences et collections vides (`''`, `[]`, `{}`, etc.). Toutes les autres valeurs sont considérées comme `True`.

```python
x = bool(0)       # x sera False
y = bool(42)      # y sera True
z = bool("")      # z sera False
w = bool("Hello") # w sera True
```

#### <span class="h4">Conversion en Liste (`list`)</span>

```python
x = list((1, 2, 3))   # x sera [1, 2, 3]
y = list("hello")     # y sera ['h', 'e', 'l', 'l', 'o']
```

#### <span class="h4">Conversion en Tuple (`tuple`)</span>

```python
x = tuple([1, 2, 3])  # x sera (1, 2, 3)
y = tuple("hello")    # y sera ('h', 'e', 'l', 'l', 'o')
```

#### <span class="h4">Conversion en Ensemble (`set`)</span>

```python
x = set([1, 2, 3, 3, 2, 1]) # x sera {1, 2, 3}
y = set("hello")            # y sera {'e', 'h', 'l', 'o'}
```

#### <span class="h4">Conversion en Dictionnaire (`dict`)</span>

Pour convertir en dictionnaire, il faut une structure appropriée, comme une liste de tuples à deux éléments.

```python
x = dict([("name", "Alice"), ("age", 30)])  # x sera {'name': 'Alice', 'age': 30}
```






### <span class="h3">Création d'Objets</span>

Un objet est créé en appelant la classe.

```python
obj = MyClass(10)
obj.display()  # Affiche : 10
```






### <span class="h3">Méthodes de Classe</span>

Les variables de classe sont partagées entre toutes les instances. Les méthodes de classe sont des méthodes qui opèrent sur la classe elle-même plutôt que sur une instance.
- `class_variable` est une variable de classe.
- `get_class_variable` est une méthode de classe.

```python
class MyClass:
    class_variable = 0
    
    def __init__(self, value):
        self.value = value
        MyClass.class_variable += 1
    
    @classmethod
    def get_class_variable(cls):
        return cls.class_variable
```



[[1.1-Fonction avancée]]
[[1.2-Fonction avancée - Type Checking]]