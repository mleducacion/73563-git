# Clase 05 - Git Desarrollo Colaborativo

## Clonar un repositorio remoto en el local

```sh
# Me crea una carpeta y dentro me clona el respositorio
git clone https://github.com/mleducacion/proyecto-helado.git 
# Si quiero que me lo clone en el directorio actual coloco ./
git clone https://github.com/mleducacion/proyecto-helado.git ./ 
```

## Para descargar la metada

```sh
git fetch # Me actualiza la carpeta .git
```

## Para descargar los commits de una rama en especifico

```sh
git pull <remoto> <rama>
git pull origin maxi # Me traigo la rama maxi del remoto a la rama maxi local
```

## Alias: Formas cortas de disparar un comando

```sh
git config --global alias.<alias-elegido> "<comando-de-git-sin-la-palabra-git>"
git config --global alias.s "status --short"
git config --global alias.l "log --oneline"
git config --global alias.ll "log --oneline --decorate --all --graph"
git config --global alias.c "commit -m"
```

## Quitar un alias

```sh
git config --global --unset alias.ll
```

## Listar los alias

```sh
git config --global --get-regexp alias
```

## Para guardar especificamente parte del código fuente que estoy creando

```sh
git add --patch
```

* y -> YES | Para ponerle el hunk en el staging
* n -> No | para no poner ese hunk en el staging
* s -> split | Divide automanticamente los hunks
* e -> Manual | Elijo manualmente que líneas quiero que se guarden en staging area
    * \+ eso va ir al SA
    * ' ' Si le saco el + esa línea no va a formar parte de lo que guarde en SA




