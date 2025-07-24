## Actualializar archivos (local)

git status
    Muestra el estado de los archivos del repo.

git add [file name]
    Actualiza el archivo localmente colocandolo en un estado de staging.

git add .
    Actualiza todos los archivos localmente colocandolo en un estado de staging.

git rm --cached [file name]
    Retrotrae el estado de stage del archivo.

git rm --cached .
    Retrotrae el estado stage de todos los archivos.

git rm --force [file name]
    Retrotrae el estado de stage del archivo (forzandolo).

git rm --force .
    Retrotrae el estado de stage de todos los archivos (forzandolos).

git commit -m '[commit message]'
    Commitea los cambios en estado stage.

git restore [file name]
    Deshace los cambios en el director de trabajo.

git stage --staged [file name]
    Deshace los cambios en el area de stage.

git restore --source=HEAD --staged --worktree [file name]
    Deshacer los cambios en el director de trabajo y el stage.

git revert [commit hash]
    Crea un nuevo commit que revierte los cambios de un commit especifico. sin eliminar 
    el historial.

git reset --soft [commit hash]
    Mueve el HEAD a un commit especifo guardando los git cambios en el stage.

git reset --mixed [commit hash]
    Mueve el HEAD a un commit especifo, deshace los cambios en el stage pero mantiene los
    mantiene los cambios en el directorio.

git reset --hard [commit hash]
    Mueve el HEAD a un commit especifo, deshace los cambios en el stage y borra los
    los cambios en el directorio.