# Repositorio de referencia
* Plantilla readme.
* Browserify.
* Beefy.
* Tape.
* Testling.
* JsDoc.
* Scripts.
* JsHint.
* JsSc.
* RetireJs.
* Ghooks.
* Readmetree.
* Mdlint.
* Shrinkwrap.
* Licencia.
* License footprint.
* JsSc JsDoc.

? Testlingify y Travisify
* [ ] blah

## Scripts

_Aprovechando la facilidad de npm para correr scripts personalizados, este repositorio cuenta con una serie de tareas preconfiguradas que lo convierten en un completo entorno de desarrollo._
### Test

    npm test

Corre tape via testling para todos los archivos de la carpeta ./tests

### Valida

    npm run valida

Verifica la calidad de todos los m&oacute;dulos mediante jscs (normas de estilo) y jshint (linter).

### Docs

    npm run docs

Compila toda la documentaci&oacute;n incluida en el c&oacute;digo utilizando jsdocs.

### Desarrollo

    npm run desarrollo

Levanta en paralelo los servidores de aplicaci&oacute;n, documentaci&oacute;n, tests y autoayuda con live reload.

### Build

    npm run build

Compila la aplicaci&oacute;n, la documentaci&oacute;n y los tests a sus respectivas carpetas de producci&oacute;n.


### Vulnerabilidades
       
    npm run vulnerabilidades

Ejecuta retire en la carpeta raiz del proyecto devolviendo notificaciones con links a los detalles de todas las vulnerabilidades conocidas en las dependencias del proyecto.

### Autoayuda

    npm run autoayuda

Corre readmetree en la carpeta root del repositorio levantando un servidor que permite navegar todos los readme de todas las dependencias.

## Seguimiento de tickets

Para facilitar el seguimiento de tickets de todo el proyecto utilizamos un fork traducido al castellano de Uberstich.
[Tickets](http://pci-tdf.github.io/ubersicht/?showOpen=true&showClosed=true&showCommented=true&showUncommented=true&last24Hours=false&repos=repositorio-de-referencia&labels=null&milestones=null&usernames=null#santiagogil)

## Somos &aacute;giles

Se puede acceder al tablero kamban del proyecto en [Hubboard](lkjlj).
