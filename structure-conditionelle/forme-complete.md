CONDITIONS:
===========

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
~~~~~~~~

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
~~~~

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
