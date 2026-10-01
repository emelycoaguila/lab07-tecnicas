# Bitacora de tecnicas avanzadas

Laboratorio 07: Tecnicas Avanzadas de Prompting.

Herramienta de IA usada: ChatGPT

## Ejercicio 2: Zero-shot, one-shot y few-shot
| Tipo | Aciertos (de 5) | Formato de la respuesta | Todas con el mismo formato (Si/No) |
|------|-----------------|-------------------------|------------------------------------|
| Zero-shot | 5 | Lista numerada | Sí |
| One-shot | 5 | Lista numerada | Sí |
| Few-shot | 5 | Texto -> etiqueta | Sí |
## Ejercicio 3: Chain of Thought
| Pedido | Respuesta de la IA | Muestra los pasos (Si/No) | Correcta (Si/No) |
|--------|--------------------|---------------------------|------------------|
| Directo | 318.60 | No | Sí |
| Paso a paso | 318.60 | Sí | Sí |

- Ver los pasos es útil porque puedo comprobar cómo llegó la IA a la respuesta.
- También puedo encontrar más fácil en qué cálculo estaría el error si la respuesta fuera incorrecta.
## Ejercicio 4: Role prompting
| Version | Vocabulario (sencillo/tecnico) | Usa ejemplos o codigo | A quien le sirve mas |
|---------|--------------------------------|-----------------------|----------------------|
| A. Sin rol | Sencillo | Puede usar ejemplos | Persona que quiere una explicación general |
| B. Rol docente | Sencillo | Sí, ejemplos cotidianos | Principiantes |
| C. Rol senior | Técnico | Sí, puede usar código Java | Personas con conocimientos de programación |
- El rol cambia la forma en que la IA explica el mismo tema.
- El rol docente es más fácil de entender para alguien que recién empieza, mientras que el rol senior puede usar términos más técnicos.
## Ejercicio 5: Descomposicion
| Paso | Resultado obtenido |
|------|--------------------|
| 1 | La IA propuso 5 requisitos principales para el sistema de inventario. |
| 2 | La IA diseñó las clases necesarias y sus atributos con tipos de datos. |
| 3 | La IA generó la clase Producto con atributos, constructor, getters y setters. |
| 4 | La IA revisó la clase Producto y propuso 3 mejoras concretas. |
- Comparación: El pedido de una sola vez generó una respuesta más general. Al dividir la tarea en pasos, pude revisar cada parte y obtener un código más relacionado con los requisitos anteriores.
## Ejercicio 6: Prompt estructurado y autocritica
| Qué revisar | Cumple (Sí / No) |
|-------------|------------------|
| ¿Tiene las 4 columnas pedidas? | Sí |
| ¿Incluye el bloqueo después de 3 intentos? | Sí |
| ¿Incluye casos con campos vacíos? | Sí |
| ¿Indica qué casos agregó en la autocrítica? | Sí |
| ¿Hay algún caso repetido o que no tenga sentido? | No |
