`git config pull.rebase false`: Fusiona la rama local y la remota, lo ideal es usarla para mantener el historial de cambioses la opcion por default.

`git config pull.rebase true`: La rama remota va a rebasa a las locales y sobreescribe sus cambios haciendo que si la rama local quiere subir sus cambios entonces deberá hacerlos de nuevo, es la opcion mas practica.

`git config pull.ff only`: Pone los cambios de la rama local por encima de los de la remota.
