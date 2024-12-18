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
```

