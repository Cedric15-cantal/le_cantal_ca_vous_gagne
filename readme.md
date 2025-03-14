**Tuto git le Cantal ça vous gagne**
--

![](img/CANTAL_Logo_Rouge_RVB_72dpi.png)

**Préalable : Création d'un repo distant sur la plateforme github**

1. Création d'un dossier sur le PC => pour le moment dossier classique

2. Création du 1er fichier readme.md (page d'accueil de notre repo)

3. Initialisation du dossier classique comme un repo local avec la commande : ```git init```
Cette commande entraîne la création d'un sous répertoire ***".git"***, notre dossier *"classique"* local est devenu un repository au sens git du terme.

4. Vérification du statut des commits dans le dossier .git : ```git status```

5. On va le versionner dans notre dossier ***".git"*** en stageant le fichier "readme.md" : ```git add readme.md```

6. On configure notre dossier ***".git"*** pour effectuer les commit, deux commandes pour cela : ```git config --global user.name "Cedric15-cantal"``` et ```git config --global user.email "courageot63@gmail.com"```

7. On effectue le premier commit en rajoutant l'option -m pour ajouter un message (qui apparaîtra dans le repo github) : ```git commit -m "premier commit du tuto"```

8. On renomme la branche principale en *"main"* (git en local a créé la branche principale en "master", alors que github attend par convention cette même branche principale en "main") : ```git branch -M main```

9. On crée le lien de notre repo local avec le repo distant : ```git remote add origin https://github.com/Cedric15-cantal/le_cantal_ca_vous_gagne.git```

10. On *"push"* le repo local vers le distant (publication) : ```git push -u origin main```

**Conculsion**

Notre repo local est jumelé avec le distant. Vu que je viens de compéter ce fichier readme.md après le premier commit, je me contredis moi-même, je dois donc refaire un commit pour être "iso".

**Mise à jour du repo github avec les différentes modif des fichiers et dossiers effectuées dans le dossier d'origine :**

1. ```git add *``` (Pour stagger tous les dossiers et documents en plus du readme.md dans le dossier du repo)

2. ```git commit -m "complément ..."``` (Pour avoir une trace des modif sur le repo github c'est bien de rajouter des messages pour chaque commit)

3. ```git push``` (Simplement cette commande sans rajouter l'origine de la branche principale car elle a été formatée lors du premier push)

