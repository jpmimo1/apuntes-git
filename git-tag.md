### Git tag nombre_etiqueta
Lista las etiquetas en orden alfabético.

### Git tag -a nombre_etiqueta -m "mensaje de la etiqueta"
Etiqueta anotada. Se guardan en la base de datos de Git un objeto entero. Tienen un checksum; contienen el nombre del etiquetador, correo electrónico y fecha; y tienen un mensaje asociado.

```
git tag -l "v1.*"
```
Lista las etiquetas que coincidan con el patrón especificado.