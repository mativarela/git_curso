
# GIT

## CLASE 1 Intro

### Regla: 
#### *cambios*: git add -> git commit -> git push

### Escenarios GIT:
- **Repo Local**: donde realizamos los cambios.
- **Staging**: luego del commit, es donde se confirman y revisan los cambios.
- **Repo Remoto**: version final, en repositorio remoto.


##### **Comandos utiles gral:**
- **Git init** -> inicializa el directorio donde se está parado, para iniciar a trabajar con GIT (se crea el archivo .git)
- **Git add -archivo/s-** -> agrega archivos al tracking, para empezar a hacerle seguimiento, o agregar para Commit. 
- **Git commit** -> Sube los cambios a Staging.
    - *-m*: mensaje de commit
    - *-am*: add + mensaje
- **Git push *repo* *rama*** -> envia los cambios al repositorio, a la rama especificada.
- **Git pull *repo* *rama*** -> te traes los cambios a tu local, merge en caso de ser necesario.
- **Git fetch** -> muestra los cambios realizados en el repo desde el ultimo pull.
- **Fork** -> copia el repo a tu repo personal, con toda la historia.
- **Git clone -url-** -> baja el repo a local
    - *-url-* nombre-local -> para cambiarle el nombre, sino toma el original.
- **Git log** -> muestra el historial
    - *--oneline*
    - *--all*
    - *--graph*
- **Git remote -v** -> muestra el destino del push y fetch
- **Git status** -> muestra el estado de los archivos desde el ultimo cambio. 
- **Git blame -archivo/s-** -> seguimiento de cambios. Muestra nombre, estado, fecha, etc.
- **Git rm --cached -archivo/s-** -> quita del index los cambios, pero mantiene el mismo en el WorkingDir.
- **Git restore --staged -archivo/s-** -> reestablece los cambios del archivo, a la ultima confirmacion.
- **Git ammend** -> enmienda errores de commit (mensajes). 
- **Git diff *repos*** -> muestra la comparacion entre local y repo.


## CLASE 2 Branchs

##### **Comandos utiles *RAMAS*:**
- **Git branch *-nombre-*** -> crea la rama nombre.
- **Git branch** -> muestra las ramas.
- **Git checkout *-nombre-*** -> cambia a rama -nombre-.
- **Git merge *-nombreRama a integrar-*** -> merge los cambios de la rama indicada a la rama donde estoy parado.
    - *Conflicto*: **git status** y se debe aceptar manualmente uno de los cambios. en VSC, se puede hacer visual, borrando y agregando a mano los cambios que quiero mantener, o por menu rapido a mantener origen, destino o ambos. 
- **Git merge --abort** -> vuelve al estado original.

##### **Apuntadores**:
###### Git checkout *apuntador*
- **HEAD:**
    - Apuntador movil para movernos dentro del historial.
    - Absoluta -> hash de commit
    - Relativa -> HEAD^^ o HEAD~2

- **BRANCH:**
    - Apuntador dinamico que se para sobre el ultimo *commit* de una historia en particular. 
    - Podemos crear ramas a partir de cualqueir *commit*.
