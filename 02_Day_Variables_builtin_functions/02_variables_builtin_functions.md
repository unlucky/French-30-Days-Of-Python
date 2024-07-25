<div align="center">
  <h1> 30 Days Of Python: Day 2 - Variables, Builtin Functions</h1>
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

[<< Day 1](../readme.md) | [Day 3 >>](../03_Day_Operators/03_operators.md)

![30DaysOfPython](../images/30DaysOfPython_banner3@2x.png)

- [📘 Jour 2](#-jour-2)
  - [Fonctions intégrées](#fonctions-intégrées)
  - [Variables](#variables)
    - [Déclarer plusieurs variables dans une ligne](#déclarer-plusieurs-variables-dans-une-ligne)
  - [Types de données](#types-de-données)
  - [Vérification des types de données et changements](#vérification-des-types-de-données-et-changements)
  - [Nombres](#nombres)
  - [💻 Exercises - Jour 2](#-exercises---jour-2)
    - [Exercises: Niveau 1](#exercises-niveau-1)
    - [Exercises: Niveau 2](#exercises-niveau-2)

# 📘 Jour 2

## Fonctions intégrées

En Python, nous disposons de nombreuses fonctions intégrées. Les fonctions intégrées sont globalement disponibles, ce qui signifie que vous pouvez les utiliser sans les importer ni les configurer. Les fonctions intégrées les plus couramment utilisées en Python sont les suivantes : _print()_, _len()_, _type()_, _int()_, _float()_, _str()_, _input()_, _list()_, _dict()_, _min()_, _max()_, _sum()_, _sorted()_, _open()_, _file()_, _help()_, et _dir()_. Le tableau suivant présente une liste exhaustive des fonctions intégrées de Python, tirée de la [documentation python](https://docs.python.org/3.9/library/functions.html).

![Built-in Functions](../images/builtin-functions.png)

Ouvrons l'interpréteur de commandes Python et commençons à utiliser certaines des fonctions intégrées les plus courantes.

![Built-in functions](../images/builtin-functions_practice.png)

Pratiquons davantage en utilisant différentes fonctions intégrées

![Help and Dir Built in Functions](../images/help_and_dir_builtin.png)

Comme vous pouvez le voir dans le terminal ci-dessus, Python possède des mots réservés. Nous n'utilisons pas de mots réservés pour déclarer des variables ou des fonctions. Nous aborderons les variables dans la section suivante.

Je pense que vous êtes maintenant familiarisé avec les fonctions intégrées. Pratiquons encore une fois les fonctions intégrées et nous passerons à la section suivante.

![Min Max Sum](../images/builtin-functional-final.png)

## Variables

Les variables stockent des données dans la mémoire d'un ordinateur. Il est recommandé d'utiliser des variables mnémoniques dans de nombreux langages de programmation. Une variable mnémotechnique est un nom de variable qui peut être facilement mémorisé et associé. Une variable fait référence à une adresse mémoire dans laquelle des données sont stockées.
Un numéro au début, un caractère spécial, un trait d'union ne sont pas autorisés pour nommer une variable. Une variable peut avoir un nom court (comme x, y, z), mais un nom plus descriptif (prénom, nom, âge, pays) est fortement recommandé.

Règles de désignation des variables Python

- Le nom d'une variable doit commencer par une lettre ou le caractère de soulignement.
- Un nom de variable ne peut pas commencer par un chiffre
- Un nom de variable ne peut contenir que des caractères alphanumériques et des traits de soulignement (A-z, 0-9 et \_ ).
- Les noms de variables sont sensibles à la casse (prénom, Prénom et PRENOM sont des variables différentes).

Voici quelques exemples de noms de variables valables :

```shell
firstname
lastname
age
country
city
first_name
last_name
capital_city
_if # if we want to use reserved word as a variable
year_2021
year2021
current_year_2021
birth_year
num1
num2
```

Noms de variables invalides

```shell
first-name
first@name
first$name
first name
num-1
1num
```

Nous utiliserons le style standard de désignation des variables Python, qui a été adopté par de nombreux développeurs Python. Les développeurs Python utilisent la convention de dénomination des variables snake case (snake_case). Nous utilisons le caractère de soulignement après chaque mot pour une variable contenant plus d'un mot (par exemple, prénom, nom, vitesse de rotation du moteur).  L'exemple ci-dessous est un exemple de dénomination standard des variables, le caractère de soulignement est nécessaire lorsque le nom de la variable contient plus d'un mot.

Lorsque nous attribuons un certain type de données à une variable, il s'agit d'une déclaration de variable. Par exemple, dans l'exemple ci-dessous, mon prénom est assigné à la variable first_name. Le signe égal est un opérateur d'affectation. Assigner signifie stocker des données dans la variable. Le signe égal en Python n'est pas une égalité comme en mathématiques.

_Example:_

```py
# Variables en Python
first_name = 'Asabeneh'
last_name = 'Yetayeh'
country = 'Finland'
city = 'Helsinki'
age = 250
is_married = True
skills = ['HTML', 'CSS', 'JS', 'React', 'Python']
person_info = {
   'firstname':'Asabeneh',
   'lastname':'Yetayeh',
   'country':'Finland',
   'city':'Helsinki'
   }
```

Utilisons les fonctions intégrées _print()_ et _len()_. La fonction Print prend un nombre illimité d'arguments. Un argument est une valeur qui peut être transmise ou placée entre les parenthèses de la fonction, voir l'exemple ci-dessous.

**Exemple:**

```py
print('Hello, World!') # Le texte Hello, World ! est un argument
print('Hello',',', 'World','!') # il peut prendre plusieurs arguments, quatre arguments ont été transmis
print(len('Hello, World!')) # il ne prend qu'un argument
```

Imprimons et trouvons également la longueur des variables déclarées en haut :

**Exemple:**

```py
# Affichage des valeurs stockées dans les variables

print('First name:', first_name)
print('First name length:', len(first_name))
print('Last name: ', last_name)
print('Last name length: ', len(last_name))
print('Country: ', country)
print('City: ', city)
print('Age: ', age)
print('Married: ', is_married)
print('Skills: ', skills)
print('Person information: ', person_info)
```

### Déclarer plusieurs variables dans une ligne

Plusieurs variables peuvent également être déclarées sur une même ligne :

**Exemple:**

```py
first_name, last_name, country, age, is_married = 'Asabeneh', 'Yetayeh', 'Helsink', 250, True

print(first_name, last_name, country, age, is_married)
print('First name:', first_name)
print('Last name: ', last_name)
print('Country: ', country)
print('Age: ', age)
print('Married: ', is_married)
```

Récupérer les données de l'utilisateur à l'aide de la fonction intégrée _input()_. Affectons les données obtenues d'un utilisateur aux variables first_name et age.
**Exemple:**

```py
first_name = input('What is your name: ')
age = input('How old are you? ')

print(first_name)
print(age)
```

## Types de données

Il existe plusieurs types de données en Python. Pour identifier le type de données, nous utilisons la fonction intégrée _type_. J'aimerais vous demander de vous concentrer sur la compréhension des différents types de données. Lorsqu'il s'agit de programmation, tout tourne autour des types de données. J'ai présenté les types de données au tout début et j'y reviens, car chaque sujet est lié aux types de données. Nous aborderons les types de données plus en détail dans leurs sections respectives.

## Vérification des types de données et changements

- Vérifier les types de données : Pour vérifier le type de données d'une certaine donnée/variable, nous utilisons la fonction _type_.
  **Exemple:**

```py
# Différents types de données en python
# Déclarons des variables avec différents types de données

first_name = 'Asabeneh'     # str
last_name = 'Yetayeh'       # str
country = 'Finland'         # str
city= 'Helsinki'            # str
age = 250                   # int, ce n'est pas mon âge réel, ne vous inquiétez pas.

# Printing out types
print(type('Asabeneh'))     # str
print(type(first_name))     # str
print(type(10))             # int
print(type(3.14))           # float
print(type(1 + 1j))         # complex
print(type(True))           # bool
print(type([1, 2, 3, 4]))     # list
print(type({'name':'Asabeneh','age':250, 'is_married':250}))    # dict
print(type((1,2)))                                              # tuple
print(type(zip([1,2],[3,4])))                                   # set
```

- Casting : Conversion d'un type de données en un autre type de données. Nous utilisons _int()_, _float()_, _str()_, _list_, _set_
  Lorsque nous effectuons des opérations arithmétiques, les chaînes de caractères doivent d'abord être converties en int ou en float, sous peine de générer une erreur. Si nous concaténons un nombre avec une chaîne de caractères, le nombre doit d'abord être converti en chaîne de caractères. Nous parlerons de la concaténation dans la section sur les chaînes de caractères.

  **Exemple:**

```py
# int to float
num_int = 10
print('num_int',num_int)         # 10
num_float = float(num_int)
print('num_float:', num_float)   # 10.0

# float to int
gravity = 9.81
print(int(gravity))             # 9

# int to str
num_int = 10
print(num_int)                  # 10
num_str = str(num_int)
print(num_str)                  # '10'

# str to int or float
num_str = '10.6'
print('num_int', int(num_str))      # 10
print('num_float', float(num_str))  # 10.6

# str to list
first_name = 'Asabeneh'
print(first_name)               # 'Asabeneh'
first_name_to_list = list(first_name)
print(first_name_to_list)            # ['A', 's', 'a', 'b', 'e', 'n', 'e', 'h']
```

## Nombres

Types de données numériques en Python:

1. Integers: Entiers (les nombres négatifs, nuls et positifs)
   Exemple:
   ... -3, -2, -1, 0, 1, 2, 3 ...

2. Float: Nombres à virgule (nombres décimaux)
   Exemple:
   ... -3.5, -2.25, -1.0, 0.0, 1.1, 2.2, 3.5 ...

3. Complex: Nombres complexe
   Exemple:
   1 + j, 2 + 4j, 1 - 1j

🌕 Vous êtes génial(e). Vous venez de relever les défis du deuxième jour et vous avez fait deux pas en avant sur la voie de la grandeur. Maintenant, fais quelques exercices pour ton cerveau et tes muscles.

## 💻 Exercises - Jour 2

### Exercises: Niveau 1

1. Dans 30DaysOfPython, créez un dossier appelé day_2. Dans ce dossier, créez un fichier nommé variables.py
2. Ecrivez un commentaire en python disant 'Day 2 : 30 Days of python programming' (Jour 2 : 30 jours de programmation en python)
3. Déclarez une variable prénom et attribuez-lui une valeur.
4. Déclarez une variable nom de famille et affectez-lui une valeur.
5. Déclarer une variable nom complet et lui affecter une valeur
6. Déclarer une variable pays et lui affecter une valeur
7. Déclarez une variable city et affectez-lui une valeur.
8. Déclarez une variable age et affectez-lui une valeur.
9. Déclarez une variable year et affectez-lui une valeur.
10. Déclarer une variable is_married et lui affecter une valeur.
11. Déclarer une variable is_true et lui affecter une valeur
12. Déclarer une variable is_light_on et lui affecter une valeur
13. Déclarer plusieurs variables sur une même ligne

### Exercises: Niveau 2

1. Vérifiez le type de données de toutes vos variables en utilisant la fonction intégrée type()
1. En utilisant la fonction intégrée _len()_, trouvez la longueur de votre prénom
1. Comparez la longueur de votre prénom et de votre nom de famille
1. Déclarez 5 comme num_one et 4 comme num_two
    1. Additionnez num_one et num_two et affectez la valeur à une variable total
    2. Soustraire num_two de num_one et affecter la valeur à une variable diff
    3. Multiplier num_two et num_one et affecter la valeur à une variable product
    4. Diviser num_one par num_two et affecter la valeur à une variable division
    5. Utiliser la division modulaire pour trouver num_two divisé par num_one et assigner la valeur à un reste variable.
    6. Calculer num_one à la puissance de num_two et affecter la valeur à une variable exp
    7. Trouver la division par le sol de num_one par num_two et assigner la valeur à une variable floor_division.
1. Le rayon d'un cercle est de 30 mètres.
    1. Calculez l'aire d'un cercle et affectez la valeur à une variable nommée _area_of_circle_
    2. Calculez la circonférence d'un cercle et affectez la valeur à une variable nommée _circum_of_circle_
    3. Prendre le rayon comme entrée utilisateur et calculer l'aire.
1. Utiliser la fonction d'entrée intégrée pour obtenir le prénom, le nom, le pays et l'âge d'un utilisateur et stocker la valeur dans les noms de variables correspondants.
1. Exécutez help('keywords') dans le shell Python ou dans votre fichier pour vérifier les mots réservés ou les mots-clés de Python.

🎉 FÉLICITATIONS ! 🎉

[<< Jour 1](../readme.md) | [Jour 3 >>](../03_Day_Operators/03_operators.md)
