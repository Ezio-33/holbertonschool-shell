# Guide des commandes Shell, redirections E/S et filtres

## Tâches

### Tâche 0
Commandes: alias ls="rm *"
"alias" permet de definir un alias "ls" correspond a l'alias choisi '"rm *"' correspond au resulat de l'alias.

### Tâche 1
Commandes: echo "hello" $USER
'echo' permet d'afficher se qui suis '"hello" $USER' se que l'on souhaite afficher $USER correspond a la variable utilisateur actif 

### Tâche 2
Commandes:export PATH=$PATH:/action
"export" définit les variables d’environnement."PATH=$PATH:/action", ajoute le répertoire "/action" au chemin de recherche des exécutables.
### Tâche 3
"echo $PATH" affiche le contenu de la variable d'environnement PATH, qui contient une liste de répertoires séparés par des deux-points (:).
"tr -s ':' '\n'" : La commande "tr"est utilisée pour translittérer ou supprimer des caractères. Ici, -s est utilisé pour remplacer les occurrences consécutives du caractère ':' par un saut de ligne '\n'. Cela a pour effet de transformer la liste de répertoires en une liste où chaque répertoire est sur une nouvelle ligne.
"wc -l" est utilisée pour compter les lignes, les mots et les caractères. L'option -l indique à wc de compter les lignes.
### Tâche 4
#!/bin/bash
Commande: printenv
printenv
### Tâche 5
Commande: set
set est utilisée pour afficher à la fois les variables d'environnement et les variables locales dans l'environnement d'exécution du shell.
### Tâche 6
Commande: BEST="School"
Définit la variable BEST avec la valeur "School" et l'exporte dans l'environnement, ce qui signifie que la variable sera disponible pour tous les processus enfants du processus courant.
### Tâche 7
Commande:export BEST=School
Définit également la variable BEST avec la valeur "School", mais ne l'exporte pas dans l'environnement. Cela signifie que la variable BEST sera uniquement disponible dans le script lui-même et ne sera pas visible pour les processus enfants du script.
### Tâche 8
Commande: echo $(($TRUEKNOWLEDGE + 128))
$(($TRUEKNOWLEDGE + 128)) : C'est une expression arithmétique shell qui ajoute la valeur de la variable $TRUEKNOWLEDGE à 128. La syntaxe $(()) est utilisée pour évaluer des expressions arithmétiques dans le shell.
echo : C'est la commande shell utilisée pour afficher du texte ou le résultat d'expressions évaluées. Dans ce cas, elle affichera le résultat de l'expression arithmétique.
### Tâche 9
Commande: echo $(($POWER / $DIVIDE))
### Tâche 10
Commande:echo $(($BREATH ** $LOVE))
### Tâche 11
Commande:echo "$((2#$BINARY))"
La commande permet de convertire en nombre en base 2 en decimal
	binaire=$([##2]décimal))
	hex=$(([##16]décimal))
	hex=$([##16]2#$binaire))
	décimal=$((2#$binaire))
### Tâche 12
Commande:echo {a..z}{a..z} | tr -d 'o' | tr -s ' ' '\n'
{a..z} : Cela génère une séquence de lettres minuscules de "a" à "z". Cette séquence est utilisée deux fois pour générer toutes les combinaisons possibles de deux lettres.
tr -d 'o' : Cela supprime toutes les occurrences de la lettre "o" de la sortie générée précédemment. Cela garantit que les combinaisons contenant la lettre "o" ne seront pas incluses dans la sortie.
tr -s ' ' '\n' : Cela transforme les espaces en sauts de ligne, ce qui signifie que chaque combinaison sera imprimée sur une nouvelle ligne.
### Tâche 13
Commande:printf "%0.2f\n" "$NUM"
### Tâche 14
Commande:echo "$((2#$BINARY))"