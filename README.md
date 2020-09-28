# Instrucciones para usar los comandos de git

Tenemos que tener dos opciones en cuenta.

## Primer paso

Usamos el comando **git init** para inicializar un archivo git el cual permanece oculto, una vez ejecutado este comando podemos volverlo a utilizar sin problema, así que no hay que preocuparse.


### Segundo paso

Tenemos que pensar varias cosas, ¿Tenemos un repo creado, es un fork, lo hemos clonado?



### Nuevo repositorio

Si vamos a crear un repositorio nuevo nos saldrá esto:

https://github.com/Zetzher/Instrucciones-Github/blob/master/github_nuevo.png

Una vez creado, tendremos que vincularlo nuestra versión local con nuestra versión en github, con lo que tenemos que hacer:

git remote add origin <link del repo>, en mi caso <git remote add origin https://github.com/Zetzher/Instrucciones-Github.git>;


## Repositorio ya creado o realizado con fork

No hará falta que hagamos el comando git remote add origin con el link del repo porque ya está vinculado.


### Comandos

Cuando hacemos algún cambio que queremos que se refleje en nuestro repo de github:

git add

Y tenemos que tener varias opciones en cuenta:

1. Si queremos subir todos los archivos utilizaremos <git add .>
2. Si queremos subir un archivo o varios <git add <nombre del archivo>>

Después tenemos que dejar un comentario:

git commit -m <comentario>, por ejemplo, git commit -m "La imagen está redimensionada"

Y por último:

git push

Ahora tenemos que tener una cosa en cuenta, queremos subirlo a la rama master o a otra rama:


Si queremos subirlo a la rama master:

git push origin master


Y en el caso de que sea en otra rama:

git push origin <nombre de la rama>, por ejemplo, git push origin julian
