# Modèle Logique des Données (MLD)

On a vu précedemment comment le MCD nou permet de définir le concept sur lequelle sera construite notre future base de donnée. C'est à partir du modèle conceptuel des données qu'on va pouvoir passer au modèle logique des données. Ce dernier va nous permettre de modéliser la structure selon laquelle les données seront stockées dans la future base de donnée. Donc on passe du concept à l'adaptation technique. En particulier, il s'agit de l'organisation des données en utilisant de tableaux à deux dimensions et de formaliser la manipulation des données réparties sur plusieurs tables.

## Les dépendances fonctionnelles

Les dépendances fonctionnelles servent à définir les liens entre les métadonnées définis précédemment. Ces métadonnées seront nommées attributs.

### Dépendances entre attributs

Formellement, on dit qu'il existe une dépendance fonctionnelle entre deux attributs X et Y liés par une relation R, si la connaissance d'une valeur de X determine au plus une valeur de Y.

Exemple : Il existe une dépendance fonctionelle entre les attributs "*immatriculation*" et "*marque de voiture*" parce que la connaissance du numéro d'immatriculation d'une voiture implique directement la connaissance de la marque de la voiture. A noter que l'inverse n'est pas vrai.

Pour trouver les différentes dépendances entre attributs on peut créer un tableau à deux entrées où l'on liste les métadonnées à la fois dans la première ligne et la première colonne. Notez bien que l'on peut lister toutes les métadonées mais dans le cas de bases de données énormes, il faut simplifier, c'est-à-dire, on peut choisir certaines métadonnées qu'on juge importantes pour déterminer les dépendances.

     	       	   | n° client | nom client | ...
	------------------------------------------------
	n° client  |	       |            |
	----------------------------------------------
	nom client |           |            |
	----------------------------------------------
	   ...     |           |            |

Pour remplir cette table, on se pose la question suivante pour **chaque colonne** :

*Pour chaque valeur de cette donnée, existe-il une seule valeur de la donnée située en ligne?*

Si la réponse est "Oui", on rempli la case par '1' ou '*'.

Ensuite on simplifie le tableau en supprimant les colonnes vides.

### Clés primaires

Si pour un ensemble d'attributs {id, nom, prenom, naissance, sex, adresse, ..} on s'appercoit que l'un entre eux est la source d'une dépendance fonctionnelle pour tous les autre, celui là est appelé un **identifiant**.

Un identifiant est appelé **clé primaire** dans le modèle relationnel.

On prend l'exemple d'informations personnelles d'un client :
{id, nom, prenom, naissance, sex, adresse, ...}
Dans ce cas, l'attribut "id" sera la **clé primaire** et il est dit **naturel** 


## Les Relations

### Le domaine

### Le produit cartésien

### La relation


## Les formes normales

### La première forme normale

### La deuxième forme normale

### La troisième forme normale


##  Elaboration du modèle relationnel

### De l'Entité à la Relation

### Des associations aux clés etrangères

### Synthèse: Du modèle conceptuel au modèle relationnel

