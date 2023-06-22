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

    - **Comando**: `git merge main`
    - **Justificación**: El merge del branch main al branch styled no tuvo ningun efecto ni conflicto debido a que el branch styled se origino desde main y no hubieron cambios en main al momento de hacer el merge.

- *El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?*

    Sí, hubieron conflictos. Esto fue debido a que los cambios realizados en el branch styled y htmlify se superponen en las mismas líneas de código con diferentes resultados. 

- *El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?*

    No. El merge no causo conflictos debido a que el branch styled se originó desde main quien no tuvo cambios desde aquel momento. Por lo tanto, los únicos cambios en los archivos que se incorporaran a la rama principal son aquellos que sucedieron en styled.

- *¿Qué comando o comandos utilizaste en el paso 25?*

    `git log --graph`

- *El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?*

    Sí. Se podría haber hecho un merge fast forward debido a que no hubieron cambios en main al momento de mergear.

- *¿Qué comando o comandos utilizaste en el paso 27?*

    `git reset HARD~1` De esta manera regrese el puntero a un commit anterior donde el merge no habia sucedido aún.

- *¿Qué comando o comandos utilizaste en el paso 28?*

    `git restore git-nuestro.md` De esta manera descarto los cambios del working copy.

- *¿Qué comando o comandos utilizaste en el paso 29?*

    `git branch -D title`

- *¿Qué comando o comandos utilizaste en el paso 30?*

    - **Comandos**: 
        - `git reflog`                      Busco el id del commit donde realice el merge de title a main (En mi caso f577cde)
        - `git reset --hard <commit-id>`    En mi caso utilice `git reset --hard f577cde` para regresar el merge a main
    - **Alternativa**: 
        - Se podría haber utilizado tambien `git merge f577cde` para realizar un merge fast-forward al commit generado en el merge eliminado previamente (f577cde)

- *¿Qué comando o comandos usaste en el paso 32?*

    - **Comandos**: 
        - `git reflog`                      Busco el id del commit donde se escribió inicialmente el poema de git-nuestro (En mi caso f577cde)
        - `git checkout <commit-id>`        En mi caso utilice `git checkout f577cde` para colocar el puntero en el commit donde se inició el poema

- *¿Qué comando o comandos usaste en el punto 33?*

    - **Comandos**: 
        - `git reflog`                      Busco el id del commit donde se escribió el título del poema de git-nuestro (En mi caso f577cde)
        - `git checkout <commit-id>`        En mi caso utilice `git checkout f577cde` para colocar el puntero en el commit donde se agregó el título del poema
