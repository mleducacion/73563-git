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