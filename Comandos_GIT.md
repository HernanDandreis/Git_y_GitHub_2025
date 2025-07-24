
## Configurar GIT

git config --global init.defaultBranch [branch name]
    Cambia el nombre de la rama por default.

git branch -m main
    Aplica el cambio de nombre sobre la rama.

git config --global user.name "[user name]"
    Aplica la configuracion de forma global.

git config --global user.email "[email]"
    Aplica la configuracion de forma global.

git config --list
    Lista la configuracion en uso.

## Iniciar un proyecto nuevo

git init 
    Inicia un repo en local.

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

## Gestion de ramas

git branch 
    Indica en que rama estoy.

git checkout -b [branch name]
    Crea una nueva rama.

git checkout [branch name]
    Cambia de rama a la indicada.

git checkout [commit hash]
    Genera un espacio temporal que nos hubica en un commit previo pudiendo hacer cambios
    que no se guardan en el repositorio.

git switch [branch name]
    Cambia de rama a la indicada.

git merge [branch name]
    Agrega y/o pisa el contenido de la rama indicada a la actual.

git branch -D [branch name]
    Elimina la rama indicada.

## Historial

git log 
    Trae el log con la informacion de los hecho en GIT.

git config --global alias.superlog "log --graph --abbrev-commit --decorate --date=relative --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
    Da estetica a log

git tag -a [tag name] -m '[tag message]'
    Crea un tag asociado al ultimo commit

git tag
    Trae la lista de tags existentes

git show [tag name]
    Trae el detalle de la etiqueta incluyendo el mensaje

git tag -d [tag name]
    Elimina el tag sin alternar el historial de commits ni los archivos.