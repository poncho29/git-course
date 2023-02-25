# Curso de _Git_ & _GitHub_

Curso de JonMircha

## Flujo basico

1. Working Directory (modified).
2. git add . -> Staging (staged) pasa los cambios a pendiente.
3. git commit -> HEAD (Commited) confirma y guardar en el registro los cambios.
4. git push -> Remote (In GITHUB) se suben los cambios al repo remoto.

## Conectar con repositorio remoto

1. git add remote origin (url repo): Crea la connexion entre el repositorio local con el repositorio remoto.
2. git push -u origin master: El -u se usa cuando la rama en el repositorio remoto no existe, esto permite que en posteriores actualizaciones (push) no se deba especificar el origen ni la rama.