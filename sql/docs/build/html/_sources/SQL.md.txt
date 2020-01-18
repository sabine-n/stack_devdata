SQL
===

Intro
-----
SQL veut dire Langage de requête structurée : Structured Query Language

C’est un langage informatique utilisé pour exploiter des bases de données. Il permet de façon générale la définition, la manipulation et le contrôle de sécurité de données.

Créé en 1974, normalisé depuis 1986, le langage est reconnu par la grande majorité des systèmes de gestion de bases de données relationnelles


A quoi ça sert
--------------
Pour que les différents logiciels et le moteur de base de données puissent se comprendre, ils utilisent un langage appelé SQL.

il est utilisé pour :
* Lire les données
* Écrire les données
* Modifier les données
* Supprimer les données
* Modifier la structure d’une base de donnée

De plus, il a plusieurs avantages consequents :

* Il peut fonctionner avec n’importe quelle base de données. Il suffira de lui indiquer avec quelle base de données il doit dialoguer.
* C’est un langage international
* Si on doit changer la base, il suffit de modifier la relation entre le logiciel et la base de données.


Commandes de base
-----------------

Select :
La commande **SELECT** permet de récupérer des données stockées dans une ou plusieurs table(s).
ex :
**SELECT** *
**FROM** personne
**WHERE** (taille > 170) ;

Insert :
La commande **INSERT** permet d'ajouter des données dans une table existante.
ex :
**INSERT INTO** personne **VALUES** (50, "Dupont", "Pierre", 25, "Sans emploi", 0, 174)

Update :
La commande **UPDATE** permet de modifier les données contenues dans la table
ex :
**UPDATE** table
**SET** colonne_1 = 'valeur 1', colonne_2 = 'valeur 2', colonne_3 = 'valeur 3'
WHERE condition ;

Delete :
La commande **DELETE** permet de supprimer une partie ou la totalité des données de la table
ex :
**DELETE FROM** nom_table ;

Commit :
**COMMIT** valide la transaction en cours. Tout le monde peut désormais voir les modifications réalisées au cours de la transaction.
ex :


Create Table :
La commande **CREATE TABLE** permet de créer une table nommée nom_sql comportant un ou plusieurs champ.
ex :
create table **PERSONNE**
(
    **ID_PERSONNE** int not null ,
    **NOM** varchar not null ,
    **PRENOM** varchar not null ,
    **AGE** int ,
    **CATEGORIE_PROFESSIONNELLE** varchar ,
    **NOMBRE_ENFANTS** int ,
    **TAILLE** float ,

    primary key (ID_PERSONNE) ,
) ;

Alter Table :
La commande **ALTER TABLE** permet de modifier la table existante désignée par l'argument nom_sql.
ex :
**ALTER TABLE** nom_table
instruction

Drop Table :
La commande **DROP TABLE** permet de supprimer la table nommée nom_sql de la base.
ex :
**DROP TABLE** nom_table

Grant :
La commande **GRANT** permet de définir les droits d’accès associés au schéma nom_sql
ex :
**GRANT ALL PRIVILEGES ON** genres TO manuel;

Revoke :
La commande **REVOKE** permet de supprimer les droits d’accès spécifiques associés au schéma défini par le paramètre nom_sql.
ex :
**REVOKE ALL PRIVILEGES ON** genres **FROM** manuel;


