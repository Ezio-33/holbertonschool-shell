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

### Tâche 6

### Tâche 7

### Tâche 8

### Tâche 9

### Tâche 10

### Tâche 11

### Tâche 12

### Tâche 13

### Tâche 14