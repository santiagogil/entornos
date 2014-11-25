# Arquitectura
## Base de datos
Dadas la naturaleza distribuida del sistema y la intermitencia en el servicio de conectividad en los establecimientos, resulta necesario implementar una base de datos capaz de sincronizar aún en situaciones de conectividad precaria.

**TRAES2** contará con una instalación de base de datos por dependencia más una central con fines estadísticos.
Este diseño permite que cada establecimiento pueda trabajar con o sin conección a la red contando con que se realizará una sincronización sin complicaciones al momento de recuperar la conectividad.

Toda la interacción de los usuarios será mediada por aplicaciones web basadas en HTML5, Javascript y CSS3 que contarán con una versión local de la base de datos. Esto brinda las mismas prestaciones de trabajo sin conección a nivel de usuario.
El usuario puede trabajar incluso fuera del establecimiento contando con que los datos se sincronizarán en cuanto retome la conección con la base de datos.

La base de datos elegida para cumplir con estos requerimientos es [Couchdb](https://couchdb.apache.org/) para los servidores y [Pouchdb](http://pouchdb.com/) para los clientes.

## Interfaces
Consistirán en aplicaciones web lado cliente, las cuales funcionarán enteramente en el navegador del usuario.
Esto elimina la necesidad de programar código del lado del servidor simplificando notáblemente la arquitectura.

### Módulos
Todo el código será desarrollado en forma modular basado en [CommonJS](http://wiki.commonjs.org/wiki/CommonJS),  sistema ampliamente difundido utilizado en [NodeJS](http://nodejs.org/).

	exports.hello = function() {
  		return 'Hello World'
	};


### Dependencias