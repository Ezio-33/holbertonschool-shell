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
La commande pour afficher les 10 premiere ligne du fichier /etc/passwd est "tail -10 /etc/passwd" on peu modifier le parametre -10 par le nombre de ligne que l'on souhaite afficher.
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
commande: "find -mindepth 1 -type d | wc -l" Explication: "-mindepth" 1 indique à find de commencer la recherche dns le repertoire actuel, mais exclut le répertoire racine lui-même. "-type d" spécifie que nous cherchons des dossiers. "|" pipe prend la sortie de la commande find (la liste des répertoires) et la transmet comme entrée à la commande suivante. "wc" est utilisée pour compter les lignes, les mots et les caractères dans une entrée donnée."-l" spécifie que nous voulons compter les lignes.
### Tâche 12
commande: "ls -1t | head -10" Explication: : La commande "ls" est utilisée pour lister les fichiers et les répertoires dans un répertoire donné. L'option "-t" trie les éléments par date de modification, en affichant d'abord les plus récents.  L'option "-1" (chiffre un) force la commande "ls" à afficher un fichier par ligne, "|" pipe prend la sortie de la commande précédente et la transmet comme entrée à la commande suivante. La commande "head" est utilisée pour afficher les premières lignes (ou les premiers éléments) d'une entrée donnée. L'option "-10" spécifie que nous voulons afficher seulement les 10 premiers éléments de l'entrée.
### Tâche 13
commande: "sort | uniq -u" Explication: "sort" est utilisée pour trier les lignes de texte dans un ordre spécifié. Par défaut, il trie dans l'ordre lexicographique.Le symbole pipe transmet le resultat comme entrée à la commande suivante."uniq" est utilisée pour filtrer ou rapporter les lignes en double à partir d'une entrée donnée. L'option "-u" ou "--unique" affiche uniquement les lignes qui ne sont pas en double.
### Tâche 14
commande: "grep root /etc/passwd" Explication: "grep" est utilisée pour rechercher des occurrences d'un motif dans un fichier.
### Tâche 15
commande: "grep -c bin /etc/passwd" Explication: "grep" pour rechercher "bin" dans le fichier "/etc/passwd". L'option "-c" de grep indique à grep de compter le nombre de lignes correspondantes a "bin" dans le fichier "/etc/passwd"
### Tâche 16
commande: "grep root /etc/passwd --after-context=3" Explication:Explication: "grep" est utilisée pour rechercher des occurrences d'un motif dans un fichier."--after-context=3 ": C'est une option de grep qui spécifie afficher un certain nombre de lignes après chaque occurrence.
### Tâche 17
commande: "grep -v bin /etc/passwd" Explication:"grep" est utilisée pour rechercher des occurrences d'un motif dans un fichier."-v"
### Tâche 18
commande: "grep '^[[:alpha:]]' /etc/ssh/sshd_config" Explication: "grep" est utilisée pour rechercher des occurrences d'un motif dans un fichier."^" signifie début de la ligne et "[[:alpha:]]" correspond à n'importe quelle lettre de l'alphabet. On aurrait aussi pus choisir l'argument "^[a-zA-Z]"
### Tâche 19
commande: "tr A Z | tr c e" Explication: "tr A Z " remplace toutes les lettre "A" par la lettre "Z"."tr c e "remplace toutes les lettre "c" par la lettre "e".
### Tâche 20
commande: "tr -d C | tr -d c" Explication: "-d" de la commande "tr" est utilisée pour indiquer que l'on souhaite supprimer les caractères spécifiés on aurrai aussi pus utiliser a la place de "tr", "sed", "awk", ou "cut"
### Tâche 21
commande: "rev" Explication: La commande rev est utilisée pour inverser les lignes dans le sens des caractères sous Linux et les systèmes de type Unix.
### Tâche 22
commande: "cut -d':' -f1,6 /etc/passwd | sort" Explication:  "cut" est utilisée pour spécifier les champs à extraire de chaque ligne d'un fichier. "-d':' "spécifie le délimiteur à utiliser pour séparer les champs dans chaque ligne du fichier. L'argument fourni à l'option -f est une liste de numéros de champs ou de plages de champs, séparés par des virgules. "-f1,6" indique que nous voulons extraire le premier champ et le sixième champ de chaque ligne. "sort" trie les lignes en entrée.