Que peut-on faire avec Python?
===============================

Avec python on peut faire beaucoup de choses voici quelques exemple :

du calcul scientifique (librairie pandas, numpy)
-------------------------------------------------
::

    >>> import pandas # on importe la biblitéque pandas

    from pandas import Series

    import numpy

    s = Series([42, 'Hello World!', 3.14, -5, None, numpy.nan])

    s.head()

résultat:

::

   >>>  0              42
        1    Hello World!
        2            3.14
        3              -5
        4            None
        dtype: object



des graphiques (librairie matplotlib) et (sous librairie pyplot)
----------------------------------------------------------------
::

    >>> mport pandas as pd #importer pandas
    import matplotlib.pyplot as plt #importer mathplitlib

    liste=["mpg","cylindres","déplacement","puissance","poids","accélération","année de modèle","origine",
    "nom de la voiture)"] #crée une liste

    plt.figure(figsize=(7,7))#pour gérer la taille du graphique 
    auto=pd.read_excel('/home/hachem/Documents/autompg.xlsx', sep= '\t', names =liste)
    auto['année de modèle'].value_counts().plot.pie()#diagramme à secteur *

résultat:

 ::   
 
    >>> <matplotlib.axes._subplots.AxesSubplot at 0x7fcb00bec210>

..  image:: output_19_1.png
    :width: 400




    

