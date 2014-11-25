# Workflow

1. Determinar si se va a trabajar sobre un módulo existente o uno nuevo.
2. Se crea un branch con un nombre descriptivo. `git checkout -b nomredescriptivo`.
3. Se escribe la documentación especificando parámetros y valores de retorno con sus tipos. En lo posible se agregan ejemplos de uso.
4. Se escribe un test que comprobará el funcionamiento del nuevo código.
5. Se escribe el código iterando hasta que pase el test, verificando que cumpla con lo especificado en la documentación.
6. Se corrige la historia para evitar contaminar la historia del proyecto con mensajes de commit poco descriptivos e intentos fallidos.
7. Se realiza el merge.
8. Se publica un pull request mencionando a quién revisará el código.

**Saltos de versión?**