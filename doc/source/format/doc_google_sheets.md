Google Sheets 
=============

Histoire et création de Google Sheets:
--------------------------------------

Le 11 octobre 2006, Google ouvre le site Google Docs & Spreadsheets qui regroupe les accès à l'ancien Writely et Google Spreadsheets2.
Quatre mois plus tard, le site est traduit en plusieurs langues, dont le français sous le nom Google Document et Tableur dans un premier temps, puis Google Documents ensuite (Google Docs en anglais).

Spreadsheets : Ce tableur en ligne développé par Google permet à des utilisateurs de créer, modifier et manipuler des feuilles de calcul grâce à une interface WYSIWYG, comme un tableur logiciel classique mais dans un simple navigateur web. Google a sorti le 6 juin 2006 Google Spreadsheets, disponible auparavant seulement en test et à un nombre limité d'utilisateurs inscrits. Une nouvelle fonctionnalité est aussi disponible, on peut créer des formulaires et voir les résultats sur les feuilles de calcul.
Présentations : Ce module permet de créer des diaporamas et de les exporter vers le format *.ppt ou *.pdf. Il est aussi possible d'importer des présentations au format .ppt et de les modifier en ligne.

*WYSIWYG: « WYSIWYG » est l’acronyme de la locution anglaise « what you see is what you get », signifiant littéralement en français « ce que vous voyez est ce que vous obtenez »1.
Les termes WYSIWYG ou tel écran, tel écrit2 désignent en informatique une interface utilisateur qui permet de composer visuellement le résultat voulu, typiquement pour un logiciel de mise en page, un traitement de texte ou d’image. C'est une interface « intuitive » : l’utilisateur voit directement à l’écran à quoi ressemblera le résultat final.

six astuces pour utiliser Google Sheets comme un pro:

Importer des données d'une autre feuille de calcul
-----------------------------------------------------
Il arrive fréquemment de travailler en même temps sur plusieurs feuilles de calcul, dont certaines peuvent avoir des données communes.
Il peut donc être très pratique d’importer automatiquement des valeurs issues d’un autre document (qui seront actualisées en temps réel en cas de modifications).
Ceci est rendu possible par la fonction =IMPORTRANGE, qui s’utilise de la manière suivante :
=Importrange(« URL du document Sheets »; « Nom de la feuille!Plage de valeurs »)


   Notez qu’il est facultatif de renseigner le nom de la feuille si le document n’en contient qu’une.

Protéger des cellules
------------------------
L’un des avantages de Google Sheets, c’est qu’il permet de partager très facilement des feuilles de calcul avec d’autres utilisateurs.
Toutefois, il y a peut-être certaines données importantes que vous ne souhaitez pas voir modifiées (ne serait-ce que par erreur) par quelqu’un d’autre : pensez alors à les verrouiller.
Pour ce faire, sélectionnez une plage de cellules, puis allez dans Données > Feuilles et plages protégées :

Dans le panneau qui apparaît à droite, cliquez sur « Définir les autorisations ». Vous pourrez alors choisir comment protéger les données concernées :

Modifier rapidement du texte
-------------------------------

Il n’est pas rare que les chaînes de caractères présentes dans une feuille Google Sheets soient désordonnées.
Trois fonctions peuvent vous aider à y remédier :

=UPPER : permet de mettre automatiquement en majuscules les lettres contenues dans une cellule ;
=LOWER : permet de mettre automatiquement en minuscules les lettres contenues dans une cellule ;
=TRIM : permet de supprimer les espaces au début ou à la fin d’une chaîne de caractères.
Par exemple, si je veux mettre rapidement en majuscules tous les mots présents dans une colonne :


Trier les données
-----------------
Mettre de l’ordre dans les données, c’est aussi effectuer des tris pour ne visualiser que les cellules qui nous intéressent (surtout quand on a une grande quantité).
Pour cela, vous pouvez utiliser la fonction de filtrage : par exemple, sélectionnez les en-têtes d’un tableau et cliquez sur le bouton en forme d’entonnoir.
Un symbole apparaît à côté des en-têtes : en cliquant dessus, vous pouvez trier les données de la colonne par ordre croissant ou décroissant, ou encore ne visualiser que les données correspondant à tel ou tel critère.


Tirer parti de l’intelligence artificielle
------------------------------------------
Google est connu pour ses prouesses en matière d’IA, et Sheets ne fait pas exception.
La fonction Explorer (en bas à droite de l’écran) permet justement d’utiliser l’intelligence artificielle à votre avantage, puisqu’elle vous permet de générer automatiquement des tableaux et autres graphiques à partir de vos données.

.. image: https://www.codeur.com/blog/wp-content/uploads/2018/05/astuce-google-sheets-6.gif
   width: 500

Utiliser Google Traduction dans Google Sheets
---------------------------------------------

Il y a des mots dans une langue étrangère dans votre document Google Sheets et vous ne souhaitez pas faire des allers-retours incessants vers Google Traduction ?
Ne vous en faites : il est possible de traduire directement un mot dans le tableur à l’aide la fonction =GOOGLETRANSLATE. Elle s’utilise comme ceci :
=Googletranslate(« mot ou phrase à traduire »; « langue source »; « langue cible »)

Remarque : la langue source et la langue de destination doivent être indiquées par un code de deux lettres (par exemple « en » pour l’anglais ou « fr » pour le français).

Pour la langue source, vous pouvez aussi indiquer « auto » pour que Google Traduction détermine automatiquement la langue.

