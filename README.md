## Empenzando
README
| Empezando con Git |
| ------------- |
| Descargamos Git|
| https://git-scm.com|
| Next - Next - Next|
| Windows Explorer integration|
| Git Bash Here|
| Git GUI Here|
| Next - Next - Next|
| Use the OpenSSL Library|

# Comandos
| Version |
| ------------- |
| Comandos|
| Verificar la version de Git |
| git --version |
| git help |
| git help commit => sabemos la funcionalidad |

# Configurar Git
| Funcionalidades |
| ------------- |
| git config --global user.name|
| git config --global user.email|
| ===> Verificar  => |
| git config --global -e|
| ===> Salir|
| :q + Enter|
| http://www.initializr.com/|

# Reconstruir proyecto 
| Comando | Descripción |
| ------------- | ------------- |
| git init  | Iniciar el proyecto (Repositorio Local)|
| git status  | Ver el estado de los archivos|
| git add . | Agregar todos los archivos|
| git commit -m "Primer Commit" | Toma un snapShot|
| git checkout -- . | Si por accidente daño algo el me sirve el siguiente comando|
| git add README.md | Si solo quiero agregar un solo archivo|

# Agregar todo al repo
| Comando | Descripción |
| ------------- | ------------- |
| git remote add origin https://github.com/cafajardop/AprendiendoGit.git | agregar al repositorio|
| git push -u origin master | Comando para guardar todo el proyecto |

# Ver un commit en particular
| Comando | Descripción |
| ------------- | ------------- |
| git log | Siempre se ven del mas nuevo al mas viejo|
| git config core.autocrlf true | Siempre se ven del mas nuevo al mas viejo|

# Si quiero agregar varios archivos que terminen en una extesion .png ejemplo
| Comando | Descripción |
| ------------- | ------------- |
|git add *.png | Con este comando agrego al stage solo los cambios que halla hecho con la extesion png|

# Mas comandos
| Comando | Descripción |
| ------------- | ------------- |
| git add css/ | Si quiero agregar todos los archivos que esten en la carpeta de css ejemplo|
| git commit -m "Agregando CSS" | Puedo hacer commits por separado |
| git reset *.xml | Si quiero agregar pero omitir algun archivo ejemplo xml|
| git add "*.txt" | Agrega todos los txt de todo el proyecto|
| git add *.txt | Agrega todos los txt del directorio actual|
| git add --all | Agrega todos los si excepción es muy parecido al git add .|
| git add <lista de archivos> | Agrega los archivos que listemos|
| git add pdfs/*.pdf | Agrega todos los pdf's dentro de la carpeta pdf |
| git add pdfs/ | Agrega todos los archivos sin importar pero que esten en la carpeta pdfs|
| git log --oneline | Nos deja ver el log y los commit mas reducido|
| git log --oneline --decorate --all --graph | Nos deja ver el log de una manera mas elegante|
| git status -s | Solo nos deja ver los archivos modificados y cuales estan en el stage|
| git add css/ | agregando una carpeta|
| git status -s | vemos cual se agrego y se ve en verde|
| git status -s -b | Nos indica la rama|

# Alias y salida del 
| Comando | Descripción |
| ------------- | ------------- |
| git config --global alias.lg "log --oneline --decorate --all --graph" | Colocar alias | 
| git lg | cuando ejecute  ejecuta todo el comando anterior y lo deja com alias |
| git config --global alias.s "status -s -b" | Alias(s) para git status -sb => sb significa stage branch |
| git s | sirve para modificar el alias|
| git config --global -e | configurar global |
| git config --global -l | este es un poco mas seguro| 
| esc +  :wq | salimos |

# Quiz 1
| Pregunta | Respuesta |
| ------------- | ------------- |
| 1-Cuando utilizamos Git, ¿Todos los miembros del equipo tienen una copia del repositorio cental?| Verdadero|
| 2-¿Un commit en Git, es como una fotografía del proyecto en ese momento?| Verdadero| 
| 3-¿Para qué sirve el comando git init ?|Para inicializar el repositorio|
| 4-Localmente, ¿Dónde se encuentra la carpeta que permite controlar todo nuestro repositorio de git?| En la carpeta .git|
| 5-Si queremos eliminar git de nuestro repositorio, ¿qué debemos hacer?| Borrar la carpeta .git |
| 6-¿Qué es el stage o el escenario?| Es un lugar donde pdemos confirmar los archivos y carpetas que conformaran el commit|
| 7-El comando git s , ¿Es propio de Git?| Falso |

# Quiz 2
| Pregunta | Respuesta |
| ------------- | ------------- |
| 1-¿Una rama se puede definir como una linea del tiempo de commits? | Verdadero |
| 2-Cuando aparece la palabra Fast Forward  después de un merge, ¿Qué significa?| Unio sin problemas ya que no existian commits en la rama a la cual unimos los cambios|
| 3-En un merge, ¿Git siempre intentará resolver los merge de forma automática?| Verdadero (Intentará hacerlo, pero si detecta conflictos, nos pedirá que los corrijamos.)|
| 4-Qué significa el siguiente mensaje en consola? ?? Historial.md | El archivo historia.md actualmente no se le esta dando un |seguimiento en el repositorio
| 5-Cómo creamos una nueva rama? | git branch rama | 

# Quiz 3
| Pregunta | Respuesta |
| ------------- | ------------- |
| ¿Para qué sirve el stash?| Sirve para colocar el trabajo actual, en un espacio temporal para posteriormente retomarlo |
| ¿Qué significa WIP cuando realizamos un git stash ?| Work in progress|
| ¿Cómo puedo ver todos los trabajos pendientes en el stash?| git stash list|
| ¿Cómo puedo recuperar el trabajo del stash?| git stash pop |
| ¿El git rebase, nos puede servir para actualizar el punto de separación de una rama? | Verdadero |
| ¿Qué puede hacer un rebase interactivo? | Puede unir dos o mas commits en un unico commit puede re-ordenar commits, corregir mensajes de commits par separar commits|

# Devolvere en el tiempo
| Comando | Descripción |
| ------------- | ------------- |
| git diff | vemos el historial de cambios|
| git add -A | Colocamos todos los archivos en el escenario|
| git s | guardarlo en el stage => recordar como hice el alias|
| git diff --staged | sabemos que diferencia hay con el staged|

# Salir del stated
| Comando | Descripción |
| ------------- | ------------- |
| git reset HEAD README.md|Como salirme del staged es decir no grabar aun por que me arrepenti|
| git s |verificamos|
| git checkout -- README.md | Devolverme por completo |

# Revertir Commits 
| Comando | Descripción |
| ------------- | ------------- |
| git commit -am "Readme actualiz" | Para agregar todos los elementos al staged|
| git commit --amend -m "Actualizamos el readme" | suponiendo que me equivoque entonces|
| git lg | verifcar log| 
| git reset --soft HEAD^ | Pero o sorpresa que se me olvido hacer algo en el mismo commit pues puedo modificar ese commit Recordar que el HEAD hacer referencia al commit que estamos modificando alt + 94 ^ ya nos habilita el commit en donde estabamos haciendo los ajustes y luego |
| git commit -am "Actualizamos el readme con todos los archivos a omitir"| Finalizar commit |

===================Preparando Repos para viajes en el tiempo============
==>Clase 21  Min 2:20
git lg
Hacemos un cambio normal 
git add -A
Verfiicamos si ya esta en el staged
git s
luego hacemos un git commit solo puedo escribir un mensaje multilinea y puedo editarlo y nos vamos hacia arriba y escribimos lo que deseemos
git commit 
Luego Salimos con el botón de escape
esc +  :wq

git lg nos muestra los id's
=> Esta es una forma 
git reset --soft c6c9af9
=> La otra para movernos en el tiempo
git reset --mixed d4456a9
=> Pero si quiero moverme al punto de la historia
git reset --hard d4456a9
=> Pero con el reflog
git reflog
podemos traer toda la historia y devolvernos asi hallamos hecho el hard 
=> y con el reset hard
git reset --hard d4456a9 => me puede devolver en el tiempo y el reflog lo que hace es mostrar todos los cambios

=======================Renombrar el archivo=====================
Creamos un archivo cualquiera y lo que vamos a hacer es renombrarlo para eso utilizamos
git mv destruir-mundo.txt salvar-mundo.txt
Automaticamente lo cambia
R  destruir-mundo.txt -> salvar-mundo.txt
git commit -m "Renombrando archivo salvar mundo"
Ahora vamos a eliminar el archivo con rm (remove)
git rm salvar-mundo.txt
Con git s  => verificamos el staged
git s
ahora vamos a decirle que si deseamos borrarlo para eso
git commit -m "Borrando archivo salvar"

=========Cambiar Nombre y Eliminar Archivos fuera de git=============
git add -u => actualizo
=== Ignorar archivos que no queremos
Si no quiero un archivo ejemplo un log
Si no existe el .gitignore

====================RAMAS====================
Posibles escenarios de un merge
FastFoward  => Git detecta que no hay ningun cambio en la rama principal y se unen como si nunca se hubiesen separado
Uniones Automáticas => Si no hay problemas git lo hace sin ningún problema
Union Manual => Git no puede arreglar el problema
========FastFoward
Para crear una rama 
git branch rama-villanos
Posterior debemos hacer un git checkout 
git checkout rama-villanos
Con git branch verifico en que rama estoy luego procedemos a hacer
git s
Para agregar todo
git add -A
El commit
git commit -m "Agregando Villanos"
Para saber las diferencias entre ramas
git diff rama-villanos master
Para unirnos debemos estar en nuestra rama principal de master 
git checkout master
Recordar que el HEAD hace referencia al ultimo commit que hicimos
Para unirnos hacemos 
git merge rama-villanos
Ya una vez hacemos el merge debemos eliminar la rama villanos
podemos ver las ramas asi 
git branch
Unificar 
git branch -d rama-villanos

========Unión Automática
Creamos la rama
git checkout -b rama-villano
Hacemos un commit
git commit -am "Agreamos algo"
Para fucionar
git merge rama-villano

========Unión Conflictos  SIEMPRE DEBO ESTAR EN MASTER PARA UNIR LAS RAMAS
Creamos la rama
git checkout -b rama-conflictos
Mofidicamos y hacemos commit
git commit -am "Modificamos algo"
Vamoa a master => es decir hacemos ese cambio 
git checkout master
Ahora vamos a hacer el merge
git merge rama-conflicto
Hacemos el git s
git s
luego resolvemos los conflictos y ejecutamos el siguiente codig
git commit -am "Resolviendo conflictos"

========Eliminar Ramas
git branch -d rama-conflicto
git branch -d rama-villano
Luego nos vemos en la master
git branch 

========Agregar Tags
Creamos tag
git tag superRelease
Verificamos tag
git tag
Borrar tag
git tag -d supeRelease

========Agregar Tags con mas modificaciones
Agregamos tag
git tag -a v1.0.0 -m "Versión 1.0.0"
Verificar tag
git tag

========Agregar Tags en un Hash especifico en el tiempo
Agregamos tag
git tag -a v0.1.0 d4456a9 -m "Version alfa"
Para ver tag
git show v0.1.0


=======Stash
Sirve para guardar mis cambios 
git stash
para listar mis stash
git stash list => los salva en un stage temporal
git stash
Para recuperar el stash
git stash pop
git stash -- git stash save Salva y restaura el último commit

git stash list --stat => podemos ver todos los stash y que se le hizo a cada
git show stash => nos muetra el stash tambien
git show stash@{1} nos muestra de manera detallada

Es bueno colocarle los mensajes a los stash
git stash save "Agregamos a loki en los villanos"

git stash clear borra todas las entradas en el stash

=======Git rebase Excelente comando
crea areas temporales sin afectar la rama master
- Ordenar commits
- Corregir mensajes de los commits
- Unir commits
- Separar commits
Sirven para evitar conflictos en los merges
ver video 38 