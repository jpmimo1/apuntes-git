## Curso Git desde cero
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos.

###  Zonas de Git
1. Directorio de trabajo
2. Área de preparación
3. Directorio Git

### Flujo de trabajo básico en Git
1. Modificar una serie de archivos en tu directorio de trabajo.
2. Preparas los archivos, añadiéndolos a tu área de preparación.
3. Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.

### Configurando Git por primera vez
```
git config --global user.name "Jean Paul"
git config --global user.email paul.fa.ac@gmail.com
git config --global core.editor code
git config --list
```
## Configuración SSH en Windows
Usando Git Bash seguimos los siguientes pasos:

1. Creamos una carpeta llamada `llaves-ssh` en el disco `C` para evitar problemas de rutas.

2. Ejecutamos el comando `ssh-keygen -t rsa -C "mi-correo@ejemplo.com"`.
El correo debe ser el mismo con el que nos registramos en Github para evitar posibles problemas.

3. Iniciamos ssh-agent en background ejecutando el comando `eval "$(ssh-agent -s)"`.

4. Agregamos la llave ssh generada a ssh-agent ejecutando el comando `ssh-add /c/llaves-ssh/github_rsa`.

5. Usar el comando `cat /c/llaves-ssh/github_rsa.pub`.
Con este comando vemos el contenido el archivo, copiamos todo el texto que nos muestra.

6. Ir a las configuraciones de nuestro perfil de Github y agregar una nueva llave SSH con el contenido que hemos copiado de `github_rsa.pub`.

Desde ahora podemos hacer pull y push sin que Github nos esté pidiendo los datos de acceso.
