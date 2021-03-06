# Curso Profesional de Git y GitHub

## Indice
    1. Datos del curso
    2. Fuentes
    3. Resumen

## Datos del curso
Link: [Curso en Platzi](https://platzi.com/clases/1557-git-github/)

Author: Jhon Fredy Vega
Twitter:

## Fuentes

## Resumen

### 01 - Configurar Git
Configurar User & Email

`git config --global user.name "Emmanuel Capandegui"`
`git config --global user.email "ecapandegui@outlook.com"`

Generar clave SSH

[Generar SSH Key](https://help.github.com/es/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

[Utilizar SSH](https://medium.com/@ancizj393/crear-una-clave-ssh-en-git-y-vincular-en-tu-cuenta-de-github-e7a6b22bc93f)


### Push Repositorio Remoto
Luego de crear un repositorio en github, debemos ejecutar los siguiente comandos para poder hacer un push.

[Referencia](https://stackoverflow.com/questions/24114676/git-error-failed-to-push-some-refs-t)


`git pull --rebase origin master`

`git pull origin master --allow-unrelated-histories`
>Permite fusionar las ramas, para los casos en que arroje error por no ser iguales las historias de las ramas.

`git fetch`

`git push origin master`



### Comandos

`git ini`
> Se realiza en la carpeta raiz, y es el comando que crea el repositorio en local.

`git add [Nombre del archivo]`
> Ejemplo: git add file.txt.
>
> Otro ejemplo es git add * para agregar todos los archivos

![Git Ciclo](images/git_02.PNG)


`git commit -m "mensaje de referencia"`
> Commit guarda los cambios en el repositorio local

`gir show [Nombre del archivo]`
>Muestra los ultimos cambios entre la ultima y la ante ultima version.

`git diff [nro commit mas viejo] [otro nro commit mas nuevo] `

>Muestra la diferencia entre dos versiones, se deben pasar los numeros de versiones de los commit.

`git log [nombre del archivo]`

`git log [nombre del archivo] --state`

`git reset [nro de commint] [--hard | --soft]`

>La opccion --hard vuelve los archivos o la version seleccionada, borrando los commit posteriores a ese.
>La opcion --soft vielve los archivos a la version seleccionada, pero mantiene los archivos que se encuentran en staging.

### Git RM
Este comando nos ayuda a eliminar archivos de Git sin eliminar su historial del sistema de versiones. 

`git rm --cached`
> Elimina los archivos del área de Staging y del próximo commit pero los mantiene en nuestro disco duro.

`git rm --forced`
> Elimina los archivos del disco duro. Pero git mantiene le historial por lo que es posible recuperarlo.

### Checkout

`git checkout [nro de commit] [nombre del archivo]`
>Ejemplo git checkpu master documento.txt

~~~
~~~


## Staging, Repositorio y Ciclo de basico de trabajo en Git

El "staging area" (Tambien denominado Index) es un area en memoria ram en la cual se agregan los archivos previo al commit. Un archivo que se encuentra en staging se dice que esta en estado __Staged__

![Git Ciclo](images/git_01.PNG)

