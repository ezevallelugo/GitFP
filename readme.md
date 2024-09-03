# Git Desarrollo Colaborativo

Esto es una guia para los alumnos de la capacitacion de **sistemas de control de versiones** que cursan los dias _lunes miercoles y viernes de 14hs a 17hs_

## Areas de GIT
- **Working Directory**: Corresponde a la carpeta donde inicializamos el repositorio, muy rara vez utilizaremos la consola por aqui.
    * __git init__: inicializa el repositorio de git
    * __git config user.name `<username>`__: define el nombre de usuario para el repositorio.
    * __git config user.email `<email>`__: establece el correo de contacto para el repositorio.
    * __rm -rf `.git`__ elimina el repositorio de git
- **Staging Area (INDEX)**: El area de control de cambios es la encargada de realizar el seguimiento a los archivos del proyecto, aqui se realizan las capturas (SNAPSHOT)
    * __git status__: muestra el estado de los archivos comparandolos con la ultima captura de codigo realizada.
    * __git diff__: muestra las diferencias de codigo con respecto a la ultima captura registrada en el INDEX
    * __git add `<file>`__: agrega los cambios del archivo al area de control de cambios mediante una captura.
- **Repository (Local)**: El almacen local, corresponde a la carpeta donde se guardan las capturas en formato BLOB, utilizan una estructura hexadecimal.
    * __git commit__: abre el editor para emitir una confirmacion de los cambios realizados.
    * __git log__: muestra el registro de confirmaciones realizadas en formato de commits.
    * __git push__: envia los cambios locales a la rama correspondiente de repositorio remoto.
    
## Configuracion inicial
Antes de trabajar en un proyecto es importante que configuremos nuestro nombre de usuario y correo con el que seremos identificados en los diferentes proyectos. Para ello utilizaremos los siguientes comandos
```sh
    git config --global user.name "username"
    git config --global user.email "user@server"
```