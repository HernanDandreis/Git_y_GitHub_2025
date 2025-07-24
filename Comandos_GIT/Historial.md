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