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

## Workflow de trabajo habitual

![Alt text](workflow-git.png)

## Subiendo el repo local al remoto

### Agregar la url del repo remoto al local

```sh
git remote add <alias> <url-repositorio-git>
git remote add origin https://github.com/mleducacion/73563-git.git
```

### Borrar la url del remoto en el repo local 

```sh
git remote remove <alias>
git remote remove <origin>
```

## Subir los commits al remoto 

```sh
git push -u origin main # Se van a trackear las ramas origin/main con main (La primera vez)
```

## Sincronizar el repositorio local con el remoto

```sh
git push
```


