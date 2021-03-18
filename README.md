# Test de git

![Git logo](https://res.cloudinary.com/practicaldev/image/fetch/s---Xg28U2u--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/q7uy4yxekcljpr70p2xk.png)

## Principe de base
    * git rm --cached enleve de la stagging area

    * git add * ajoute tout les fichier sauf les fichier commencant par un point 

    * git diff changement/ajout


> Pas de dépôt git dans un dépôt git

    * git branch <nom_branche>

> Git head pointe vers la branche master

    * git branch -a affiche toute les branches

    * git branch affiche les branches local

     * git checkout <nom_de_la_branche> creation de branche 

    * git checkout -b <nom_de_la_branche> creation et aller directement sur la branche
 
![Git logo](/assets/capt01.png)

    * git branch -D <nom_de_la_branche> supprime la branch

## Fusion des branches
 * git merge <nom_de_la_branche>

### Gestion des conflits
    * Push impossible 
    * Faire un fetch avant
  > git fetch
  
  > git merge || git pull
 * Resoudre les conflits

## Remote
 Utilisation d'une remote

    * git remote add <nom de remote> <url du dépot>
    * git fetch <nom de remote>
    * (modification des fichier)
    * git add *
    * git commit -m "message"
    * git <nom de remote> <nom de branche>

## Stash
Avant un add (limite dernier commit dans le depot local)

    * git stash  annule modif
    * git stash pop  Voir changement annulé
    * git stash show  Voir les changement annulé
    * git stash drop  Supprimer dernier remisage
    * git stash clear  Vide la pile


## Commit
Modification de commit

    * git commit --amend  -m "nouveau message" remplace le message du dernioer commit
    * git revert <id du commit> reviens au commit
    * git revert HEAD~3. .HEAD revjiend de trois commit en arriere (creez un nouveau commit)
    *git reset <nom du commit > supprime tout les commit apres ce commit reviens a cette etat.

<!-- ## Pull request -->