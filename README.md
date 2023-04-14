**Nom :** Baillobay Trystan

**Groupe :** B

**Année :** 1ère

**IUT Le Havre - Cours GIT**

# Compte-rendu TP2 Introduction GIT

Dans ce TP on s'initie à GitHub, aux répertoires distants.
Ce compte rendu me servira seulement à citer les commandes "utiles" vues aucours du TP, *une aide mémoire*
Les explications sont synthétiques, elles ne servent pas à reproduire le TP à la lettre.

## 1.  Créer un compte sur github

> Mon compte : nom d'utilisateur : **ydroo**

## 2.  Ajouter une nouvelle clé SSH à votre compte GitHub

* Penser à entrer des noms explicites, pour mieux se retrouver quand plusieurs machines seront renseignées 
* Pour copier la clé SSH publique de sa machine : ``` cat ~/.ssh/id_rsa.pub ```

## 3.  Pousser un dépôt existant depuis la ligne de commande

```git remote [...]```

Cette commande sert à gérer (ajouter) des dépôts distants (“remotes”). En d’autres termes, nous utiliserons cette commande pour créer un lien entre notre dépôt local tp1 et celui distant que nous allons créer dans github.

Avec ce corps de commande nous pouvons aussi faire :

* ```git remote -v``` : Nous retourne le répertoire distant sur lequel nous travaillons (ne renvoie rien si aucun répertoire distant)
* ```git remote remove fichier``` : Retire un fichier dans le répertoire distant
* ```git remote rename ancien nouveau``` : Renomme un fichier dans le répertoire distant
* ```git remote add url``` : Ajoute un répertoire distant sur lequel travailler
* ```...```

```git push```
Cette commande permet de mettre à jour le dépôt distant (e.g. github) à partir de la dernière version validée (commit) de notre dépôt local.

```git pull```
Cette commande sert à mettre à jour notre dépot local à partir de la dernière version de notre dépôt distant.

```git branch```
Cette commande renvoie la branche distante sur la quelle nous opérons (généralement **main** ou **master**)

## 4.  Séquence de travail avec un dépôt distant

```git status```
Cette commande permet de savoir si les fichiers ont été mis à jour/ajoutés dans le dépot distant.

```git log```
Cette commande nous permet de voir les modifications les plus récentes ainsi que leur commit renseignés.

## 5. Nous avons aussi vu comment cloner un répertoire distant en local :

**Ajouter/Mettre à jour un fichier du local au GitHub :**```git add (fichier)```

**Ajouter un commentaire à la modification effectuée :** ```git commit -m "Commentaire"```

**Appliquer les modification au GitHub :** ```git push```


