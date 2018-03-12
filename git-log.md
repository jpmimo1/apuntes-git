### Git log
Muestra todo el historial de commits del proyecto

`git log --pretty=format:"%h - %an, %ar : %s"`
Muestra el historial con el formato que indicamos.

### Limitar la salida del historial
`git log -n`: Cambiamos la n por cualquier número entero, por ejemplo: `git log -2` nos mostrará los 2 commits más recientes.

`git log --after="2018-03-12 03:00:00"`: Muestra los commits realizados después de la fecha especificada.

`git log --before="2018-03-12 03:00:00"`: Muestra los commits antes de la fecha especificada.

Las banderas del comando `git log` se pueden usar juntas según convenga, por ejemplo:
` git log --before="2018-03-12 03:00:00" --after="2018-03-12 02:30:00"`