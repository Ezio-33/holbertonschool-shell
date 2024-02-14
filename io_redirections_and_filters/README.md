# Guide des commandes Shell, redirections E/S et filtres

## Tâches

### Tâche 0
La commande "echo "Hello, World" permet ecrire "Hello, World", suivi d'une nouvelle ligne sur la sortie standard.
### Tâche 1
La commande qui affiche un smiley confus "(Ôo)' est "echo "(Ôo)'".
### Tâche 2
La commande qui permet d'affiche le contenue du fichier /etc/passwd est "cat /etc/passwd"
### Tâche 3
La commande qui permet d'affiche le contenue des fichiers est "cat /etc/passwd /etc/hosts" je met un espace entre les deux pour cible les deux fichiers.
### Tâche 4
#!/bin/bash
la commande pour afficher les 10 premiere ligne du fichier /etc/passwd est "tail -10 /etc/passwd" on peu modifier le parametre -10 par le nombre de ligne que l'on souhaite afficher.
### Tâche 5
j'ai utiliser la commande "head -n 10 /etc/passwd" Explication: head permetd'afficher par defaut les 10 premiere ligne d'un fichier. On peu aussi utiliser la parametre "n- nombre_de_ligne" pour avoir le nombre de ligne voulus comme dans ma commande.

### Tâche 6
j'ai utiliser la commande "head -n 3 iacta | tail -n 1" Explication:  head -n 3 iacta": est utilisée pour afficher les premières lignes d'un fichier. Ici, -n 3 spécifie que nous voulons afficher les 3 premières lignes du fichier "iacta".
"|" (pipe) prend la sortie de la commande précédente (dans ce cas, la sortie des 3 premières lignes de "iacta") et la transmet comme entrée à la commande suivante.
"tail -n 1" est utilisée pour afficher les dernières lignes d'un fichier. 
### Tâche 7
commande "echo "Best School" > '\*\\'\''"Best School"\'\''\\*$\?\*\*\*\*\*:)'" "echo" permet d'ercire un texte choisi ">" permet d'ecrire et ecraser le contenue du fichier qui suivra la commande. si le fichier n'existe pas il le crée.
### Tâche 8
commande: "ls -la > ls_cwd_content" "ls" liste le contenu du répertoire courant "l" Affiche les détails de chaque fichier ou répertoire. "a" Inclut les fichiers cachés ">" permet d'ecrire et ecraser le contenue du fichier qui suivra la commande. si le fichier n'existe pas il le crée.
### Tâche 9
commande: "tail -1 iacta >> iacta" Explication: "tail" affiche les derniere ligne "-1" defini le nombrede ligne ">>" ajoute les ligne a la suite dans le fichier choisi.
### Tâche 10
commande: "find -type f -name "*.js" -delete" Explication: "find" recherche les fichier "-type f" définit le type de fichier a rechercher "-name" le nom du fichier "*.js" pour definir tout se qui fini par .js
### Tâche 11

### Tâche 12

### Tâche 13

### Tâche 14

### Tâche 15

### Tâche 16
