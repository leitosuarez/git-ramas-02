# Git Ramas (Branches)

# Crear una rama

```sh
git branch <nombre-rama> # crea una rama y nos deja en la rama actual
```

# Me muevo entre ramas

```sh
git switch <nombre-rama>
```

# Una forma de ver el cambio que se hizo en un commit es con

```sh
git show <hash-del-commit> #el hash del commit (id) lo puedo ver con el git log
```

De esta forma vamos a ver que cambios exacatamente hubo de un commit a otro, osea la diferencia, lo que se agrego. Esto es parecido al git diff

# Forma de ver las ramas que tengo en el WD o LR

```sh
git branch
```

Una forma de darse cuenta donde estoy parado es: cuando hago git log "HEAD" va a tener una flechita que a donde apunte es a donde estoy poe ej "HEAD -> feature/ramas"
