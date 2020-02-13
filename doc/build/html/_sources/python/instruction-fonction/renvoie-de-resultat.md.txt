Renvoi des résultat 
----------------------
		
**Python permet aux fonctions de renvoyer plusieurs objets a la fois comme sur l'exemple ci dessous**


    ***1->>> def  carre_cube(x):
    2-...return x**2, x**33...
    4->>> carre_cube (2)
    5-(4, 8)***

**En réalité Python ne renvoie qu’un seul objet, mais celui-ci a la possibilité d'etre séquentiel, donc de contenir lui même d’autres objets.
Exemple ou Python renvoie un objet de type tuple :**


    ***1>>> def  carre_cube2(x):
    2...return [x**2, x**3]
    3...
    4>>> carre_cube2 (3)
    5[9, 27]***

**Le fait de renvoyer un tuple ou une liste de deux éléments (ou plus) est très pratique en conjonction avec l’affectation multiple, par exemple :**


    ***1>>> z1 , z2 = carre_cube2 (3)
    2>>> z1
     39
    4>>> z25
     27***
 

**Donc on peut récupérer plusieurs valeurs renvoyées par une fonction et de les affecter à la volée à des variables différentes.**


