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

`git config --global user.name "FirstName LastName"`
`git config --global user.email "user@domain.com"`

Generar clave SSH

[Generar SSH Key](https://help.github.com/es/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

[Utilizar SSH](https://medium.com/@ancizj393/crear-una-clave-ssh-en-git-y-vincular-en-tu-cuenta-de-github-e7a6b22bc93f)


### Push Repositorio Remoto
Luego de crear un repositorio en github, debemos ejecutar los siguiente comandos para poder hacer un push.

[Referencia](https://stackoverflow.com/questions/24114676/git-error-failed-to-push-some-refs-t)


`git pull --rebase origin master`

`git push origin master`



### Comandos

`git ini`
> Se realiza en la carpeta raiz, y es el comando que crea el repositorio en local.

`git add [Nombre del archivo]`
> Ejemplo: git add file.txt.
>
> Otro ejemplo es git add * para agregar todos los archivos

`git commit -m "mensaje de referencia"`
> COmmit guarda los cambios en el repositorio local

`gir show [Nombre del archivo]`
>Muestra los ultimos cambios entre la ultima y la ante ultima version.

`git diff [nro commit mas viejo] [otro nro commit mas nuevo] `

>Muestra la diferencia entre dos versiones, se deben pasar los numeros de versiones de los commit.


~~~
~~~


## Staging, Repositorio y Ciclo de basico de trabajo en Git

![Git Ciclo](\images\git_01.PNG)

