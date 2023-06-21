# Entrega módulo GIT

*Alumno: Gonzalo Gregorio*

*Ejercicio 1:*

- *¿Qué comando utilizaste en el paso 11? ¿Por qué?*

    - **Comando**: `git reset --hard HEAD~1` 
    - **Justificación**: El `reset --hard` es una combinacion del reset (deshacer un commit) + restore (deshacer cambios en el working directory). Como el commit que se quería deshacer era el último se combino el `reset --hard` con el `HARD~1` para indicar al puntero que debía ir al commit anterior.

- *¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?*

    - **Comandos**: 
      - `git reflog` 
      - `git reset --hard <commit-id>` 
    - **Justificación**: El primer comando `git reflog` lo utilice para obtener el id del commit al cual queria llevar el puntero (en mi caso, el id a70413f). Luego utilice el commando `git reset --hard a70413f` para restaurar los cambios + el commit en mi branch.

- *El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?*



- *El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?*



- *El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?*



- *¿Qué comando o comandos utilizaste en el paso 25?*



- *El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?*



- *¿Qué comando o comandos utilizaste en el paso 27?*



- *¿Qué comando o comandos utilizaste en el paso 28?*



- *¿Qué comando o comandos utilizaste en el paso 29?*



- *¿Qué comando o comandos utilizaste en el paso 30?*



- *¿Qué comando o comandos usaste en el paso 32?*



- *¿Qué comando o comandos usaste en el punto 33?*


