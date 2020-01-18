Ligne de commande git tag
=========================

voici quelques ligne de commande de git tag :

* Pour créer un tag sur votre branche actuelle:
    
    git tag < tagname >

Cela créera une tag locale avec l'état actuel de la branche sur laquelle vous vous trouvez.

* Pour créer une balise avec un commit:
    
    git tag tag-name commit-identifier

Cela créera une tag locale avec l'identificateur de validation de la branche sur laquelle vous vous trouvez.

* push un commit dans GIT:
    
    git push origin tag-name

* push  toutes les étiquettes à la fois
    
    git push origin --tags