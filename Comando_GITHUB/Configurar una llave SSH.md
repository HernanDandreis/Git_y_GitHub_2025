## Configurar una SHH

ssh-keygen -t ed25519 -C "[email@email.com]"
    Crea la llave SSH

eval "$(ssh-agent -s)"
    Confirma que el agente de SSH esta funcionando

ssh-add [ssh key path]
    Guarda la llaves dentro del agente

ssh -T git@github.com
    Establece una conexion con GITHUB para confirmar que todo este OK