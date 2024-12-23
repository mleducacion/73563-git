# Clase 06 - Git Desarrollo Colaborativo

## Git Reset (Continuación...)
Tener en cuenta que cuando uso el comando, el hash que escribo es el inmiato inferior al que quiero resetear.

## 3 tipos de resets

1. Reset Soft
Va a borrar el commit o los commits seleccionados y arrojar los cambios al staging area

```sh
git reset --soft <hash>
```

2. Reset Mixed
Va a borrar el commit o los commits seleccionados y arrojar el contenido de esos commits dentro de la área Working directory.

```sh
git reset <hash>
git reset --mixed <hash>
```

3. Reset Hard (CUIDADO)
Va a borrar el commit o los commits seleccionados y descartar el contenido. O sea los cambios se pierden.

```sh
git reset <hash>
git reset --hard <hash>
```

# GIT Stash
Es un comando que permite guardar temporalmente todos los cambios que tenemos tanto en el WD como el SA

## Listar los stashes

```sh
git stash list
```

