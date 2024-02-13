# Guide des commandes pour la gestion des permissions et des utilisateurs

## Tâches

### Tâche 0
La commande "su" permet de changer d'utilisateur.

### Tâche 1
La commande pour afficher le nom d'utilisateur effectif de l'utilisateur actuel est "whoami".

### Tâche 2
La commande "groups" permet d'afficher tous les groupes auxquels l'utilisateur actuel appartient.

### Tâche 3
Pour changer le propriétaire d'un fichier sur "sudo chown betty hello", sudo permet de passer en mode administrateur et chown permet de changer le propriétaire.

### Tâche 4
La commande pour créer un fichier vide appelé "hello" en utilisant un script est "touch hello". "touch" permet de créer un fichier.

### Tâche 5
La commande pour donner les droits au fichier hello est "chmod u+x hello". "chmod" est le nom de la commande utilisée pour changer les permissions. "u" indique que l'opération doit être effectuée sur l'utilisateur (propriétaire) du fichier. "+x" indique l'ajout de la permission d'exécution.

### Tâche 6
La commande pour donner les droits au fichier hello est "chmod u+x,o+r hello". "chmod" est le nom de la commande utilisée pour changer les permissions. "u" pour l'utilisateur (propriétaire) du fichier. "o" pour les autres utilisateurs (non propriétaires). "+x" pour ajouter la permission d'exécution. "+r" pour ajouter la permission de lecture.

### Tâche 7
La commande "chmod ugo+x hello" ajoute les permissions d'exécution au propriétaire (u), au groupe propriétaire (g) et aux autres utilisateurs (o) pour le fichier hello "+x" indique l'ajout de la permission d'exécution.

### Tâche 8
Les chiffres pour représenter les différentes combinaisons de permissions sont : lecture = 4, écriture = 2, exécution = 1. La commande qui permet de définir les permissions Propriétaire : aucune permission du tout, Groupe : aucune permission du tout, Autres utilisateurs : toutes les permissions est "chmod 007 hello".

### Tâche 9
Dans "-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello", Le propriétaire a les permissions de lecture, écriture et exécution (rwx). Le groupe a les permissions de lecture et d'exécution (r-x). Les autres utilisateurs ont les permissions d'écriture et d'exécution (wx). Les chiffres pour représenter les différentes combinaisons de permissions sont lecture = 4, écriture = 2, exécution = 1. Donc la commande est "chmod 753 hello".

### Tâche 10
La commande "chmod --reference=olleh hello" "chmod" est une commande utilisée pour modifier les permissions des fichiers. "--reference=olleh" spécifie que les permissions du fichier "olleh" doivent être utilisées comme référence. "hello" est le fichier auquel les mêmes permissions seront appliquées.

### Tâche 11
La commande est "chmod -R a+X *". "-R" pour récursive, "X" pour les permissions d'exécution sur les dossiers "*", pour cibler tous les sous-répertoires et fichiers, "a" pour tous les utilisateurs (all). On aurait aussi pu utiliser ugo pour user + group + ownership.

### Tâche 12
Pour créer un dossier avec les permissions 751, il faut réaliser la commande "mkdir -m 751 my_dir". L'option -m permet de spécifier les permissions du nouveau répertoire.

### Tâche 13
"chown :school hello". "chown" est la commande utilisée pour modifier le propriétaire et le groupe d'un fichier ou d'un répertoire. ":school" est l'argument de la commande qui spécifie le nouveau groupe pour le fichier "hello". "hello" est le nom du fichier pour lequel on souhaite modifier le propriétaire.

### Tâche 14
"chown -R vincent:staff *". "chown" est utilisé pour changer le propriétaire et le groupe propriétaire. "-R" pour effectuer la modification de manière récursive. "vincent:staff" spécifie le nouveau propriétaire et groupe propriétaire pour les fichiers et répertoires. "*" spécifie tous les fichiers et répertoires du répertoire de travail.

### Tâche 15
Pour changer le propriétaire et le groupe propriétaire d'un lien symbolique la commande est "chown -h vincent:staff _hello" option -h est ajoutée à la commande chown, spécifiant que la modification doit être appliquée au lien symbolique lui-même plutôt qu'à la cible du lien.


### Tâche 16
À compléter.
