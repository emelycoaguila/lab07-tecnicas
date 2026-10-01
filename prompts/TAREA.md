# Tarea: Mi prompt avanzado

## Tarea elegida
Elegí como tarea generar casos de prueba para un sistema de login. El sistema permite ingresar un correo y una contraseña y bloquea la cuenta después de 3 intentos fallidos.

Quise mejorar el prompt poco a poco para obtener casos de prueba más completos y ordenados.
## Version 1: prompt basico
Dame casos de prueba para un login.
Técnica agregada

En esta versión no agregué una técnica específica. Es un prompt básico y muy general.

¿Por qué?
Queria comprobar que respuestas obtenia solamente indicando la tarea.

¿Qué mejoró en la respuesta?

La respuesta podía dar algunos casos generales, pero podía dejar de lado casos importantes como campos vacíos, correo sin @, espacios en la contraseña o el bloqueo después de 3 intentos.
## Version 2
Actúa como analista de pruebas de software.

Genera 8 casos de prueba para un sistema de login que utiliza correo y contraseña. La cuenta se bloquea después de 3 intentos fallidos.

Presenta la respuesta en una tabla con estas columnas:
- Número
- Caso de prueba
- Datos de entrada
- Resultado esperado

Incluye casos correctos, incorrectos y casos límite.
Técnica agregada

Agregué role prompting y un formato estructurado.

¿Por qué?

El rol de analista de pruebas ayuda a enfocar la respuesta en pruebas de software. También definí una tabla para que los casos fueran más fáciles de revisar.

¿Qué mejoró en la respuesta?

Los casos fueron más específicos y organizados. Además, se incluyeron casos correctos, incorrectos y algunos casos límite.
## Version 3: prompt final
<rol> Actúa como analista de pruebas de software especializado en pruebas funcionales de aplicaciones web. </rol> <contexto> Estoy probando un sistema de login que permite ingresar correo y contraseña. La cuenta se bloquea después de 3 intentos fallidos consecutivos. </contexto> <tarea> Genera 10 casos de prueba para verificar el funcionamiento del login. Descompón la tarea considerando: 1. Inicio de sesión correcto. 2. Datos incorrectos. 3. Campos vacíos. 4. Formato del correo. 5. Espacios en los datos. 6. Límite de 3 intentos fallidos. 7. Intento de acceso después del bloqueo. </tarea> <ejemplos> Ejemplo de caso: Caso: Inicio de sesión correcto. Entrada: correo válido y contraseña válida. Resultado esperado: El usuario ingresa al sistema. Ejemplo de caso: Caso: Correo sin @. Entrada: usuarioejemplo.com y contraseña válida. Resultado esperado: El sistema rechaza el correo e indica que el formato no es válido. </ejemplos> <revision> Antes de entregar la respuesta, revisa que los casos incluyan datos válidos, datos inválidos y casos límite, especialmente los relacionados con los 3 intentos fallidos y el bloqueo. </revision> <formato> Presenta los resultados en una tabla con las columnas: Número | Caso de prueba | Datos de entrada | Resultado esperado Después de la tabla, agrega una lista corta indicando qué casos corresponden a casos límite. </formato>

## Tecnicas usadas en el prompt final
| Técnica | Parte del prompt final | ¿Para qué se utilizó? |
|---------|-------------------------|------------------------|
| Role prompting | `<rol>` | Indicar que la IA actúe como analista de pruebas de software. |
| Descomposición | `<tarea>` | Dividir la tarea en diferentes situaciones del login. |
| Few-shot | `<ejemplos>` | Mostrar ejemplos del tipo de casos que se esperan. |
| Autocrítica | `<revision>` | Revisar que no falten casos importantes. |
| Prompt estructurado | `<rol>`, `<contexto>`, `<tarea>`, `<ejemplos>`, `<revision>`, `<formato>` | Organizar las instrucciones de manera clara. |
## Evaluacion del resultado
| Criterio | Resultado |
|----------|-----------|
| Incluye casos correctos e incorrectos | Sí |
| Incluye campos vacíos | Sí |
| Incluye correo con formato inválido | Sí |
| Incluye casos límite | Sí |
| Considera los 3 intentos fallidos | Sí |
| Considera el bloqueo de la cuenta | Sí |
| Presenta los casos en una tabla | Sí |
| Tiene un rol específico | Sí |
## Por que elegi estas tecnicas
Elegí estas técnicas porque la tarea necesita casos de prueba completos y ordenados. El role prompting ayuda a definir el tipo de respuesta, la descomposición permite separar las diferentes situaciones del login y el few-shot ayuda a mostrar ejemplos. También usé autocrítica para revisar que no falten casos importantes y el prompt estructurado para organizar mejor todas las instrucciones. No usé otras técnicas porque estas eran suficientes para mejorar la respuesta de esta tarea.