LES FONCTIONS
=============


1 QU'EST CE QU'UNE FONCTION
---------------------------

**Définition :**
En programmation, les fonctions sont très utiles pour réaliser plusieurs fois la même opération au sein d’un programme. Lorsqu’une tâche doit être réalisée plusieurs fois, on peut l’isoler dans un programme au sein d’une fonction.
Elles rendent également le code plus lisible et plus clair en le fractionnant en blocs logiques.
Pour déﬁnir une fonction, Python utilise le mot-clé def et si on veut que celle-ci renvoie quelque chose, il faut utiliser le mot-clé return. 


	*Par exemple :*
	>>> def carre(x):
	…   	return x**2 
	…
	>>> print(carre(2)) 
	4

**Syntaxe :**
Ainsi, une fonction est une suite d'instructions que l'on peut appeler avec un nom.

def nom_fct(paramètre(s))
	bloc d'instruction

Une fonction comporte quatre parties :
- le terme "def" qui définit la fonction,
- le nom de la fonction,
- les paramètres si besoin est,
- le bloc d'instruction.

Après le terme "def", il s'agit de donner un nom à notre fonction qui la qualifie et l'identifie mais attention certains noms, déjà utilisés par Python dans des situations très précises sont interdits. Il n'est pas possible d'écrire : def def() ou def break(). Cela occasionnerait une erreur de syntaxe.

**Voici la liste des mots interdits :**

and	as	assert	break	class	continue	def	del
elif	else	except	exec 	finally	for	from	global
if	import	in	is	lambda	not	or	pass
print	raise	return	try	while	with	yield





