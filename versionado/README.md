# Versionado

> ##Versionamiento Semántico 2.0.0-rc.2

> En el mundo de la gestión de software existe el temor de caer en algún momento en el llamado “infierno de las dependencias”. Mientras más grande crece tu sistema y mientras más paquetes integras en tu software, más probable es que te encuentres, un día, en este pozo de la desesperación.

> En sistemas con muchas dependencias, publicar nuevas versiones de un paquete puede transformarse rápidamente en una pesadilla. Si las especificaciones de dependencia son muy estrictas está el peligro del bloqueo de versiones (la imposibilidad de actualizar un paquete sin tener que actualizar todos los que dependen de este). Si las dependencias se especifican de manera muy amplia, inevitablemente caerás en promiscuidad de versiones (asumir más compatibilidad con versiones futuras de lo razonable). El infierno de las dependencias es donde te encuentras cuando el bloqueo de versiones o la promiscuidad de versiones te impiden avanzar en tu proyecto de manera fácil y segura.

> Como solución a este problema, propongo un set simple de reglas y requerimientos que dictan cómo asignar y cómo aumentar los números de versión. Para que este sistema funcione, tienes que declarar primero un API pública. Esto puede consistir en documentación o ser explicitado en el código mismo. De cualquier forma, es importante que esta API sea clara y precisa. Una vez que identificaste tu API pública, comunicas cambios a ella con aumentos específicos al número de versión. Considera un formato de versión del tipo X.Y.Z (Major.Minor.Patch) Los arreglos de bugs que no cambian el API incrementan el patch, los cambios y adiciones que no rompen la compatibilidad de las dependencias anteriores incrementan el minor, y los cambios que rompen la compatibilidad incrementan el major.

> Yo llamo a este sistema “Versionamiento Semántico”. Bajo este esquema, los números de versión y la forma en que cambian entregan significado del código que está detrás y lo que fue modificado de una versión a otra.



*Citado de la traducción de Agustin Feuerhake realizada sobre la especificación de Tom Preston-Werner.*
[Semver](http://semver.org/lang/es/)