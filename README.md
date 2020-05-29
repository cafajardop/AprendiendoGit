# Empenzando
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

## Comandos
| Version |
| ------------- |
| Comandos|
| Verificar la version de Git |
| git --version |
| git help |
| git help commit => sabemos la funcionalidad |

## Configurar Git
| Funcionalidades |
| ------------- |
| git config --global user.name|
| git config --global user.email|
| ===> Verificar  => |
| git config --global -e|
| ===> Salir|
| :q + Enter|
| http://www.initializr.com/|

## Reconstruir proyecto 
| Comando | Descripción |
| ------------- | ------------- |
| git init  | Iniciar el proyecto (Repositorio Local)|
| git status  | Ver el estado de los archivos|
| git add . | Agregar todos los archivos|
| git commit -m "Primer Commit" | Toma un snapShot|
| git checkout -- . | Si por accidente daño algo el me sirve el siguiente comando|
| git add README.md | Si solo quiero agregar un solo archivo|

## Agregar todo al repo
| Comando | Descripción |
| ------------- | ------------- |
| git remote add origin https://github.com/cafajardop/AprendiendoGit.git | agregar al repositorio|
| git push -u origin master | Comando para guardar todo el proyecto |

## Ver un commit en particular
| Comando | Descripción |
| ------------- | ------------- |
| git log | Siempre se ven del mas nuevo al mas viejo|
| git config core.autocrlf true | Siempre se ven del mas nuevo al mas viejo|

## Si quiero agregar varios archivos que terminen en una extesion .png ejemplo
| Comando | Descripción |
| ------------- | ------------- |
|git add *.png | Con este comando agrego al stage solo los cambios que halla hecho con la extesion png|

## Mas comandos
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
| git remote -v | ver el enlace de la rama|
| git pull | Descargamos cambios |

## Alias y salida del 
| Comando | Descripción |
| ------------- | ------------- |
| git config --global alias.lg "log --oneline --decorate --all --graph" | Colocar alias | 
| git lg | cuando ejecute  ejecuta todo el comando anterior y lo deja com alias |
| git config --global alias.s "status -s -b" | Alias(s) para git status -sb => sb significa stage branch |
| git s | sirve para modificar el alias|
| git config --global -e | configurar global |
| git config --global -l | este es un poco mas seguro| 
| esc +  :wq | salimos |

## Quiz 1
| Pregunta | Respuesta |
| ------------- | ------------- |
| 1-Cuando utilizamos Git, ¿Todos los miembros del equipo tienen una copia del repositorio cental?| Verdadero|
| 2-¿Un commit en Git, es como una fotografía del proyecto en ese momento?| Verdadero| 
| 3-¿Para qué sirve el comando git init ?|Para inicializar el repositorio|
| 4-Localmente, ¿Dónde se encuentra la carpeta que permite controlar todo nuestro repositorio de git?| En la carpeta .git|
| 5-Si queremos eliminar git de nuestro repositorio, ¿qué debemos hacer?| Borrar la carpeta .git |
| 6-¿Qué es el stage o el escenario?| Es un lugar donde pdemos confirmar los archivos y carpetas que conformaran el commit|
| 7-El comando git s , ¿Es propio de Git?| Falso |

## Quiz 2
| Pregunta | Respuesta |
| ------------- | ------------- |
| 1-¿Una rama se puede definir como una linea del tiempo de commits? | Verdadero |
| 2-Cuando aparece la palabra Fast Forward  después de un merge, ¿Qué significa?| Unio sin problemas ya que no existian commits en la rama a la cual unimos los cambios|
| 3-En un merge, ¿Git siempre intentará resolver los merge de forma automática?| Verdadero (Intentará hacerlo, pero si detecta conflictos, nos pedirá que los corrijamos.)|
| 4-Qué significa el siguiente mensaje en consola? ?? Historial.md | El archivo historia.md actualmente no se le esta dando un |seguimiento en el repositorio
| 5-Cómo creamos una nueva rama? | git branch rama | 

## Quiz 3
| Pregunta | Respuesta |
| ------------- | ------------- |
| ¿Para qué sirve el stash?| Sirve para colocar el trabajo actual, en un espacio temporal para posteriormente retomarlo |
| ¿Qué significa WIP cuando realizamos un git stash ?| Work in progress|
| ¿Cómo puedo ver todos los trabajos pendientes en el stash?| git stash list|
| ¿Cómo puedo recuperar el trabajo del stash?| git stash pop |
| ¿El git rebase, nos puede servir para actualizar el punto de separación de una rama? | Verdadero |
| ¿Qué puede hacer un rebase interactivo? | Puede unir dos o mas commits en un unico commit puede re-ordenar commits, corregir mensajes de commits par separar commits|

## Devolvere en el tiempo
| Comando | Descripción |
| ------------- | ------------- |
| git diff | vemos el historial de cambios|
| git add -A | Colocamos todos los archivos en el escenario|
| git s | guardarlo en el stage => recordar como hice el alias|
| git diff --staged | sabemos que diferencia hay con el staged|

## Salir del stated
| Comando | Descripción |
| ------------- | ------------- |
| git reset HEAD README.md|Como salirme del staged es decir no grabar aun por que me arrepenti|
| git s |verificamos|
| git checkout -- README.md | Devolverme por completo |

## Revertir Commits 
| Comando | Descripción |
| ------------- | ------------- |
| git commit -am "Readme actualiz" | Para agregar todos los elementos al staged|
| git commit --amend -m "Actualizamos el readme" | suponiendo que me equivoque entonces|
| git lg | verifcar log| 
| git reset --soft HEAD^ | Pero o sorpresa que se me olvido hacer algo en el mismo commit pues puedo modificar ese commit Recordar que el HEAD hacer referencia al commit que estamos modificando alt + 94 ^ ya nos habilita el commit en donde estabamos haciendo los ajustes y luego |
| git commit -am "Actualizamos el readme con todos los archivos a omitir"| Finalizar commit |

## Pull Request
| Git | Descripción |
| ------------- | ------------- |
| Fork | Abrir una rama y clonar otro proyecto para posteriormente hacer un pull requests Clase 64|
| Pull request | Es cuando queremos modificar el proyecto de otra persona  Clase 65|
| Actualizando el Fork | Ver clase 67 los pasos del Fork|
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
git tag superRelease Creamos tag
git tag Verificamos tag
git tag -d supeRelease Borrar tag
git push --tags => sube todos los tags

========Agregar Tags con mas modificaciones
git tag -a v1.0.0 -m "Versión 1.0.0" | Agregamos tag
git tag | Verificar tag

========Agregar Tags en un Hash especifico en el tiempo
git tag -a v0.1.0 d4456a9 -m "Version alfa" | Agregamos tag
git show v0.1.0 | Para ver tag

=======Stash
git stash | Sirve para guardar mis cambios 
git stash list | para listar mis stash 
git stash | los salva en un stage temporal
git stash pop | Para recuperar el stash
--git stash save | Salva y restaura el último commit
git stash list --stash | podemos ver todos los stash y que se le hizo a cada
git show stash | nos muetra el stash tambien
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

# h1
## h2
### h3
#### h4
##### h5

Un **gran poder** requiere _una_ gran *responsabildad*
>Carlos Fajardo
## Listas ordenadas
1. item
2. item
3. item
  * subitem
  * subitem
  * subitem

![Batman](https://upload.wikimedia.org/wikipedia/en/1/19/Batman_%28circa_2016%29.png)
[ir a la imagen](https://upload.wikimedia.org/wikipedia/en/1/19/Batman_%28circa_2016%29.png)

[ir a Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
[ir a turorial markdown](https://www.markdowntutorial.com/)
[ir a emojis](https://www.webpagefx.com/tools/emoji-cheat-sheet/)


# Tips
```
command + P : Markdown Open Preview
command + P : Markdown Open Preview to the side

Ctrl + P : Markdown Open Preview
Ctrl + P : Markdown Open Preview to the side
```

# Dillinger

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)


Dillinger is a cloud-enabled, mobile-ready, offline-storage, AngularJS powered HTML5 Markdown editor.

  - Type some Markdown on the left
  - See HTML in the right
  - Magic

# New Features!

  - Import a HTML file and watch it magically convert to Markdown
  - Drag and drop images (requires your Dropbox account be linked)


You can also:
  - Import and save files from GitHub, Dropbox, Google Drive and One Drive
  - Drag and drop markdown and HTML files into Dillinger
  - Export documents as Markdown, HTML and PDF

Markdown is a lightweight markup language based on the formatting conventions that people naturally use in email.  As [John Gruber] writes on the [Markdown site][df1]

> The overriding design goal for Markdown's
> formatting syntax is to make it as readable
> as possible. The idea is that a
> Markdown-formatted document should be
> publishable as-is, as plain text, without
> looking like it's been marked up with tags
> or formatting instructions.

This text you see here is *actually* written in Markdown! To get a feel for Markdown's syntax, type some text into the left window and watch the results in the right.

### Tech

Dillinger uses a number of open source projects to work properly:

* [AngularJS] - HTML enhanced for web apps!
* [Ace Editor] - awesome web-based text editor
* [markdown-it] - Markdown parser done right. Fast and easy to extend.
* [Twitter Bootstrap] - great UI boilerplate for modern web apps
* [node.js] - evented I/O for the backend
* [Express] - fast node.js network app framework [@tjholowaychuk]
* [Gulp] - the streaming build system
* [Breakdance](http://breakdance.io) - HTML to Markdown converter
* [jQuery] - duh

And of course Dillinger itself is open source with a [public repository][dill]
 on GitHub.

### Installation

Dillinger requires [Node.js](https://nodejs.org/) v4+ to run.

Install the dependencies and devDependencies and start the server.

```sh
$ cd dillinger
$ npm install -d
$ node app
```

For production environments...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### Plugins

Dillinger is currently extended with the following plugins. Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| Github | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |


### Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantanously see your updates!

Open your favorite Terminal and run these commands.

First Tab:
```sh
$ node app
```

Second Tab:
```sh
$ gulp watch
```

(optional) Third:
```sh
$ karma test
```
#### Building for source
For production release:
```sh
$ gulp build --prod
```
Generating pre-built zip archives for distribution:
```sh
$ gulp build dist --prod
```
### Docker
Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```
This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out `${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

See [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)


### Todos

 - Write MORE Tests
 - Add Night Mode

License
----

MIT


**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
