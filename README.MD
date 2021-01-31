# Comandos basicos para GIT

GIT es el SCV (sistema de control de versiones) de código abierto más utilizado que te permite rastrear los cambios realizados en los archivos. Las empresas y los programadores suelen utilizar el GIT para colaborar en el desarrollo de software y aplicaciones.

El objetivo de esta guia, recordar de vez en cuando los comando basicos de git. Existen muchas paginas y cursos por todo internet que hablan de ellos, por Udemy y Youtube existen varios.

Un video basico es de Fernando Herrera, [12 Comandos de Git que debe de saber](https://www.youtube.com/watch?v=iT4UOkyI09k)

[git - guia sencilla](https://rogerdudler.github.io/git-guide/index.es.html) por Roger Dudler

Entre otros, iniciemos con los comandos.

## git --version

Muestra el numero de version de GIT instalado en nuestro PC, la importancia de esto son los comandos que permite las diferentes versiones.

```
git --version
```

## git init

Crea un nuevo repositorio local GIT.

```
git init
git init [nombre direcctorio]
```

Copiar un repositorio, que se encuentra en un servidor remoto.

```
git clone nombredeusuario@host:/path/to/repository
```

Agregar archivos al area de trabajo y con . agrega todos los que han tenido cambio.

```
git add .
git add <tempfile.txt>
```

Crear una fotografia del estado actual de los archivos.

```
git commit -m "mensaje para el commit"
```

Matando dos pajaros de un tiro, el (git add . + git commit -m)

```
git commit -am "mensaje para el commit"
```

Revertir todos los cambio que hace git commit

```
git reset .
```

Muestra la lista de los archivos que se han cambiado junto con los archivos que están por ser preparados o confirmados

```
git status
```

Restaura los cambios antes de el ultimo commit

```
git checkout -- .
```

Mostrar los cambio o commit realizados

```
git log
```

Edita el resultado de los log, mostrados

```
git commit --amend
```

Crea ramas y te ayuda a navegar entre ellas. Por ejemplo, el siguiente comando crea una nueva y automáticamente se cambia a ella

```
git checkout -b rama-nueva
```

Muestra las ramas existentes y con (\*) la rama actual donde se trabaja

```
git branch
```

Cambiar de rama se indica el nombre de la rama.

```
git checkout [nombre_rama]
```

Para fusionar una rama con otra rama activa

```
git merge <rama-name>
```

Borrar una rama

```
git branch -d <rama-name>
```

Renombra la rama master a main

```
git branch -M main
```

Asigna la ruta destino del reposito

```
git remote add origin https://github.com/pedroobando/gitbasico.git
```

Graba los cambios en el repositorio...

```
git push -u origin main
```
