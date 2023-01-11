### Chuleta de control de versiones con git
•	Definir brevemente en qué consiste el control de versiones: un sistema que registra los cambios que ha sufrido un fichero, de manera que se pueda recuperar cualquier versión pasada si fuera necesario.

•	Explicar los siguientes conceptos: repositorio local, copia local, repositorio remoto, log, conflicto.
-	repositorio local: carpeta o directorio en el disco duro de nuestro propio ordenador
-	copia local: copia que se realiza en una unidad de almacenamiento que está localmente conectada al equipo.
-	repositorio remoto: Los repositorios remotos son versiones de tu proyecto que están hospedadas en Internet o en cualquier otra red. Puedes tener  varios de ellos, y en cada uno tendrás generalmente permisos de solo lectura o de lectura y escritura.
-	Log: una grabación secuencial en un archivo o en una base de datos de todos los acontecimientos (eventos o acciones) que afectan a un proceso particular (aplicación, actividad de una red informática, etc.). De esta forma constituye una evidencia del comportamiento del sistema.
-	Conflicto: Surge un conflicto cuando dos ramas independientes han editado la misma línea de un archivo o cuando un archivo se ha eliminado en una rama, pero editado en la otra.

•	Explicar los siguientes estados de un fichero: sin seguimiento, confirmado, modificado, preparado, ignorado.
- sin seguimiento:  Un archivo que no se ha preparado o confirmado.
-	confirmado: significa que los datos están almacenados de manera segura en tu base de datos local.
-	modificado: significa que has modificado el archivo pero todavía no lo has confirmado a tu base de datos.
-	preparado: significa que has marcado un archivo modificado en su versión actual para que vaya en tu próxima confirmación.
-	ignorado: Un archivo que se le ha indicado explícitamente a Git que ignore.

•	Explicar las siguientes operaciones: Clone, Add, Commit, Push, Pull, Fork y Pull Request.
-	Clone: clone se utiliza para apuntar a un repositorio existente y clonar o copiar dicho repositorio en un nuevo directorio, en otra ubicación.
-	Add: la operación add añade un cambio del directorio de trabajo en el entorno de ensayo. De este modo, indica a Git que quieres incluir actualizaciones en un archivo concreto en la próxima confirmación.
-	Commit: El comando commit guardará todos los cambio hechos en la zona de montaje o área de preparación (staging area), junto con una breve descripción del usuario, en un "commit" al repositorio local.
-	Push: se usa para cargar contenido del repositorio local a un repositorio remoto. 
-	Pull: se emplea para extraer y descargar contenido desde un repositorio remoto y actualizar al instante el repositorio local para reflejar ese contenido.
-	Fork: sirve para crear una copia de un repositorio en tu cuenta de usuario. Ese repositorio copiado será básicamente un clon del repositorio desde el que se hace el fork, pero a partir de entonces el fork vivirá en un espacio diferente y podrá evolucionar de manera distinta, a tu propio cargo.
-	Pull Request: es una operación que consiste en una petición para integrar nuestras propuestas o cambios de código a un proyecto.

•	Traducir entre inglés y español la terminología de los tres puntos anteriores.
Clone=copiar, add=añadir, commit=confirmar, push=cargar, pull=actualizar, Fork= bifurcación, pull Request= una petición.

•	Nombrar al menos dos servicios de repositorio remoto para el control de versiones.
Git, CVS, Apache subversión (SVN), Mercurial, Monotone.

•	Nombrar al menos un cliente gráfico (GUI) para el control de versiones.
Git Force para Linux, GitHub o Sourcetree para Windows, GitBox para Mac, SmartGit (multiplataforma).


• Que tenemos que saber hacer con Git (y GitHub) 

-En el interprete de comandos de git-bash

•	Mostrar en que directorio estamos = pwd
•	Crear un directorio = mkdir + el nombre de la carpeta/archivo
•	Cambiar de directorio = cd + el nombre de la carpeta/archivo
•	Mostrar la lista de ficheros de un directorio = ls
•	Borrar un fichero = git rm + nombre
•	Cambiar (mover) un fichero de directorio =git  mv + origen + destino 

-En control de versiones local

•	Crear un repositorio local en nuestra máquina.  git init
•	Preparar ficheros para ser confirmados en un repositorio local= git add + nombre del fichero
•	Confirmar cambios en un repositorio local=
•	Deshacer la operación de preparar= git Reset + nombre del fichero
•	Deshacer la operación de confirmar= git checkout – nombre del fichero/ git restore + nombre del fichero 
•	Identificar el estado de un fichero o ficheros en un repositorio local= git status
•	Descartar los cambios de un fichero de trabajo mediante la recuperación de una versión almacendada en el repositorio local=
•	Crear una rama en un repositorio local= git Branch + nombre de la rama 
•	Cambiar de rama en la copia local= git switch + nombre de la rama

-En control de versiones centralizado



-En control de versiones distribuido




  
