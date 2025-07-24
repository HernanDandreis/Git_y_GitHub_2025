## Clonar repositorios

git clone [repo URL]
    Clona el repositorio de GITHUB a nuestro local (Metodo sin SSH)

git clone [SHH URL]
    Clona el repositorio de GITHUB a nuestro local (Metodo sin SSH)

## Configurar una SHH

ssh-keygen -t ed25519 -C "[email@email.com]"
    Crea la llave SSH

eval "$(ssh-agent -s)"
    Confirma que el agente de SSH esta funcionando

ssh-add [ssh key path]
    Guarda la llaves dentro del agente

ssh -T git@github.com
    Establece una conexion con GITHUB para confirmar que todo este OK

## Actualiar repositorios local-nube / nube-local

git pull 
    Actualiza el repo local con la informacion de la rama main

git push origin [branch]
    Sube la informacion en stage al repositorio en la nube

git push -u origin [new branch]
    Sube la informacion en stange al repositorio en la nube creando una nueva rama

git fetch origin
    Actualiza la informacion en el repo local pero no realizar el merge automaticamente

git log main..origin/main
    Me deja ver en el log la actualizacion traida con fetch

git merge origin/main
    Confirma el merge de la informacion traida con fetch