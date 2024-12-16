# Clase 03 - Git Desarrollo Colaborativo

## .gitignore
Me permite ignorar archivos o carpetas que quiero que no sean parte del repositorio.

## .gitkeep
Son archivos que permiten que las carpetas vacías puedan ser parte de un repositorio de git.

<https://www.campusmvp.es/recursos/post/que-son-los-archivos-gitkeep-en-git.aspx>

## Ramas (Branches)

### Workflow Reducido
![workflow-reducido](_ref/workflow-reducido.png)

### Workflow Ampliado
![workflow-ampliado](_ref/workflow-ampliado.png)


### Listar ramas

```sh
git branch 
```

### Crear una rama

```sh
git branch <nombre-rama>
git branch feature/branches
```

## Cambiar entre ramas

```sh
git switch <nombre-ramas>
git switch feature/branches
```

## Crear una rama y moverme a esa rama

```sh
git switch -c feature/branches-bis
```

## Fusiones (Merge)
Me permite fusionar ramas entre si. Logrando así obtener los commit de una rama en otra.

### Hay 3 tipos de funsiones

* fast-forward - Automaticas
* Triple vía (Cuando utiliza alguno de los algoritmos/estrategias) - Automaticas
* La fusión con conflicto - Manual 


