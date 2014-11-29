# Workflow
## Módulos nuevos
1. Primero que nada realizamos una investigación rápida para determinar si estamos por resolver un problema que ya estaba resuelto.
Nuestra primera opción de búsqueda debería ser el repositorio de npm.
Por ejemplo, si estamos por crear un módulo que interactúa, de alguna manera con Pouchdb.
		npm search pouchdb | more

	Nos daría la siguiente salida

		NAME                               DESCRIPTION                                                  AUTHOR               DATE       VERSION     KEYWORDS                     
                                                                 
		add-cors-to-couchdb                add CORS to couchdb                                          =cwmma =nolanlawson  2014-10-24 0.0.3       cors couchdb pouchdb         
                                                                 
		americano-cozy-pouchdb             Americano helpers to build Cozy applications faster with…    =mycozycloud         2014-09-24 0.3.16      plugin cozy pouchdb americano
                                                                 
		ampersand-collection-pouchdb-mixin A mixin for extending ampersand-collection with pouchdb…     =svnlto              2014-10-06 0.1.2       backbone sync pouchdb ampersand                                                               
		ampersand-model-pouchdb-mixin      A mixin for extending ampersand-model with pouchdb…          =svnlto              2014-09-20 0.1.1       model, ampersand, state      
                                                                 
		ampersand-pouchdb-sync             AmpersandJS PouchDB Sync Adapter                             =svnlto              2014-09-02 0.1.1       backbone sync pouchdb ampersand                                                               
		backbone-pouch                     Backbone PouchDB Sync Adapter                                =jo                  2014-07-07 1.4.0       backbone sync adapter pouchdb
                                                                 
		backbone-pouch-collection          Backbone Collections with PouchDB as the data source         =klaemo              2014-06-17 0.3.1       pouchdb couchdb backbone collection                                                           
		couchdb-eval                       Compiles a piece of code to a function object, providing a…  =commandoline        2014-09-01 1.0.4       pouch pouchdb couch couchdb eval                                                              
		couchdb-objects                    Aids in the construction of JSON objects as used by CouchDB. =commandoline        2014-09-01 1.0.4       pouch pouchdb couch couchdb object                                                            
		couchdb-render                     Given the code of a CouchDB show/list function (and some…    =commandoline        2014-09-01 1.0.0       pouch pouchdb couch couchdb render showlist                                                  
		couchdb-resp-completer             Builds a complete CuchDB-like response object from a very…  =commandoline        2014-09-01 1.0.0       pouch pouchdb couch couchdb response object                                                   
		cozy-pouchdb-clearance             cozy-pouchdb-clearance provides clearance management for…    =mycozycloud         2014-08-11 0.1.13      cozy clearance               
                                                                 
		delta-pouch                        Conflict-free collaborative editing for PouchDB              =redgeoff            2014-09-26 0.1.7       pouch pouchdb plugin delta partial updates couch couchdb
		dimensional_pouch                  Stay synchronized with a remote CouchDB instance,…           =justicefries        2014-10-15 1.0.0       pouchdb                      
                                                                 
		ember-pouch                        PouchDB adapter for Ember Data                               =nolanlawson         2014-11-19 1.1.1       Ember Data adapter PouchDB CouchDB                                                            
		express-pouchdb                    Express submodule with a CouchDB style REST interface to…    =nick-thompson…      2014-10-29 0.7.2                                    
                                                                 
		factoryng                          An all-in-one angularjs factory that wraps multiple backends =redgeoff            2014-11-06 0.0.11      angular angularjs factory binding pouch pouchdb delta-pouch delta pouch couch couchdb firebase
		filter-pouch                       Filter Pouch - a PouchDB plugin for filtering documents      =nolanlawson…        2014-11-25 1.0.0       pouch pouchdb plugin filter couch couchdb                                                     
		generator-angular-pouchdb          Yeoman generator for angular-pouchdb directives              =tlvince             2014-08-07 0.1.0       yeoman-generator angular pouc
		--Más--

2. Si encontramos módulos similares, analizamos de qué manera resuelven el problema, qué podemos aprender de cómo lo resuelven y en qué se diferencia nuestra propuesta.
3. El siguiente paso es clonar nuestro repositorio de ejemplo, lo cuál nos va a ahorrar buena parte del trabajo necesario para iniciar un módulo respetable. (Para más información ver [Repositorio de ejemplo](/repositorio/README.html)).

		git clone https://github.com/PCI-TDF/modulodeejemplo.git nombreDelNuevoModulo
4. Nos movemos al directorio modulodeejemplo e instalamos las dependencias de desarrollo.
    
		npm install
5. Una vez instaladas las dependencias modificamos en el archivo `package.json` los siguientes datos:
		{
    	"name": "",
    	"version": "",
    	"homepage": "",
    	"description": "",
    	"main": "",
    	"bin": {
        "gitbook": "" // archivo que funciona como punto de entrada del módulo.
    	},
    	"repository": {
        
        "url": "" // url desde la que se puede clonar el repositorio.
    	},
    	"keywords": [
    
    	],
    	"author": " <email>",
    	"bugs": {
        "url": "" // url que apunta a los issues del repositorio en Github.
    	},
    	"contributors": [
        {
            "name": "",
            "email": ""
        }
    	]
		}



1. Determinar si se va a trabajar sobre un módulo existente o uno nuevo.
2. Se crea un branch con un nombre descriptivo. `git checkout -b nomredescriptivo`.
3. Se escribe la documentación especificando parámetros y valores de retorno con sus tipos. En lo posible se agregan ejemplos de uso.
4. Se escribe un test que comprobará el funcionamiento del nuevo código.
5. Se escribe el código iterando hasta que pase el test, verificando que cumpla con lo especificado en la documentación.
6. Se corrige la historia para evitar contaminar la historia del proyecto con mensajes de commit poco descriptivos e intentos fallidos.
7. Se realiza el merge.
8. Se publica un pull request mencionando a quién revisará el código.

**Saltos de versión?**