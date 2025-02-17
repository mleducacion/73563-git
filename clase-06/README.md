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

## Recuperar un stash 

1. Pop
Siempre recupera el último colocado en el stash. Y si no hay conflicto, borra el stash

```sh
git stash pop
```

2. Apply
Le indico cual quiero recuperar. Y el que recupero no se borra de la lista de stash

```sh
git stash apply 4
git stash apply stash@{4}
```

## Borrar un stash

```sh
git stash drop # el último
git stash drop stash@{4} # El 4 indicado
git stash drop 4 # El 4 indicado
```

## Borrar todos los stashes

```sh
git stash clear
```

**NOTA IMPORTANTE**: Los stashes son solo locales. No se pueden subir al remoto.

# Git Cherry Pick
Permite selecionar un commit o varios de manera independiente y colocars en otra rama.

## Selecciono un único commit 

```sh
git cherry-pick <hash>
```

### Para avanzar en la solución si hay conflicto
Si hay conflicto, solucionarlo y hacer los siguientes pasos

```sh
git add .
```

```sh
git cherry-pick --continue
```

### Seleciono varios commits con extremos

```sh
git cherry-pick <hash>^..<hash>
```

### Seleciono varios commits sin extremos

```sh
git cherry-pick <hash>..<hash>
```

# GITHUB CLI
Es una herramienta para interacturar con los repositorio remotos de GITHUB.

<https://cli.github.com/>


## Contacto

* maxi.principe@gmail.com
* mlapeducacion@gmail.com
