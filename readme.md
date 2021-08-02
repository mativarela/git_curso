## CLASE 2 Branchs

### Regla: 
#### git add -> git commit -> git push
===

##### **Comandos utiles gral:**
- **Fork** -> copia el repo a tu repo personal, con toda la historia.
- **Git clone -url-** -> baja el repo a local
  *-url-* nombre-local -> para cambiarle el nombre, sino toma el original.
- **Git log** -> muestra el historial
  *--online*
  *--all*
  *--graph*
- **Git remote -v** -> muestra el destino del push y fetch
- **Git status** -> muestra el estado de los archivos desde el ultimo cambio. 
- **Git add -archivo/s-** -> agrega archivos al tracking. 
- **Git blame -archivo/s-** -> seguimiento de cambios. Muestra nombre, estado, fecha, etc.
- **Git rm --cached -archivo/s-** -> quita del index los cambios, pero mantiene el mismo en el WorkingDir.
- **Git restore --staged -archivo/s-** -> reestablece los cambios del archivo, a la ultima confirmacion.
- **Git commit -am** -> ADD + Commit
- **Git ammend** -> enmienda errores de commit (mensajes).
- **Git push *repo* *rama*** -> envia los cambios al repositorio, a la rama especificada.
- **Git pull *repo* *rama*** -> te traes los cambios a tu local, merge en caso de ser necesario.
- **Git fetch** -> muestra los cambios realizados en el repo desde el ultimo pull. 
- **Git diff *repos*** -> muestra la comparacion entre local y repo.

##### **Comandos utiles *RAMAS*:**
- **Git branch *-nombre-*** -> crea la rama nombre.
- **Git branch** -> muestra las ramas.
- **Git checkout *-nombre-*** -> cambia a rama -nombre-.

##### *Apuntadores**:
- **HEAD:**
    - Apuntador movil para movernos dentro del historial.
    - Absoluta -> hasd de commit
    - Relativa -> HEAD^^ o HEAD~2

