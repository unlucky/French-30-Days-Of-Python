<div align="center">
  <h1> 30 Days Of Python: Day 3 - Operators</h1>
  <a class="header-badge" target="_blank" href="https://www.linkedin.com/in/asabeneh/">
  <img src="https://img.shields.io/badge/style--5eba00.svg?label=LinkedIn&logo=linkedin&style=social">
  </a>
  <a class="header-badge" target="_blank" href="https://twitter.com/Asabeneh">
  <img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/asabeneh?style=social">
  </a>

<sub>Author:
<a href="https://www.linkedin.com/in/asabeneh/" target="_blank">Asabeneh Yetayeh</a><br>
<small> Second Edition: July, 2021</small>
</sub>
</div>

[<< Jour 2](../02_Day_Variables_builtin_functions/02_variables_builtin_functions.md) | [Jour 4 >>](../04_Day_Strings/04_strings.md)

![30DaysOfPython](../images/30DaysOfPython_banner3@2x.png)

- [📘 Jour 3](#jour-3)
  - [Booléen](#booléen)
  - [Opérateurs](#opérateurs)
    - [Opérateurs affectation](#opérateurs-affectation)
    - [Opérateurs arithmétiques](#opérateurs-arithmétiques)
    - [Opérateurs de comparaison](#opérateurs-de-comparaison)
    - [Opérateurs logiques](#opérateurs-logiques)
  - [💻 Exercices - Jour 3](#-exercices--jour-3)

# 📘 Day 3

## Booléen

Un type de données booléen représente l'une des deux valeurs suivantes : _True_ ou _False_. L'utilisation de ces types de données sera claire lorsque nous commencerons à utiliser l'opérateur de comparaison. La première lettre **T** pour True et **F** pour False doit être en majuscule contrairement à JavaScript.
**Exemple : Valeurs booléennes**

```py
print(True)
print(False)
```

## Opérateurs

Le langage Python prend en charge plusieurs types d'opérateurs. Dans cette section, nous nous concentrerons sur quelques-uns d'entre eux.

### Opérateurs affectation

Les opérateurs d'affectation sont utilisés pour attribuer des valeurs aux variables. Prenons l'exemple de =. En mathématiques, le signe égal indique que deux valeurs sont égales, mais en Python, il signifie que nous stockons une valeur dans une certaine variable et nous l'appelons affectation ou assignation d'une valeur à une variable. Le tableau ci-dessous présente les différents types d'opérateurs d'affectation en Python, tirés de [w3school](https://www.w3schools.com/python/python_operators.asp).

![Assignment Operators](../images/assignment_operators.png)

### Opérateurs arithmétiques:

- Addition(+): a + b
- Subtraction(-): a - b
- Multiplication(*): a * b
- Division(/): a / b
- Modulus(%): a % b
- Floor division(//): a // b
- Exponentiation(**): a ** b

![Arithmetic Operators](../images/arithmetic_operators.png)

**Exemple : nombres entiers**

```py
# Opérations arithmétiques en Python
# Integers

print('Addition: ', 1 + 2)        # 3
print('Subtraction: ', 2 - 1)     # 1
print('Multiplication: ', 2 * 3)  # 6
print ('Division: ', 4 / 2)       # 2.0  La division en Python donne un float
print('Division: ', 6 / 2)        # 3.0
print('Division: ', 7 / 2)        # 3.5
print('Division without the remainder: ', 7 // 2)   # 3,  donne sans le nombre flottant ou sans le reste
print ('Division without the remainder: ',7 // 3)   # 2
print('Modulus: ', 3 % 2)         # 1, Donne le reste
print('Exponentiation: ', 2 ** 3) # 9 cela signifie 2 * 2 * 2
```

**Exemple : Floats**

```py
# Nombres flottants
print('Floating Point Number, PI', 3.14)
print('Floating Point Number, gravity', 9.81)
```

**Exemple : Nombres complexes**

```py
# Nombres complexes
print('Complex number: ', 1 + 1j)
print('Multiplying complex numbers: ',(1 + 1j) * (1 - 1j))
```

Déclarons une variable et attribuons-lui un type de données numérique. Je vais utiliser une variable à caractère unique, mais n'oubliez pas de ne pas prendre l'habitude de déclarer ce type de variables. Les noms de variables doivent toujours être mnémotechniques.

**Exemple:**

```python
# Déclarer d'abord la variable en haut de page

a = 3 # a est un nom de variable et 3 est un type de données entier
b = 2 # b est un nom de variable et 3 est un type de données entier

# Opérations arithmétiques et affectation du résultat à une variable
total = a + b
diff = a - b
product = a * b
division = a / b
remainder = a % b
floor_division = a // b
exponential = a ** b

# J'aurais dû utiliser sum au lieu de total, mais sum est une fonction intégrée - essayez d'éviter d'écraser les fonctions intégrées.
print(total) # si vous n'étiquetez pas votre affichage avec une chaîne de caractères, vous ne saurez jamais d'où vient le résultat
print('a + b = ', total)
print('a - b = ', diff)
print('a * b = ', product)
print('a / b = ', division)
print('a % b = ', remainder)
print('a // b = ', floor_division)
print('a ** b = ', exponentiation)
```

**Exemple:**

```py
print('== Addition, Subtraction, Multiplication, Division, Modulus ==')

# Déclarer des valeurs et les organiser ensemble
num_one = 3
num_two = 4

# Opérations arithmétiques
total = num_one + num_two
diff = num_two - num_one
product = num_one * num_two
div = num_two / num_one
remainder = num_two % num_one

# Impression des valeurs avec étiquette
print('total: ', total)
print('difference: ', diff)
print('product: ', product)
print('division: ', div)
print('remainder: ', remainder)
```

Commençons à relier les points et à utiliser ce que nous savons déjà calculer (surface, volume, densité, poids, périmètre, distance, force).

**Exemple:**

```py
# Calculer l'aire d'un cercle
radius = 10                                 # rayon d'un cercle
area_of_circle = 3.14 * radius ** 2         # deux * signifient exposant ou puissance
print('Area of a circle:', area_of_circle)

# Calculer l'aire d'un rectangle
length = 10
width = 20
area_of_rectangle = length * width
print('Area of rectangle:', area_of_rectangle)

# Calculer le poids d'un objet
mass = 75
gravity = 9.81
weight = mass * gravity
print(weight, 'N')                         # Ajouter une unité au poids

# Calculer la densité d'un liquide
mass = 75 # en kg
volume = 0.075 # en mètre cube
density = mass / volume # 1000 Kg/m^3

```

### Opérateurs de comparaison

En programmation, nous comparons des valeurs, nous utilisons des opérateurs de comparaison pour comparer deux valeurs. Nous vérifions si une valeur est supérieure, inférieure ou égale à une autre valeur. Le tableau suivant présente les opérateurs de comparaison Python, tirés de [w3shool](https://www.w3schools.com/python/python_operators.asp).

![Comparison Operators](../images/comparison_operators.png)
**Exemple : Opérateurs de comparaison**

```py
print(3 > 2) # True, car 3 est plus grand que 2
print(3 >= 2) # True, car 3 est plus grand que 2
print(3 < 2) # False, car 3 est plus grand que 2
print(2 < 3) # True, car 2 est inférieur à 3
print(2 <= 3) # True, car 2 est inférieur à 3
print(3 == 2) # False, car 3 n'est pas égal à 2
print(3 != 2) # True, car 3 n'est pas égal à 2
print(len('mango') == len('avocado'))  # False
print(len('mango') != len('avocado'))  # True
print(len('mango') < len('avocado'))   # True
print(len('milk') != len('meat'))      # False
print(len('milk') == len('meat'))      # True
print(len('tomato') == len('potato'))  # True
print(len('python') > len('dragon'))   # False


# En comparant quelque chose, on obtient un True ou un False.

print('True == True: ', True == True)
print('True == False: ', True == False)
print('False == False:', False == False)
```

En plus de l'opérateur de comparaison ci-dessus, Python utilise :

- _is_ : Retourne vrai si les deux variables sont le même objet(x is y)
- _is not_ : Retourne vrai si les deux variables ne sont pas le même objet (x n'est pas y)
- _in_ : Retourne True si la liste interrogée contient un certain élément(x in y)
- _not in_ : Retourne True si la liste interrogée ne contient pas un certain élément(x in y)

```py
print('1 is 1', 1 is 1)                   # True - parce que les valeurs des données sont les mêmes
print('1 is not 2', 1 is not 2)           # True - parce que 1 n'est pas 2
print('A in Asabeneh', 'A' in 'Asabeneh') # True - A trouvé dans la chaîne
print('B in Asabeneh', 'B' in 'Asabeneh') # False - il n'y a pas de B majuscule
print('coding' in 'coding for all') # True - parce que coding for all contient le mot coding
print('a in an:', 'a' in 'an')      # True
print('4 is 2 ** 2:', 4 is 2 ** 2)   # True
```

### Opérateurs logiques

Contrairement à d'autres langages de programmation, Python utilise les mots-clés _and_, _or_ et _not_ pour les opérateurs logiques. Les opérateurs logiques sont utilisés pour combiner des déclarations conditionnelles :

![Logical Operators](../images/logical_operators.png)

```py
print(3 > 2 and 4 > 3) # True - parce que les deux déclarations sont vraies
print(3 > 2 and 4 < 3) # False - parce que la deuxième affirmation est fausse
print(3 < 2 and 4 < 3) # False - parce que les deux déclarations sont fausses
print('True et True : ', True and True)
print(3 > 2 or 4 > 3) # True - parce que les deux déclarations sont vraies
print(3 > 2 or 4 < 3) # True - parce que l'une des affirmations est vraie
print(3 < 2 or 4 < 3) # False - parce que les deux déclarations sont fausses
print('True ou False:', True or False)
print(not 3 > 2) # False - parce que 3 > 2 est vrai, alors not True donne False
print(not True) # False - La négation, l'opérateur not transforme true en false
print(not False) # True
print(not not True) # True
print(not not False) # False
```

🌕 Vous avez une énergie débordante. Vous venez de relever les défis du troisième jour et vous avez fait trois pas en avant sur la voie de la grandeur. Maintenant, faites quelques exercices pour votre cerveau et vos muscles.

## 💻 Exercises - Jour 3

1. Déclarez votre âge comme une variable entière
2. Déclarez votre taille comme une variable flottante
3. Déclarez une variable qui stocke un nombre complexe
4. Ecrivez un script qui demande à l'utilisateur d'entrer la base et la hauteur du triangle et calculez l'aire de ce triangle (aire = 0,5 x b x h).

```py
    Enter base: 20
    Enter height: 10
    The area of the triangle is 100
```

5. Écrivez un script qui invite l'utilisateur à saisir le côté a, le côté b et le côté c du triangle. Calculez le périmètre du triangle (périmètre = a + b + c).

```py
Enter side a: 5
Enter side b: 4
Enter side c: 3
The perimeter of the triangle is 12
```

6. Obtenir la longueur et la largeur d'un rectangle à l'aide de l'invite. Calculez sa surface (surface = longueur x largeur) et son périmètre (périmètre = 2 x (longueur + largeur)).
7. Obtenez le rayon d'un cercle à l'aide de l'invite. Calculez l'aire (aire = pi x r x r) et la circonférence (c = 2 x pi x r) où pi = 3,14.
8. Calculez la pente, l'ordonnée à l'origine et l'ordonnée à l'origine de y = 2x -2.
9. La pente est (m = y2-y1/x2-x1). Trouvez la pente et la [distance euclidienne] (https://en.wikipedia.org/wiki/Euclidean_distance#:~:text=In%20mathematics%2C%20the%20Euclidean%20distance,being%20called%20the%20Pythagorean%20distance.) entre le point (2, 2) et le point (6,10).
10. Comparez les pentes dans les tâches 8 et 9.
11. Calculez la valeur de y (y = x^2 + 6x + 9). Essayez d'utiliser différentes valeurs de x et de déterminer à quelle valeur de x y sera égal à 0.
12. Trouvez la longueur de « python » et de « dragon » et faites une déclaration de comparaison fiable.
13. Utilisez l'opérateur _et_ pour vérifier si « on » se trouve à la fois dans « python » et dans « dragon
14. Le système de gestion de l'information est un système de gestion de l'information qui permet à l'utilisateur d'avoir accès à l'information. Utilisez l'opérateur _in_ pour vérifier si _jargon_ se trouve dans la phrase.
15. Il n'y a pas de « on » dans dragon et python.
16. Trouvez la longueur du texte _python_ et convertissez la valeur en float et convertissez-la en chaîne de caractères.
17. Les nombres pairs sont divisibles par 2 et le reste est zéro. Comment vérifier si un nombre est pair ou non en utilisant python ?
18. Vérifiez si la division floor de 7 par 3 est égale à la valeur convertie int de 2.7.
19. Vérifiez si le type '10' est égal au type 10.
20. Vérifier si int('9.8') est égal à 10
21. Rédigez un script qui invite l'utilisateur à saisir les heures et le taux horaire. Calculez la rémunération de la personne ?

```py
Enter hours: 40
Enter rate per hour: 28
Your weekly earning is 1120
```

22. Écrire un script qui invite l'utilisateur à entrer le nombre d'années. Calculez le nombre de secondes qu'une personne peut vivre. Supposons qu'une personne puisse vivre cent ans

```py
Enter number of years you have lived: 100
You have lived for 3153600000 seconds.
```

23. Écrivez un script Python qui affiche le tableau suivant

```py
1 1 1 1 1
2 1 2 4 8
3 1 3 9 27
4 1 4 16 64
5 1 5 25 125
```

🎉 FÉLICITATIONS ! 🎉

[<< Jour 2](../02_Day_Variables_builtin_functions/02_variables_builtin_functions.md) | [Jour 4 >>](../04_Day_Strings/04_strings.md)
