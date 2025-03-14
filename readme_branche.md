# Les branches d'un repo git

La bonne pratique est de ne pas travailler sur la branche principale qui est dédiée à la production.

Les branches de développement permettent d faire évoluer le repo sans edommager le code principal.

1. Créer une nouvelle branche *"dev"* et basculer dessus : ```git checkout -b dev```

2. ```git branch``` Pour avoir l'info des branches existantes et sur laquelle on travaille en vert

3. ```touch readme_branche.md``` Pour créer un fichier readme dans la nouvelle branche *"dev"*

4. Pour pousser cette nouvelle branche, le premier push se fait avec l'option d'origine de la nouvelle branche *"dev"* :
```
git push -u origin dev
```

5. On modifie qu'il n'y a qu'un push simple à faire :
```
git commit -a -m "complément ... add + commit directement"

git push
```

**Conclusion**

La nouvelle branche dev est bien à jour dans le repo github

## Fermer une branche pour la rattacher à la principale

1. ```git checkout main``` pour reprendre la main sur la branche principale *"main"*

2. ```git merge``` dev pour effectuer le merge de la branche *"dev"* sur la branche *"main"*

3. ```git push``` pour publier les élements de la branche *"dev"* dans la branche *"main"*

*Checker sur la branche main du github si les éléments de la branche dev on bien été rajouté.*