# Guia de Estudio para el Control de Versiones. 

Guia de Estudio de la parte de Gestión de la Documentación - Control de Versiones. Indica qué tenemos que saber y saber hacer en la asignatura de Proyectos de Sistemas Electrónicos. 

## Conceptos mínimos que tenemos que saber sobre el control de versiones
* Definir brevemente en qué consiste el control de versiones.
---    
Sistema que registra los cambios que ha sufrido un fichero, de manera que se pueda recuperar cualquier versión pasada si fuera necesario compuesto normalmente de un servidor y un cliente.
* Explicar los siguientes conceptos: repositorio local, copia local, repositorio remoto, *log*, conflicto.
---
	-repositorio local (Local Repository): base de datos centralizado donde se guardan las distintas versiones de los ficheros sometidos a control de versiones
	-copia local: (working copy): Es la copia que hacen los usuarios de un fichero sometido a control de versiones. todas las copias locales son contenidas en el DIRECTORIO LOCAL (working directory/working tree/workspace).
	-repositorio remoto:  versiones del proyecto almacenadas en Internet o en cualquier otra red.
	-Log o historico: Registro de todos los cambios que se han producido en el repositorio. 
	-conflicto: Problema que surge cuando los clientes realizan cambios incompatibles entre sí.

* Explicar los siguientes estados de un fichero: sin seguimiento, confirmado, modificado, preparado, ignorado. 
* Explicar las siguientes operaciones: Clone, Add, Commit, Push, Pull, Fork y Pull Request. 
---
	-Clone: Replica un repositorio entero con todo su historial de cambios y actualiza el directorio local
	-Add: Realiza una copia de un fichero modificado, poniéndola en la zona de preparación para poder ser confirmada. 
	-Commit: Confirmar los ficheros preparados para su almacenamiento en el repositorio.
	-Push: Es la operación en la que se envían al repositorio centralizado (remoto) un commit o conjunto de commits, incluido una rama entera.
	-Pull: Es la operación en la que se actualiza el repositorio local y el directorio local con commits que provienen del repositorio remoto.
	-Fork: Clone que se hace dentro del mismo servidor. Por ejemplo, el repositorio original y el clonado ambos residen en (xej)GitHub…
	-Pull Request: (entre repositorios): Petición que hace el desarrollador de que los cambios hechos en su repositorio clonado mediante un FORK sean incorporados al repositorio original

* Traducir entre inglés y español la terminología de los tres puntos anteriores. 
* Nombrar al menos dos servicios de repositorio remoto para el control de versiones.
---
GitHub y GuitLab 
* Nombrar al menos un cliente gráfico (GUI) para el control de versiones.
---
Git Force 

## Qué tenemos que saber hacer con Git (y GitHub)

### En el intérprete de comandos de git-bash
* Mostrar en qué directorio estamos.
---
pwd
* Crear un directorio.
---
mkdir <dir>
* Cambiar de directorio.
---
cd <dir>
* Mostrar la lista de ficheros de un directorio. 
---
ls [-l] [-a]
* Borrar un fichero.
--- 
rm <file>
* Cambiar (mover) un fichero de directorio.
---
mv <source> <dest>

### En control de versiones local 
* Crear un repositorio local en nuestra máquina.
---
git init 
* Preparar ficheros para ser confirmados en un repositorio local.
---
git add <file/files>
* Confirmar cambios en un repositorio local. 
---
git commit
* Deshacer la operación de preparar. 
---
git reset
* Deshacer la operación de confirmar.
---
git reset --hard o --soft
* Identificar el estado de un fichero o ficheros en un repositorio local.
---
git status
* Descartar los cambios de un fichero de trabajo mediante la recuperación de una versión almacendada en el repositorio local.
---
git restore
* Crear una rama en un repositorio local.
---
git branch <nombre>
* Cambiar de rama en la copia local.
---
git switch <nombre>

### En control de versiones centralizado
* Configurar git para que trabaje tras un proxy
---
git config --global http.proxy http://proxy.user:proxy.pass@proxy.name_or_ip:proxy.port proxy.user es el usuario que tiene permiso para acceder al proxy. proxy.pass es la password de dicho usuario. proxy.name_or_ip es el nombre DNS o la dirección IP de la máquina que hace de proxy de internet. proxy.port es el puerto por el que se accede a comunicar con el proxy de internet. –global le indica a git que la configuración es propia del usuario y sirve para todos sus repositorios.
Para consultar el proxy configurado en git: git config --global --get http.proxy
Para borrar el proxy configurado en git: git config --global --unset http.proxy

* Replicar un repositorio remoto localmente en nuestra máquina.
---
git clone <repo>
* Repolicar un repositorio local en un servidor remoto.
---
git push -u origin main 
* Traer los cambios de un repositorio remoto a un repositorio local.
---
git pull origin <repo> 
* Resolver los conflictos que se puedan producir al traerse estos cambios. 
* Enviar los cambios de un repositorio local a uno remoto.
---
git push <repo>  
* Enviar una rama local al repositorio remoto.
* Incorporar a ramas locales cambios que se producen en el repositorio remoto.  
* Realizar un pull request entre dos ramas de un repositorio remoto. 

### En control de versiones distribuido

* Realizar un pull request entre dos repositorios que resultaron de un Fork.  
