## Les branches d'un repo git

La bonne pratique est de ne pas travailler sur la branche principale qui est dédiée à la production.

Les branches de développement permettent d faire évoluer le repo sans edommager le code principal.

1. Créer une nouvelle branche *"dev"* et basculer dessus : ```git checkout -b dev```

2. ```git branch``` Pour avoir l'info des branches existantes et sur laquelle on travaille en vert

3. ```touch readme_branche.md``` Pour créer un fichier readme dans la nouvelle branche *"dev"*