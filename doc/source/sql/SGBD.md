Système de Gestion de Base de Données   
====

Intro
-----

**L'acronyme SGBD, pour Système de Gestion de Base de Données, désigne un logiciel informatique permettant le stockage, la consultation, la mise à jour, la structuration ou encore le partage d'informations dans une base de données. Il garantit en outre la         confidentialité et la pérennité de ces données. En effet, il n'y a d'intermédiaire ni entre  l'informaticien et les données, ni entre l'utilisateur et les données.**

Dans la pratique, un SGBD peut être utilisé pour rechercher ou trier des informations. Dans sa version la plus simple, il se compose d'une interface graphique. Les SGBD les plus complexes, eux, intègrent différents langages de programmation pour proposer des fonctionnalités toujours plus performantes.

On retrouve les systèmes de gestion de base de données dans de nombreuses applications informatiques comme dans les logiciels de réservation, les guichets automatiques des banques, les logiciels d'inventaire, etc.

Exemple de SGBD
------------------------

Oracle est un SGBD relationnel (et relationnel-objet dans ses dernières versions) très reconnu pour les applications professionnelles.

PostgreSQL est un SGBD relationnel et relationnel-objet très puissant qui offre une alternative open source aux solutions commerciales comme Oracle ou IBM.

**MySQL est un SGBD relationnel libre (licence GPL et commerciale), simple d'accès et très utilisé pour la réalisation de sites Web dynamiques. Depuis la version 4 MySQL implémente la plupart des fonctions attendues d'un SGBD relationnel.**

Access est un SGBD relationnel Microsoft, qui offre une interface graphique permettant de concevoir rapidement des applications de petite envergure ou de réaliser des prototypes.

Composition & Fonctionnement SGBD
----------------------------------------

Stockées sur un disque dur, plus vaste, mais plus lent, les données contenues dans chaque base peuvent atteindre plusieurs téraoctets. Les SGBD modernes sont équipés de programme pour accélérer le traitement des opérations commandées. 

**La majorité des SGBD se compose de quatre éléments qui garantissent leur bon fonctionnement :**

le moteur de base de données assure la gestion des fichiers de la BD, la transmission des données entrantes et sortantes vers des programmes tiers, ainsi que la protection et la maintenance des données. 

un programme gère le magasin où sont contenues les règles d'organisation des données et les contraintes, les contrôles d'accès, et la liste des individus admis à accéder aux données et à les modifier.  
un processeur de requête exécute les opération requises en langage de commande ou via une interface graphique. 

la très grande majorité des SGBD actuels utilise SQL comme langage de commande de base, mais d'autres peuvent venir le compléter, selon la complexité du système. 
  
  
Type de SGBD
--------------------------       

Il y a différentes façons de classer les SGBD, en voici une reposant sur des aspects pratiques, avec des avantages et des inconvénients : 

**Le SGBD relationnel, le plus fréquent actuellement, repose sur la théorie mathématique des ensembles. Ce système fiable et robuste est dominé depuis trente ans par de grands acteurs, comme Oracle, Microsoft et IBM. Il garantit de bonnes performances en ce qui concerne le stockage, les accès et la sécurité des données, mais avec l'avènement du Big Data, il s'avère rigide et limité, ce qui remet en cause sa prédominance.**

Le système NoSQL, plus flexible, il ne demande pas de définir  chaque donnée pour chaque entité, ce qui en fait une option intéressante pour gérer des bases de données importante, avec beaucoup de données éparses et dont la structure est susceptible d'évoluer au fil du temps. Il regroupe quatre catégories de fonctions principales : clé-valeurs, documents, colonnes et graphiques.  
                
Le Système de gestion de BD in-Memory, dont l'intérêt principale est de se passer de disque dur et de stocker les données dans sa mémoire. Il est beaucoup plus rapide pour traiter les opérations, mais sa capacité et ses fonctionnalités sont limitées. 

D'autres systèmes, comme le SGBD pour les données XML, peu avantageux par rapport aux autres, le système avec une base de données en colonnes, optimisé et rapide en lecture, mais pas en écriture, les SGBD orientés objets, populaires dans les années 1990, ou enfin, les systèmes hiérarchiques ou les systèmes de réseaux, antérieurs aux bases de données relationnelles. 
