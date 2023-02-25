# Curso de _Git_ & _GitHub_

Curso de JonMircha https://www.youtube.com/watch?v=suzMNqDQiyU&t=2193s

## Flujo basico

1. Working Directory (modified).
2. **git add . :** Staging (staged) - pasa los cambios a pendiente.
3. **git commit:** HEAD (Commited) - confirma y guardar en el registro los cambios.
4. **git push:** Remote (In GITHUB) - se suben los cambios al repo remoto.

## Conectar con repositorio remoto

1. **git add remote origin (url repo):** Crea la conexión entre el repositorio local con el repositorio remoto.
2. **git push -u origin master:** El -u se usa cuando la rama en el repositorio remoto no existe, esto permite que en posteriores actualizaciones (push) no se deba especificar el origen ni la rama.

## Obtener cambios del repositorio remoto

1. **git pull:** Trea lo cambios que puede haber agregado otra persona o cambios que se hallan hecho desde github.

## Cambiar el nombre de la rama Master a Main en repositorios existentes

1. **git branch -m master main:** Este comando crea una nueva rama llamada main pero con el comando -m esta remplaza a la rama master quedando como rama principal.
2. **git push -u origin main:** Seguidamente se realiza un push, pero de nuevo con la bandera -u.
3. **git symbolic-ref refs/remotes/origin/HEAD refs/remotes/origin/main:** Luego se debe apuntar el HEAD a la rama main.
4. Ahora se debe cambiar la rama default de master a min en el repositorio remoto en GitHub. Para ello en el GitHub vamos a settings -> Branches -> Cambiar rama.
5. **git push origin --delete master:** Por último eliminamos la rama master del repositorio remoto.