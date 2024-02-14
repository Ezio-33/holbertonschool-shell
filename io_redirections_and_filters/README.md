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

### Tâche 8

### Tâche 9

### Tâche 10

### Tâche 11

### Tâche 12

### Tâche 13

### Tâche 14

### Tâche 15

### Tâche 16
