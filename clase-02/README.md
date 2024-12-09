# Clase 02 - Git Desarrollo Colaborativo

## Archivos del Working Directory al Staging Area

```sh
git add <nombre-archivo>
git add <nombre-archivo1> <nombre-archivo2>
git add . # No es tan recomendable.
```

## Hacer un commit de lo que está en el Staging Area

```sh
git commit # Se va abrir un editor de texto para escribir el mensaje
git commit -m "Escribo un mensaje descriptivo sobre lo que se hizo"
```

## Ver historico de commits

```sh
git log
git log --oneline
```

## Recuperar archivos de las diferentes áreas

```sh
git restore . # Recupero todo. Me traigo todo lo que esta en el repo local al working directory. Si tengo archivos modificados pierdo la modificaciones.
git restore <nombre-archivo1> <nombre-archivo2>
git restore --staged <nombre-archivo> # Me recupera los cambios marcados en el staging area al working directory
```
