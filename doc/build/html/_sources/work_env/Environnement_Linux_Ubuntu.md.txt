# Environnement Linux Ubuntu

Veille Environnement Linux/Ubuntu

## Présentation de Linux et de Ubuntu

Linux est un système d’exploitation basé sur un noyau qui permet d’utiliser un environnement gratuit et libre de droit qui a crée par Linus Tovarlds en 1991.

Ubuntu est est une distribution qui est basé sur le noyau de Linux open-source qui permet de naviguer sur Internet, utiliser des applications et gérer une bibliothèque multimédia.

C’est un noyau utilisé par beaucoup de systèmes d’exploitation très connus : entre autre, Android et MacOSx, l’un a été crée par Google et l’autre par Apple et se base sur ce noyau commun.

Ubuntu est la distribution Linux la plus connue car c’est l’un des système qui possède le plus d’améliorations, de fonctionnalités, de stabilité basé sur l’entraide de la communauté.

Il est l’un des systèmes d’exploitations les plus utilisés au monde avec des millions d’utilisateurs, que ce soit sur utilisation classique en bureautique qu’avec des serveurs informatiques et sur le cloud.

## Installation d’Ubuntu sur un PC

*Il y a plusieurs façons d’installer Linux sur un ordinateur.*


Tout d’abord : Deux médias peuvent être utilisés, sois un lecteur CD ou une clé USB.
Il faut télécharger le fichier ISO (l’image disque) su son PC et l’importer sur un média à l’aide d’un logiciel qui permettra de rendre son CD ou sa clé bootable. 

Avec le BIOS en lançant le logiciel d’installation par cela. L’installation s’effectue en quelques minutes selon la vitesse en écriture et en lecture de son espace de stockage (SSD ou disque dur classique ) et nous atterrissons sur l’environnement Ubuntu.


Ensuite : nous pouvons lancer une machine virtuel depuis un OS qui peut le permettre (par exemple Windows) pour lancer Ubuntu.
La virtualisation permet de lancer un ou plusieurs système d’exploitation en utilisant les ressources matérielles d’un ordinateur pour simuler un « faux ordinateur » .

Pour cette option, il est recommandé d’avoir une bonne configuration pour faire tourner la machine dans de bonnes conditions.

Pour l’utiliser, il faudra également télécharger l’ISO pour exploiter et Ubuntu et installer Virutal Box, le logiciel qui permettra de lancer la machine virtuelle.
Lors de l’exécution de l’application, une partie de la mémoire vive de l’ordinateur est utilisée.pour assurer son bon fonctionnement. Cela peut être modifier.
Plus il y a de RAM, plus le virtualisation sera fluide et sans latence.


## Présentation du terminal Ubuntu

Le terminal Linux est un programme qui émule une console à partir d’une interface graphique.
Savoir utiliser le terminal est très pratique car utiliser des raccourcis au clavier peut être beaucoup plus rapide que des faire des clics en naviguant avec des onglets.
Pour ouvrir le terminal, il faut utiliser la commande « Ctrl» « Alt » « T ».
Plusieurs éléments visuels peuvent apparaître. 
Le nom du user est « utilisateur » et le nom du pc est « utilisateur-ThinkPad-T430 ».
    • ~ : c'est le dossier dans lequel on se trouve actuellement. Vous pouvez naviguer de dossier en dossier dans la console et il est très utile qu'on vous rappelle systématiquement où vous vous trouvez avant chaque commande. Pour information, le symbole ~ signifie que vous êtes dans votre dossier personnel, ce qu'on appelle le « home » sous Linux ; c'est l'équivalent du dossier « Mes documents » de Windows.
      
    • $ : ce dernier symbole est très important ; il indique votre niveau d'autorisation sur la machine. Il peut prendre deux formes différentes :
    • $ : signifie que vous êtes en train d'utiliser un compte utilisateur « normal », avec des droits limités (il ne peut pas modifier les fichiers système les plus importants). Mon compte « utilisateur » est donc un compte normal avec des droits limités ;
# : signifie que vous êtes en mode super-utilisateur, c'est-à-dire que vous êtes connectés sous le pseudonyme « root ». 

## Le système de fichiers

Le système de fichiers est similaire à celui de Windows. 
La racine
Dans un système de fichiers, il y a toujours ce qu'on appelle une racine, c'est-à-dire un « gros dossier de base qui contient tous les autres dossiers et fichiers ».
Sous Windows, il y a en fait plusieurs racines.C:\est la racine de votre disque dur,D:\est la racine de votre lecteur CD (par exemple).
Sous Linux, il n'y a qu'une et une seule racine : « / ». Comme vous le voyez, il n'y a pas de lettre de lecteur car justement, Linux ne donne pas de nom aux lecteurs comme le fait Windows. Il dit juste « La base, c'est/ ».

Architecture des dossiers
    • Sous Windows, un dossier peut être représenté de la manière suivante :C:\Program Files\Winzip. On dit queWinzipest un sous-dossier du dossierProgram Files, lui-même situé à la racine.
Vous noterez que c'est l'antislash\(aussi appelé backslash) qui sert de séparateur aux noms de dossiers.
    • Sous Linux, c'est au contraire le/qui sert de séparateur.
Comme je vous l'ai dit, il n'y a pas deC:sous Linux, la racine (le début) s'appelant juste/.
      Le dossier de notre super-programme ressemblerait plutôt à quelque chose comme cela :/usr/bin/. On dit quebinest un sous-dossier du dossierusr, lui-même situé à la racine.




## Informations par rapport aux commandes effectués :

    • bin : contient des programmes (exécutables) susceptibles d'être utilisés par tous les utilisateurs de la machine. 
      
    • boot : fichiers permettant le démarrage de Linux.

    • dev : fichiers contenant les périphériques. En fait – on en reparlera plus tard – ce dossier contient des sous-dossiers qui « représentent » chacun un périphérique. On y retrouve ainsi par exemple le fichier qui représente le lecteur CD.
    • etc : fichiers de configuration.
      
    • home : répertoires personnels des utilisateurs. On en a déjà parlé un peu avant : c'est dans ce dossier que vous placerez vos fichiers personnels, à la manière du dossierMes documentsde Windows. Chaque utilisateur de l'ordinateur possède son dossier personnel.

    •  lib : dossier contenant les bibliothèques partagées (généralement des fichiers.so) utilisées par les programmes. C'est en fait là qu'on trouve l'équivalent des.dllde Windows.
    • media : lorsqu'un périphérique amovible (comme une carte mémoire SD ou une clé USB) est inséré dans votre ordinateur, Linux vous permet d'y accéder à partir d'un sous-dossier demedia. On parle de montage.

    • mnt : c'est un peu pareil quemedia, mais pour un usage plus temporaire.
    • opt : répertoire utilisé pour les add-ons de programmes.
    • proc : contient des informations système.
    • root : c'est le dossier personnel de l'utilisateur « root ». Normalement, les dossiers personnels sont placés danshome, mais celui de « root » fait exception. En effet, comme je vous l'ai dit dans le chapitre précédent, « root » est le superutilisateur, le « chef » de la machine en quelque sorte. Il a droit à un espace spécial.
    • sbin : contient des programmes système importants.
    • tmp : dossier temporaire utilisé par les programmes pour stocker des fichiers.
    • usr : c'est un des plus gros dossiers, dans lequel vont s'installer la plupart des programmes demandés par l'utilisateur.
      . var : ce dossier contient des données « variables », souvent des logs (traces écrites de ce qui s'est passé récemment sur l'ordinateur).







