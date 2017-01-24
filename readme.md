*¿Qué comando utilizaste en el paso 11? ¿Por qué?
git reset --hard HEAD~1 => deshace el último commit, dejando el working copy como estaba antes, vacía el staging area(ideal para recuperar ficheros, descartar cambios experimentales, etc)

*¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
git reflog lo que me devuelve el registro de las acciones sobre el repositorio, entre los datos el SHA del commit que se deshizo. 
Con el SHA correspondiente(52947fa) ejecuto git reset --hard 52947fa

*El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
NO causa ningún conflicto, sólo nos indica que la rama styled está actualizada.

*El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
SI causa ningún conflicto, dado que hay diferencias en el fichero git-nuestro.md de la rama styled y la rama htmlify.

*El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No causa ningun conflicto, actualiza con un fast-forward el fichero git-nuestro.md

*¿Qué comando o comandos utilizaste en el paso 25?
git log --graph --decorate --pretty

El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Si podría ya que title solo tiene el titulo adicional para ser incorporado en la rama master.

¿Qué comando o comandos utilizaste en el paso 27?
git reset HEAD~1

¿Qué comando o comandos utilizaste en el paso 28?
git checkout git-nuestro.md

¿Qué comando o comandos utilizaste en el paso 29?
git branch -D title

¿Qué comando o comandos utilizaste en el paso 30?
git reflog para mirar el SHA del merge que realizamos pasos atrás
git reset --hard f1e5929 para volver a ese merge

¿Qué comando o comandos usaste en el paso 32?
git reflog para mirar el SHA del commit inicial
git reset --hard 8930ba3 para volver a ese commit

¿Qué comando o comandos usaste en el punto 33?
git reflog para mirar el SHA del commit cuando añadimos el título
git reset --hard 8930ba3 para volver a ese commit