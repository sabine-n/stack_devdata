# Modèle Logique des Données Relationnelles

On a vu précedemment comment le MCD nou permet de définir le concept sur lequelle sera construite notre future base de donnée. C'est à partir du modèle conceptuel des données qu'on va pouvoir passer au modèle logique des données. Ce dernier va nous permettre de modéliser la structure selon laquelle les données seront stockées dans la future base de donnée. Donc on passe du concept à l'adaptation technique. En particulier, il s'agit de l'organisation des données en utilisant de tableaux à deux dimensions et de formaliser la manipulation des données réparties sur plusieurs tables.

   3.1. Les dépendances fonctionnelles

Les dépendances fonctionnelles servent à définir les liens entre les métadonnées définis précédemment. Ces métadonnées seront nommées attributs.

   3.1.1. Dépendances entre attributs

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

   3.1.2. Clés primaires

Si pour un ensemble d'attributs {id, nom, prenom, naissance, sex, adresse, ..} on s'appercoit que l'un entre eux est la source d'une dépendance fonctionnelle pour tous les autre, celui là est appelé un **identifiant**.

Un identifiant est appelé **clé primaire** dans le modèle relationnel.

On prend l'exemple d'informations personnelles d'un client :
{id, nom, prenom, naissance, sex, adresse, ...}
Dans ce cas, l'attribut "id" sera la **clé primaire** et il est dit **naturel** 


    3.2. Les Relations

   3.2.1. Le domaine

   3.2.2. Le produit cartésien

   3.2.3. La relation

    3.3. Les formes normales

   3.3.1. La première forme normale

   3.3.2. La deuxième forme normale

   3.3.3. La troisième forme normale

    3.4. Elaboration du modèle relationnel

   3.4.1. De l'Entité à la Relation

   3.4.2. Des associations aux clés etrangères

   3.4.3. Synthèse: Du modèle conceptuel au modèle relationnel

