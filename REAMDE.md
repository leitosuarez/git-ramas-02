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

En resumen HEAD es un puntero que apunta hacia el ultimo commit de la rama a la que estoy

# Acordarse de hacer:

```sh
git push -u origin <nombre-de-la-rama> #esto es para que se suba al repo remoto la rama, si yo no hago esto la rama nunca va a aparecer en el remoto
```

# Para ver las ramas locales (no subidas) y remotas (subidas) que tengo, tengo que usar el comando:

```sh
git brnach -a # esto sirve mucho para abobinarme de si subi o no la rama
```

# Como traer el contenido de una rama a la main:

```sh
#estando en la rama en la cual me quiero traer las cosas tengo que hacer el comando:
git merge <nombre-de-la-rama> # esto va a fusionar el contenido de la rama main con el de la rama que que quremos que se fucione
```

# Como borrar una rama:

```sh
git branch -d <nombre-de-la-rama> # si la rama que estou borrando ya fue fusionada me va a borrar la rama
git branch -D <nombre-de-la-rama> # confirmacion de borrado de una rama que todavia no ha sido fucionada en el repositorio
```

* Fusion: Fast-forward : git hace la fusion automaticamente (aca no genera un commit extra)
* Fusion: Con estrategia : git hace la fusion automaticamente. (genera un commit donde se soluciona automaticamente la situacion)
* Fusion: Con conflicto : git no puede fusionar automaticamente, entonces nos va a pedir ayuda

# Abortar la fusion

```sh
git merge --abort
```
# Manera de solucionar un conflicto al fusionar ramas

Para ello debemos editar el archivo, eliminar las lineas "========" y "<<<<<<<<>>>>>>>>" (osea modificar manualmente el archivo) que van a aparecer y luego hacer un git add y un git commit, eso es todo.