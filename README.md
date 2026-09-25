# MyBash
> Desarrollado por Facundo Palacio, Tomás Morcos y Milagros Vera para el cursado de Sistemas Operativos 2025, LCC, FaMAF.
## Concepto
El repositorio provee una shell interactiva estilo Bash, con funcionalidad para la ejecución de cualquier programa en el sistema.
### Compilación
Desde el root del repositorio, correr:
```sh
make
```
Esto generará el binario ejecutable `mybash`.
### Ejecución
Desde el root del repositorio, correr:
```sh
./mybash
```
Esto abrirá la shell interactiva.
### Estructura del proyecto
El repositorio consiste de los siguientes módulos:
* `mybash`: Implementa el loop de la shell interactiva.
* `command`: Implementa los TADs utilizados (`scommand`, un comando simple con redirecciones; `pipeline`, un caño de comandos simples).
* `parsing`: Implementa la lógica para parsear entrada por terminal y devolver la estructura `pipeline` correspondiente.
* `builtin`: Implementa la ejecución de comandos propios de la shell (por ejemplo, `cd`).
* `execute`: Implementa la ejecución de comandos en el sistema.
* Varios archivos provistos por la cátedra para manejo de strings, parsers, etcétera.
### Trabajo en equipo
Para `command`, pensamos juntos cómo implementar la interfaz de los TAD. Usamos Git para trabajar por separado, haciendo aportes intercalados. Además estuvimos en constante comunicación, vá­a presencial y virtual sincrónica, de modo que todo el trabajo estuvo integrado.
Para la entrega final, la idea era repartirnos distintos módulos para el trabajo, y al principio así­ lo hicimos. Tomás se encargó de `mybash`, Milagros, de `builtin`, y Facundo, de `execute`. Pero, para el módulo `parsing`, todo el grupo volvió a la metodología anterior, intercalando commits sobre lo pensado grupalmente.
### Declaración de uso de IA
Se utilizó IA principalmente para la comprensión de los conceptos y para debuggear. En particular, se utilizó IA:
* Para entender varios conceptos relacionados al módulo `execute`
* Para entender varios conceptos relacionados al módulo `parsing`
* Para entender el uso del TAD `GQueue` de la GLib
* Para debuggear todo el proyecto.
