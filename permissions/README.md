tasks 0: la commande "su" permet de changer d'utilisateur.
tasks 1: La commande pour afficher le nom d'utilisateur effectif de l'utilisateur actuel est "whoami".
tasks 2: La commande "groups" permet d'afficher tous les groupes auxquels l'utilisateur actuel appartient.
tasks 3: Pour changer le propriétaire d'un fichier sur "sudo chown betty hello" sudo permet de passer en mode administrateur et chown permet de changer le propriétair.
tasks 4: La commande pour créer un fichier vide appelé "hello" en utilisant un script est "touch hello". "touch" permetant de crée un fichier
tasks 5: La commande pour donner les droit au fichier hello est "chmod u+x hello""chmod" c'est le nom de la commande utilisée pour changer les permissions."u" ndique que l'opération doit être effectuée sur l'utilisateur (propriétaire) du fichier. "+x" indique l'ajout de la permission d'exécution.
tasks 6: La commande pour donner les droit au fichier hello est "chmod u+x,o+r hello" "chmod" c'est le nom de la commande utilisée pour changer les permissions."u" pour l'utilisateur (propriétaire) du fichier."g" pour le groupe propriétaire du fichier."o" pour les autres utilisateurs (non propriétaires)."+x" pour ajouter la permission d'exécution."+r" pour ajouter la permission de lecture."+w" pour ajouter la permission d'écriture.
"-x" pour supprimer la permission d'exécution."-r" pour supprimer la permission de lecture."-w" pour supprimer la permission d'écriture.
tasks 7:La commande "chmod ugo+x hello" ajoute les permissions d'exécution au propriétaire (u), au groupe propriétaire (g) et aux autres utilisateurs (o) pour le fichier hello "+x" indique l'ajout de la permission d'exécution.
tasks 8: les chiffres pour représenter les différentes combinaisons de permissions (lecture = 4, écriture = 2, exécution = 1)
La commande qui permet de définir les permissions Propriétaire : aucune permission du tout Groupe : aucune permission du tout Autres utilisateurs : toutes les permissions est "chmod 007 hello"
tasks 9: Dans "-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello",Le propriétaire a les permissions de lecture, écriture et exécution (rwx)
Le groupe a les permissions de lecture et d'exécution (r-x)
Les autres utilisateurs ont les permissions d'écriture et d'exécution (wx)
les chiffres pour représenter les différentes combinaisons de permissions (lecture = 4, écriture = 2, exécution = 1). donc la commande est "chmod 753 hello"
tasks 10:  La commande "chmod --reference=olleh hello" "chmod" est une commande utilisée pour modifier les permissions des fichiers. "--reference=olleh" spécifie que les permissions du fichier "olleh" doivent être utilisées comme référence. "hello" est le fichier auquel les mêmes permissions seront appliquées.
tasks 11: la commande est "chmod -R a+X *" "-R" pour récursive "X" pour les permissions d'exécution sur les dossier "*" pous ciblé tous les sous-répertoires et fichiers "a" pour tous les utilisateurs (all) on aurrait aussi pu utiliser ugo pour user + group + ownership.
tasks 12: Pour crée un dossier avec les permission 751 il faut realisé la commande "mkdir -m 751 my_dir" l'option -m permet de spécifier les permissions du nouveau répertoire.
tasks 13: "chown :school hello" "chown" est la commande utilisée pour modifier le propriétaire et le groupe d'un fichier ou d'un répertoire. ":school" est l'argument de la commande qui spécifie le nouveau groupe pour le fichier "hello"."hello" est le nom du fichier pour lequel on souhaitez modifier le propriétaire.
tasks 14:
tasks 15:
tasks 16: