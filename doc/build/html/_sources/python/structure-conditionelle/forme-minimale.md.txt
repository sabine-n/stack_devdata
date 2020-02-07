Documentation Python: Les structures conditionnelles
====================================================

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
-------------------------------------


La première ligne est un commentaire décrivant qu'il s'agit du premier test de condition. 
Elle est ignorée par l'interpréteur et sert juste à vous renseigner sur le code qui va suivre.
Cette ligne, vous devriez la comprendre sans aucune aide. On se contente d'affecter la valeur 5 à la variablea.
Ici se trouve notre test conditionnel. Il se compose, dans l'ordre :

Le mot clé "if" qui signifie « si » en anglais ;
de la condition proprement dite,a > 0, qu'il est facile de lire (une liste des opérateurs autorisés pour la comparaison sera présentée plus bas) ;
du signe deux points, « : », qui termine la condition et est indispensable : Python affichera une erreur de syntaxe si vous l'omettez.

Ici se trouve l'instruction à exécuter dans le cas oùaest supérieur à0. Après que vous ayez appuyé sur Entrée à la fin de la ligne précédente, l'interpréteur vous présente la série de trois points qui signifie qu'il attend la saisie du bloc d'instructions concerné avant de l'interpréter. Cette instruction (et les autres instructions à exécuter s'il y en a) est indentée, c'est-à-dire décalée vers la droite. Des explications supplémentaires seront données un peu plus bas sur les indentations.

L'interpréteur vous affiche à nouveau la série de trois points et vous pouvez en profiter pour saisir une nouvelle instruction dans ce bloc d'instructions. Ce n'est pas le cas pour l'instant. Vous appuyez donc sur Entrée sans avoir rien écrit et l'interpréteur vous affiche le message « a est supérieur à 0 », ce qui est assez logique vu queaest effectivement supérieur à 0.

Il y a deux notions importantes sur lesquelles je dois à présent revenir, elles sont complémentaires ne vous en faites pas.
La première est celle de bloc d'instructions. On entend par bloc d'instructions une série d'instructions qui s'exécutent dans un cas précis (par condition, comme on vient de le voir, par répétition, comme on le verra plus tard…). Ici, notre bloc n'est constitué que d'une seule instruction (la ligne 4 qui fait appel àprint). Mais rien ne vous empêche de mettre plusieurs instructions dans ce bloc.

```
>>> a = 5
>>>b = 8
>>>if a > 0:
    # On incrémente la valeur de b
   >>>b += 1
    # On affiche les valeurs des variables
   >>>print("a =",a,"et b =",b)
``` 

La seconde notion importante est celle d'indentation. On entend par indentation un certain décalage vers la droite, obtenu par un (ou plusieurs) espaces ou tabulations.
Les indentations sont essentielles pour Python. 
Il ne s'agit pas, comme dans d'autres langages tels que le C++ ou le Java, d'un confort de lecture mais bien d'un moyen pour l'interpréteur de savoir où se trouvent le début et la fin d'un bloc.

