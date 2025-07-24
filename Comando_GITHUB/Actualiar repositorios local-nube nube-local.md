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