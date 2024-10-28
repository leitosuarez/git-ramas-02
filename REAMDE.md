# Git Ramas (Branches)

# Una forma de ver el cambio que se hizo en un commit es con

```sh
git show <hash-del-commit> #el hash del commit (id) lo puedo ver con el git log
```

De esta forma vamos a ver que cambios exacatamente hubo de un commit a otro, osea la diferencia, lo que se agrego. Esto es parecido al git diff

# Acordarse de hacer:

```sh
git push -u origin <nombre-de-la-rama> #esto es para que se suba al repo remoto la rama, si yo no hago esto la rama nunca va a aparecer en el remoto
```