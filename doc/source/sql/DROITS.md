Gestion des droits
=========

Intro
-----
***En SQL la gestion des droits des utilisateurs est très importante elle permet de définir  les actions  que un  utilisateur peut effectuer***

**Les différentes actions s'appelle des***DCL (Data Control Language)* **elle permentent de controller la base de données, on peut aussi bien les exécuter via le terminal que via une interface graphique**

Les commandes priviliges 
----------

```GRANT```: autorisation d'un utilisateur à effectuer une action ;

```DENY``` : interdiction à un utilisateur d'effectuer une action ;

```REVOKE``` : annulation d'une commande de contrôle de données précédente ;

```COMMIT``` : validation d'une transaction en cours ;

```ROLLBACK``` : annulation d'une transaction en cours ;

```LOCK``` : verrouillage sur une structure de données.

Privilèges du CRUD :
Les privilèges ```SELECT```, ```INSERT```, ```UPDATE```  et ```DELETE```  permettent aux utilisateurs d'utiliser ces mêmes commandes.

```CREATE TABLE``` : Création de tables

```CREATE TEMPORARY TABLE``` :Création de tables temporaires

```CREATE VIEW``` : Création de vues (il faut également avoir le privilège SELECTsur les colonnes sélectionnées par la vue)

```ALTER``` : Modification de tables (avec ALTER TABLE)

```DROP``` : Suppression de tables, vues et bases de données

```CREATE ROUTINE``` : Création de procédures stockées (et de fonctions stockées - non couvertes dans ce cours)

```ALTER ROUTINE``` : Modification et suppression de procédures stockées (et de fonctions stockées)

```EXECUTE``` : Exécution de procédures stockées (et de fonctions stockées)

```INDEX``` : Création et suppression d'index

```TRIGGER``` : Création et suppression de triggers

```LOCK TABLES``` : Verrouillage de tables (sur lesquelles on a le privilège SELECT)

```CREATE USER``` : Gestion d'utilisateur (commandes CREATE USER, DROP USER, RENAME USER  et SET PASSWORD)

Exemple de requête
-------

***Autorisation d'un utilisateur à effectuer une action :***
```
GRANT UPDATE (nom, prenom) ON eleves
TO enseignant
WITH GRANT OPTION;
```

***Interdiction d'un utilisateur à effectuer une action :***
```
DENY DELETE
TO enseignant
```

***Annulation d'une commande de contrôle de données précédente :***
```
REVOKE UPDATE (nom, prenom)
ON eleves
FROM enseignant
```

***Verrouillage d'une structure de données :***
```LOCK TABLE eleves IN EXCLUSIVE MODE;```

