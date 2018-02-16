# Git

Fiche mémo

Nos fichiers sont sur nos ordi, le add les met dans la zone de déchargement (staging area), le commit le met dans l'entrepôt local (toujours sur notre ordi qui est un repository), le push le met dans github (qui est un autre repository).

Dans l'entrepôt , on peut mettre plusieurs commits et les pusher en une fois

| EXPRESSION | A QUOI CA SERT ? | EXEMPLE D'UTILISATION |
| --- | --- | --- |
| git | Pour spécifier qu'on est en git |   |
| cd | Pour aller à la racine du dossier |	|
| cd ../nom du fichier.extension | Pour revenir en arrière et aller sur le fichier spécifié |	|
| $ git init | Pour configurer les outils dont git aura besoin  
git remote add origin URL_DE_TON_REPOSITORY

git add . 
puis git commit -m "Initial commit" 
enfin git push -u origin master|   |
| $ pwd | Pour savoir où on est (dans le C :, ou dans P :…) |   |
| $git status | Permet de savoir ce qu'il s'est passé depuis la dernière fois (si commit, si add...) |   |
| $ git clone (+nom adresse du fichier à cloner) | Pour faire la copie du fichier sur lequel on veut travailler |   |
| $git diff | Pour voir quelles sont les différences entre le fichier en local (sur lequel on a fait les changements) et le staging area |   |
| $git add +  nom du fichier | Ce qui fera partie de ma prochaine version, stocké dans le staging area | On peut faire ensuite un $git status pour vérifier les changements |
| $git commit | Pour enregistrer le fichier dans le staging area ET on rajoute un commentaire rapide qui explique ce qu'on a modifié en rajoutant -m(pour message) « ... » |
| $git commit -m "J'ai effectué telle modification" |
| Sha 1 | Identifiant unique créée automatiquement pour chaque utilisateur à chaque changement | [master 7cd7258] |
| $ git add '*.txt' | Ajoutera toutes les fichiers .txt du dossier dans le staging area |   |
| $ git log | Fonctionne comme un journal qui permet d'afficher tous les changements (dans l'ordre et qui a effectué les changements), il affiche l'historique des commits. Appuyer sur la touche q pour sortir du log |   |
| $git push | Pour le mettre sur github qui l'affichera | Si on veut spécifier le chemin, la première fois on rajoute -u et les noms des emplacements, on n'aura plus à le faire ensuite |
| $git pulll | Pour vérifier si des changements ont été effectué dans le projet |   |
| $ git diff --staged | Pour voir les changements que vous venez juste de déposer |   |
| $ git reset  (+dossier/fichier) | Pour désactiver/supprimer des fichiers du staging | Le fichier apparait encore mais il est désactivé |
|   |   |   |
| $ git checkout - -  (+ nom de fichier) | Pour revenir à l&#39;état avant le dernier changement |   |
| $ git branch (+nom de la branche à créer) | On crée une nouvelle branche (si par exemple on a fait des copies pour faire du débug et qu&#39;ensuite on veut faire du ménage) |   |
| $ git checkout (+nom de la branche créée) | Pour switcher de l&#39;ancienne branche à la nouvelle |   |
| $ git rm '*.txt'; | Pour supprimer les fichiers du dossiers et du staging |   |
| $ git merge (+nom de la branche) | On va sur la branche que l&#39;on veut garder puis on tape git merge (+nom de la branche sur laquelle on a fait des changements) cela fusionnera la branche sur laquelle on est et celle sur laquelle on a fait des modifs |   |
| $  git branch -d (+nom de la branche) | Cela supprime la branche nommée |   |
|   |   |   |
|   |   |   |

