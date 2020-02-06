Les structures conditionnelles
==============================

Créez des structures conditionnelles:
-------------------------------------


Vos premières conditions et blocs d'instructions
------------------------------------------------

Forme minimale en if 
--------------------

Les conditions sont un concept essentiel en programmation (oui oui, je me répète à force mais il faut avouer que des concepts essentiels, on n'a pas fini d'en voir). 
Elles vont vous permettre de faire une action précise si, par exemple, une variable est positive, une autre action si cette variable est négative, ou une troisième action si la variable est nulle. 
Comme un bon exemple vaut mieux que plusieurs lignes d'explications, voici un exemple clair d'une condition prise sous sa forme la plus simple.

Cela étant posé, revenons à nos conditions :

```
>>> # Premier exemple de condition
>>> a = 5
>>> if a > 0: # Si a est supérieur à 0
...     print("a est supérieur à 0.")
... 
a est supérieur à 0.
>>>
``` 

Détaillons ce code, ligne par ligne :

La première ligne est un commentaire décrivant qu'il s'agit du premier test de condition. 
Elle est ignorée par l'interpréteur et sert juste à vous renseigner sur le code qui va suivre.
Cette ligne, vous devriez la comprendre sans aucune aide. On se contente d'affecter la valeur 5 à la variablea.
Ici se trouve notre test conditionnel. Il se compose, dans l'ordre :

du mot cléifqui signifie « si » en anglais ;
de la condition proprement dite,a > 0, qu'il est facile de lire (une liste des opérateurs autorisés pour la comparaison sera présentée plus bas) ;
du signe deux points, « : », qui termine la condition et est indispensable : Python affichera une erreur de syntaxe si vous l'omettez.
Ici se trouve l'instruction à exécuter dans le cas oùaest supérieur à0. Après que vous ayez appuyé sur Entrée à la fin de la ligne précédente, l'interpréteur vous présente la série de trois points qui signifie qu'il attend la saisie du bloc d'instructions concerné avant de l'interpréter. Cette instruction (et les autres instructions à exécuter s'il y en a) est indentée, c'est-à-dire décalée vers la droite. Des explications supplémentaires seront données un peu plus bas sur les indentations.
L'interpréteur vous affiche à nouveau la série de trois points et vous pouvez en profiter pour saisir une nouvelle instruction dans ce bloc d'instructions. Ce n'est pas le cas pour l'instant. Vous appuyez donc sur Entrée sans avoir rien écrit et l'interpréteur vous affiche le message « a est supérieur à 0 », ce qui est assez logique vu queaest effectivement supérieur à0.
Il y a deux notions importantes sur lesquelles je dois à présent revenir, elles sont complémentaires ne vous en faites pas.
La première est celle de bloc d'instructions. On entend par bloc d'instructions une série d'instructions qui s'exécutent dans un cas précis (par condition, comme on vient de le voir, par répétition, comme on le verra plus tard…). Ici, notre bloc n'est constitué que d'une seule instruction (la ligne 4 qui fait appel àprint). Mais rien ne vous empêche de mettre plusieurs instructions dans ce bloc.

```
a = 5
b = 8
if a > 0:
    # On incrémente la valeur de b
    b += 1
    # On affiche les valeurs des variables
    print("a =",a,"et b =",b)
 ``` 

La seconde notion importante est celle d'indentation. On entend par indentation un certain décalage vers la droite, obtenu par un (ou plusieurs) espaces ou tabulations.
Les indentations sont essentielles pour Python. 
Il ne s'agit pas, comme dans d'autres langages tels que le C++ ou le Java, d'un confort de lecture mais bien d'un moyen pour l'interpréteur de savoir où se trouvent le début et la fin d'un bloc.

CONDITIONS :
----------

SYNTAX
------

Tous les programmes de la première leçon ont été exécutés séquentiellement, ligne après ligne. Aucune ligne
n'a pu être sautée.

Considérons le problème suivant: pour l'entier donné, X détermine sa valeur absolue. Si X> 0, le programme 
devrait imprimer la valeur X, sinon il devrait imprimer -X. Ce comportement ne peut pas être atteint à 
l'aide du programme séquentiel. Le programme doit sélectionner conditionnellement l'étape suivante. C'est 
là que les conditions aident:

:: 

x = -273
if x > 0:
    print(x)
else:
    print(-x)

:: 273

CONDITION if, else et elif
--------------------------

if, else
-------

Ce programme utilise une instruction conditionnelle if. Après le if nous mettons une condition (x > 0)
suivie par deux points. Après cela, nous mettons un bloc d'instructions qui ne seront exécutées que si la 
condition est vraie (c'est-à-dire évaluée à True). Ce bloc peut être suivi du mot else, deux points et d'un 
autre bloc d'instructions qui ne seront exécutées que si la condition est fausse (c'est-à-dire évaluée à 
False). Si c'est le cas ci-dessus, la condition est fausse, donc le bloc 'else' est exécuté. Chaque bloc 
doit être mis en retrait à l'aide d'espaces.

Pour résumer, l'instruction conditionnelle en Python a la syntaxe suivante:

::
if condition:
    true-block
    several instructions that are executed        
    if the condition evaluates to True
else:
    false-block
    several instructions that are executed
    if the condition evaluates to False

Dans cet exemple, la variable x n'est affectée -x qu'à si x < 0. En revanche, l'instruction print(x) est 
exécutée à chaque fois, car elle n'est pas en retrait, elle n'appartient donc pas au bloc «vrai».

L'indentation est un moyen général en Python de séparer des blocs de code. Toutes les instructions d'un 
même bloc doivent être mises en retrait de la même manière, c'est-à-dire qu'elles doivent avoir le même 
nombre d'espaces au début de la ligne. Il est recommandé d'utiliser 4 espaces pour l'indentation.

L'indentation est ce qui rend Python différent de la plupart des autres langages, dans lesquels les 
accolades {et }sont utilisés pour former les blocs.

Soit dit en passant, il existe une fonction intégrée pour la valeur absolue en Python:

::
    x = -273
    print(abs(x))

:: 273

elif
----

Si vous avez plus de deux options pour les distinguer à l'aide de l'opérateur conditionnel, vous pouvez 
utiliser l' if... elif... elseinstruction.

Montrons comment cela fonctionne en réécrivant l'exemple avec le point (x, y) sur le plan et les quadrants 
d'en haut:

::
    x = -5
    y = 7
    if x > 0 and y > 0:
        print("Quadrant I")
    elif x > 0 and y < 0:
        print("Quadrant IV")
    elif y > 0:
        print("Quadrant II")
    else:
        print("Quadrant III")

:: Quadrant II

CONDITIONS IMBRIQUÊES
---------------------

Toute instruction Python peut être placée dans des blocs «vrais» et «faux», y compris une autre instruction 
conditionnelle. De cette façon, nous obtenons des conditions imbriquées. Les blocs de conditions internes 
sont indentés en utilisant deux fois plus d'espaces (par exemple 8 espaces). Voyons un exemple. Étant donné 
les coordonnées du point sur le plan, imprimez son quadrant.

::
    x = 2
    y = -3
    if x > 0:
        if y > 0:
            # x is greater than 0, y is greater than 0
            print("Quadrant I")
        else:    
            # x is greater than 0, y is less or equal than 0
            print("Quadrant IV")
    else:
        if y > 0:
            # x is less or equal than 0, y is greater than 0
            print("Quadrant II")
        else:    
            # x is less or equal than 0, y is less or equal than 0
            print("Quadrant III")

:: Quadrant IV



OPÊRATEURS DE COMPARAISON
-------------------------

Habituellement, la condition après ifpossède un ou plusieurs des opérateurs suivants:

<
less  - la condition est vraie si le côté gauche est inférieur au côté droit.
>
supérieur  - la condition est vraie si le côté gauche est supérieur au côté droit.
<=
inférieur ou égal.
>=
supérieur ou égal.
==
égal.
!=
inégal

OBJETS BOOLÊENS ET OPÊRATEURS LOGIQUES
--------------------------------------

Lorsque nous additionnons deux objets entiers en utilisant l' +opérateur, comme 2 + 5, nous obtenons un 
nouvel objet: 7. De la même manière, si l' on compare deux entiers à l' aide de l' <opérateur, comme 2 < 5, 
nous obtenons un nouvel objet: True.

::
    print(2 < 5)
    print(2 > 5)

::
    True
    False

    Les objets Trueet Falseont un type spécial appelé bool. Comme chaque nom de type peut être utilisé pour 
    convertir des objets en ce type, voyons ce que cette distribution donne pour les nombres:

::
    print(bool(-10))    
    print(bool(0))      
    print(bool(10))     

    print(bool(''))     
    print(bool('abc'))  

:: 
    False
    True
    False
    True

Parfois, vous devez vérifier plusieurs conditions à la fois. Par exemple, vous pouvez vérifier si un nombre 
nest divisible par 2 en utilisant la condition n % 2 == 0 ( ndonne un reste 0lors de la division par 2). Si 
vous devez vérifier que les deux chiffres net msont à la fois divisble par 2, vous devriez vérifier à la 
fois n % 2 == 0 et m % 2 == 0. Pour ce faire, vous joindre à eux à l' aide d' un opérateur and (logique): n 
% 2 == 0 and m % 2 == 0.

Python a un ET logique, un OU logique et une négation.

L'opérateur andest un opérateur binaire qui évalue True si et seulement si son côté gauche et son côté 
droit le sont True.

L'opérateur orest un opérateur binaire qui évalue True si au moins un de ses côtés l'est True.

L'opérateur notest une négation unaire, il est suivi d'une certaine valeur. Il est évalué Truesi cette 
valeur est Falseet vice versa.

Vérifions qu'au moins l'un des deux nombres se termine par 0:

:: 
    a = 15
    b = 40
    if a % 10 == 0 or b % 10 == 0:
        print('YES')
    else:
        print('NO')

::
    YES


[comment] <> (LOTFI) 

Mots clés Python :
------------------


AND:
----

Synthaxe:
booleen et entier

En booléen, ce parametre permet d'indiquer une expression de type booléen avec lequel un "et logique" est effectué.

En entier , ce parametre permet d'indiquer une expression de type entiere avec lequel un "et binaire" est effectué .

Ce mot réservé permet d'indiquer une opération de «Et logique» ou de «Et binaire».

OR:
---

Synthaxe :
booléen et entier

En booléence parametre permet d'indiquer une expression de type booléen avec lequel  un "Ou logique" est effectué.
En entier , ce parametre permet d'indiquer une expression de type entiere avec lequel un "Ou binaire" est effectué.
Ce mot réservé permet d'indiquer une opération de «Ou logique» ou «Ou binaire».

NOT:
----
Synthaxe:
not exp

exp , ce parametre permet d'indiquer l'expression à traiter.
Ce mot réservé permet d'effectuer un Non logique sur des booléens ou Non binaire sur des valeurs numériques.




[comment] <> (LOTFI) 

Mots clés Python :
----------------


AND:
----

Synthaxe:
booleen et entier

En booléen, ce parametre permet d'indiquer une expression de type booléen avec lequel un "et logique" est effectué.

En entier , ce parametre permet d'indiquer une expression de type entiere avec lequel un "et binaire" est effectué .

Ce mot réservé permet d'indiquer une opération de «Et logique» ou de «Et binaire».

OR:
---

Synthaxe :
booléen et entier

En booléence parametre permet d'indiquer une expression de type booléen avec lequel  un "Ou logique" est effectué.
En entier , ce parametre permet d'indiquer une expression de type entiere avec lequel un "Ou binaire" est effectué.
Ce mot réservé permet d'indiquer une opération de «Ou logique» ou «Ou binaire».

NOT:
----
Synthaxe:
not exp

exp , ce parametre permet d'indiquer l'expression à traiter.
Ce mot réservé permet d'effectuer un Non logique sur des booléens ou Non binaire sur des valeurs numériques.






