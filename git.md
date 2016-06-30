# CURSO GIT

1. git init
1. git add .
1. git commit -m "app inicial"
1. git remote add origin https://github.com/yayomanosalva/Curso-Rails.git
1. git push -u origin master

## configuracion

  ```bash
  -->> git config --global user.name "jair manosalva"
  -->> git config --global user.mail yayomanosalva@gmail.com
  -->> git config --global core.editor sublime          --->>> configuras el editor preferido
  -->> git config --global -l                           --->>> Muestra las configuraciones de git
  -->> git config --global alias.st status              --->>> puedes cambiar el comando por un alias
  ```

## Glosario

   ```bash
  1. git init                                           --->>> Creamos un repositorio en el directorio actual
  2. git clone direccionURL /name.git (nombreProyecto)  --->>> clona un repositorio existente dentro de un directorio
  3. git add nombreArchivo (.)                          --->>> agraga al repositorio los archivos que le indiquemos
  4. git commit -m "mensaje"                            --->>> hace cometario
  5. git commit -a                                      --->>> añade todos los commits
  6. git rm (archivo)                                   --->>> borra el archivo/Dir del repositorio local
  7. git mv origen destino                              --->>> mover a nueva ruta
  8. git status                                         --->>> informe estado actual
  9. git diff                                           --->>> muestra los cambios/diferencias en local
  10. git diff - -staged                                --->>> muestra los cambios/diferencias en index
  11. git stash                                         --->>> cuando se quiere registrar el estado actual del directorio de trabajo y el índice, pero quiere volver a un directorio de trabajo limpio
  12. pwd                                               --->>> comando linux para ubicacion de directirio
  ```

## RAMAS
    
```bash
    1- git checkout -b  <nombre de rama>       --->>> Crea una nueva rama
    2- git checkout master                     --->>> vuelve a la rama principal
    3- git branch -d <nombre de rama>          --->>> borra la rama
    4- git push origin <branch>                --->>> subas (push) la rama a tu repositorio remoto
    5- git branch                              --->>> ver rama actual
    6- git checkout -- archivo                 --->>> dos guiones y un espacio en blanco
    7- git branch -m old_branch new_branch     --->>> Renombrar Rama
    8- git rm -r directoio_a_borrar            --->>> Borrar Directorio Completo
```

## .git log

```bash
    1- git log                                           --->>> Muestra la historia d los commits completa con el formato predeterminado
    2- git log -n 3                                      --->>>los ultimos 3 cambios
    3- git log --oneline                                 --->>> Resumen en una linea
    4- git log --stat                                    --->>> Que archivos han cambiado y el numero relativo de lineas añadido o cambiado
    5- git log --author="jair"                           --->>> Que commits ha realizado ese autor
    6- git log --decorate                                --->>> Añade los nombres de ramas o etiquetas de los cambios
```

## actualiza & fusiona

```bash
    1- git pull                                          --->>> Para actualizar tu repositorio local al commit más nuevo
    2- git merge <branch>                                --->>> Para fusionar otra rama a tu rama activa (por ejemplo master)
```

## .git ignore

```bash
    >ls -a
    >cd .git
    >ls -a
    >cd info
    >ls -a
    <- Muestra un archivo con nombre exclude ->
    >cat exclude
    >nano exclude
    <- Añadimos el archivo que queremos ignorar .DS_Store ->
    >comando + x
    >y
    <- Listo se guardó el archivo ->
```

## deleted

```bash 
> git add             --->>> updates all your changes - asi allas eliminado una carpeta, actualia el repositorio.
```

## subir al repositorio bitbucker

```bash
  despues de git push origin <branch>, te cambias de rama a dev con -> git checkout <branch>
y haces git pull. y si quieres borrar la rama arriba.

> git stash pop                                       --->>> vuelve al estado anterior
> git stash                                           --->>> continuar sin cambios
```