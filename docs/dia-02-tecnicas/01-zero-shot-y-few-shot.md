# Zero-shot y few-shot

Zero-shot y few-shot son dos formas de proporcionar instrucciones a un modelo de lenguaje.

La diferencia principal está en si incluimos ejemplos de la tarea dentro del prompt.

En **zero-shot**, solicitamos el trabajo sin aportar demostraciones de entrada y salida.

En **few-shot**, añadimos unas pocas demostraciones para orientar cómo debe resolverse.

Ambas estrategias pueden utilizar instrucciones, contexto, restricciones y un formato explícito.

Ninguna garantiza por sí sola que el resultado sea correcto.

Esta unidad explica cuándo utilizar cada enfoque, cómo seleccionar ejemplos y cómo comparar sus resultados.

Trabajaremos principalmente con clasificación, extracción y transformación de textos.

El objetivo es aprender a tomar decisiones basadas en evidencias, no asumir que añadir ejemplos siempre mejora una respuesta.

!!! info "Alcance de la unidad"
    La sesión lectiva dura 1,5 horas.
    Esta página incluye documentación ampliada y prácticas opcionales.
    La actividad obligatoria consiste en comparar zero-shot y few-shot sobre una tarea controlada.
    Las ampliaciones pueden realizarse después o adaptarse al perfil del grupo.

## 1. Fundamentos: instrucciones, demostraciones y aprendizaje en contexto

Esta sección presenta los conceptos necesarios para distinguir ambos enfoques y comprender qué aportan los ejemplos.

### 1.1. Ficha de la unidad

La unidad pertenece al segundo día del curso.

| Elemento | Descripción |
|---|---|
| Jornada | Día 2 · Técnicas y formatos |
| Unidad | Zero-shot y few-shot |
| Duración | 1,5 horas |
| Modalidad | Explicación, demostración y práctica |
| Resultado | Comparación documentada de dos estrategias |

Se presupone que conoces la anatomía básica de un prompt.

No necesitas programar.

Una interfaz conversacional autorizada es suficiente.

Utilizaremos datos ficticios y reglas explícitas.

El trabajo puede realizarse individualmente o por parejas.

**La evaluación se centra en el diseño de la comparación y en la revisión de sus resultados.**

### 1.2. Objetivos de aprendizaje

Al finalizar podrás distinguir instrucciones y demostraciones.

También podrás seleccionar ejemplos que aporten información relevante.

Los objetivos son:

- Explicar qué significa zero-shot.
- Explicar qué significa few-shot.
- Redactar ambas versiones para una misma tarea.
- Separar ejemplos y entradas de evaluación.
- Identificar ejemplos ambiguos o incorrectos.
- Comprobar si los ejemplos mejoran el cumplimiento.
- Reconocer costes y limitaciones.
- Documentar una decisión de uso.

No se exige que few-shot obtenga mejores resultados.

Puede empatar o funcionar peor.

**Una comparación que contradice tu expectativa también es un resultado válido.**

### 1.3. Qué significa zero-shot

Zero-shot significa que no proporcionamos demostraciones de la tarea en el prompt.

El modelo recibe la instrucción y debe responder con la información disponible.

Puede recibir reglas muy detalladas.

Puede recibir un esquema de salida.

Puede recibir un documento que debe procesar.

Nada de eso convierte automáticamente la solicitud en few-shot.

Ejemplo:

```text
Clasifica la solicitud como Información, Incidencia o Sugerencia.
Devuelve únicamente la categoría.

Solicitud:
No puedo acceder al material.
```

Aquí hay una entrada que resolver, pero no una demostración resuelta.

**Zero-shot no significa “sin instrucciones” ni “sin contexto”.**

### 1.4. Qué significa few-shot

Few-shot incorpora unas pocas demostraciones de la tarea.

Normalmente cada demostración contiene una entrada y una salida esperada.

Ejemplo:

```text
Clasifica la solicitud.

Ejemplo:
Entrada: ¿Cuánto dura la sesión?
Salida: Información

Ejemplo:
Entrada: El enlace no funciona.
Salida: Incidencia

Entrada nueva: Sugiero añadir una práctica.
Salida:
```

Los ejemplos muestran asociaciones y convenciones de respuesta.

No existe un número universal que defina un buen conjunto.

**La utilidad depende más de lo que enseñan que de cuántos son.**

### 1.5. One-shot y otras denominaciones

One-shot designa una solicitud con una demostración.

Few-shot suele utilizarse para un conjunto pequeño de demostraciones.

Las denominaciones describen la configuración del prompt.

No son niveles de calidad.

Un ejemplo bien elegido puede ser suficiente.

Varios ejemplos redundantes pueden aportar poco.

| Enfoque | Demostraciones |
|---|---|
| Zero-shot | Ninguna |
| One-shot | Una |
| Few-shot | Unas pocas |

En esta unidad utilizaremos dos condiciones: ninguna demostración y cuatro demostraciones.

Otros números pueden explorarse en las ampliaciones.

**No interpretes el nombre de la técnica como una recomendación automática.**

### 1.6. Qué cuenta como demostración

Una demostración enseña una relación entre una entrada y una respuesta.

Debe estar identificada como ejemplo resuelto.

Una lista de etiquetas no es necesariamente una demostración.

Una definición de categorías tampoco lo es.

Un documento pendiente de resumir es una entrada de trabajo.

Un documento acompañado de su resumen puede ser una demostración.

Conviene distinguir:

- Reglas: explican qué hacer.
- Ejemplos: muestran una aplicación.
- Entrada nueva: contiene lo que debe resolverse.
- Salida: presenta el resultado.

Esta separación facilita revisar el prompt.

También evita que el modelo responda otra vez a los ejemplos.

**Una demostración debe tener una función reconocible.**

### 1.7. Aprendizaje en contexto

El término *in-context learning* describe la adaptación a información presentada dentro del contexto.

Las demostraciones pueden orientar la respuesta sin actualizar los parámetros del modelo durante esa interacción.

No estamos realizando un entrenamiento completo.

Tampoco estamos creando automáticamente una habilidad permanente.

El efecto depende de que la información esté disponible en el contexto utilizado.

Una conversación nueva puede no conservar esos ejemplos.

Una función de memoria de la aplicación es un mecanismo diferente.

No debemos confundir:

- Adaptación dentro del prompt.
- Historial de conversación.
- Memoria del producto.
- Ajuste de parámetros.

Estas diferencias afectan a la reutilización.

**Si necesitas que una demostración esté disponible, inclúyela en el diseño documentado.**

### 1.8. Few-shot no es fine-tuning

Fine-tuning modifica parámetros mediante un proceso de entrenamiento adicional.

Few-shot incorpora demostraciones durante el uso del modelo.

Ambas estrategias pueden relacionarse con una misma tarea.

Sin embargo, sus procedimientos y costes son distintos.

| Aspecto | Few-shot | Fine-tuning |
|---|---|---|
| Ubicación de ejemplos | Contexto | Datos de entrenamiento adicional |
| Cambio de parámetros | No por la interacción | Sí, mediante entrenamiento |
| Actualización | Editar el prompt | Ejecutar un proceso de ajuste |
| Persistencia | Depende del contexto | Depende del modelo ajustado |

Esta unidad no incluye fine-tuning.

No necesitas preparar un conjunto de entrenamiento.

Sí necesitas mantener demostraciones coherentes.

**Editar ejemplos dentro del prompt no equivale a reentrenar el modelo.**

### 1.9. Qué pueden enseñar los ejemplos

Los ejemplos pueden comunicar convenciones difíciles de describir brevemente.

Pueden orientar:

- Etiquetas.
- Estructura.
- Nivel de detalle.
- Tratamiento de ausencias.
- Aplicación de excepciones.
- Estilo.
- Límites de inferencia.

También pueden mostrar una decisión en un caso fronterizo.

Eso resulta útil cuando una regla admite interpretaciones.

Pero un ejemplo incorrecto puede enseñar una asociación equivocada.

Un ejemplo demasiado específico puede favorecer una copia superficial.

**Diseñar ejemplos implica decidir qué conducta queremos demostrar.**

### 1.10. Qué no garantizan los ejemplos

Los ejemplos no garantizan generalización.

El modelo puede copiar detalles que no debería conservar.

Puede privilegiar el último ejemplo.

Puede aplicar una categoría por semejanza superficial.

También puede ignorar una regla explícita.

Una respuesta puede cumplir el formato y equivocarse en el contenido.

La presencia de demostraciones tampoco garantiza seguridad.

Un documento malicioso sigue siendo contenido no confiable.

Por eso debemos comprobar:

- Exactitud.
- Cumplimiento.
- Robustez sobre variaciones.
- Fidelidad a las fuentes.
- Alcance.

**Los ejemplos son una ayuda de diseño, no una garantía de comportamiento.**

### 1.11. Cuándo comenzar con zero-shot

Zero-shot es una referencia inicial razonable cuando la tarea puede describirse con claridad.

Puede resultar suficiente para transformaciones habituales.

También facilita mantener prompts compactos.

Ventajas frecuentes:

- Menos contenido que revisar.
- Menor ocupación del contexto.
- Menos riesgo de contradicciones entre ejemplos.
- Edición más sencilla.
- Línea base fácil de interpretar.

Estas ventajas no implican mejor exactitud.

Si la salida incumple, debemos estudiar el fallo.

Puede faltar una regla.

Puede faltar una fuente.

**Antes de añadir ejemplos, identifica qué información necesitan aportar.**

### 1.12. Cuándo explorar few-shot

Few-shot puede ser útil cuando existen convenciones específicas.

También cuando una regla abstracta no comunica suficientemente una excepción.

Situaciones habituales:

- Etiquetas propias de una organización.
- Campos con tratamiento especial.
- Estilos muy concretos.
- Casos ambiguos.
- Formatos con convenciones particulares.
- Límites de inferencia difíciles de expresar.

Primero define la tarea.

Después selecciona demostraciones relevantes.

No añadas ejemplos solo porque la técnica parezca más avanzada.

La decisión debe considerar resultados y costes.

**Utiliza few-shot cuando puedas explicar qué enseñan las demostraciones.**

---

## 2. Diseño: construir demostraciones claras y comparaciones justas

Esta sección explica cómo redactar las dos condiciones y cómo evitar problemas que falsean la comparación.

### 2.1. Mantener una tarea común

Zero-shot y few-shot deben resolver la misma tarea.

La comparación pierde claridad si cambias también las categorías o la salida.

Mantén constantes:

- Acción principal.
- Datos nuevos.
- Reglas.
- Categorías.
- Formato.
- Restricciones.
- Criterios de aceptación.

La diferencia inicial será la presencia de demostraciones.

Si cambias más elementos, registra esa circunstancia.

No atribuyas entonces todo el efecto a few-shot.

La prueba puede seguir siendo útil, pero responde a otra pregunta.

**Una comparación justa empieza por definir qué variable cambia.**

### 2.2. Redactar una base zero-shot sólida

La condición zero-shot no debe ser deliberadamente deficiente.

Debe contener instrucciones suficientes para realizar la tarea.

Una base puede incluir:

```text
TAREA
Clasifica cada solicitud.

REGLAS
[Definiciones y prioridad]

SALIDA
Tabla con identificador y categoría.

DATOS
[Solicitudes nuevas]
```

Esta base se reutilizará en few-shot.

No eliminaremos reglas para favorecer los ejemplos.

Tampoco añadiremos requisitos distintos en la evaluación.

**La técnica debe compararse contra una alternativa razonable.**

### 2.3. Construir pares de entrada y salida

Cada demostración debe mostrar una correspondencia clara.

Utiliza identificadores si necesitas revisar el conjunto.

Ejemplo:

```text
EJEMPLO E01

Entrada:
¿Cuál es la duración de la formación?

Salida:
Información
```

Comprueba que la salida corresponda exactamente a la entrada.

No dejes respuestas sin etiquetar.

No mezcles varias entradas si la tarea procesa una por vez.

Conserva el mismo vocabulario de categorías.

Un error tipográfico puede cambiar un nombre de campo.

**Los pares deben poder auditarse de forma independiente.**

### 2.4. Elegir ejemplos representativos

Un ejemplo representativo enseña un patrón relevante.

No necesita ser estadísticamente representativo de toda una organización.

Para esta unidad buscamos cobertura conceptual.

Incluye ejemplos que ayuden a distinguir:

- Categorías frecuentes.
- Categorías confundibles.
- Información insuficiente.
- Excepciones relevantes.
- Estructuras de salida.

No utilices cuatro ejemplos que enseñen exactamente lo mismo.

La variedad debe responder a las reglas.

Evita introducir dificultad que no corresponde a la tarea.

Documenta el motivo de cada selección.

**La cobertura útil es más importante que la diversidad decorativa.**

### 2.5. Incluir casos fronterizos

Un caso fronterizo obliga a aplicar una distinción importante.

Por ejemplo, describir un fallo y preguntar cómo resolverlo.

Si la política exige Incidencia, el ejemplo puede mostrar esa prioridad.

Pero la prioridad debe estar también en las reglas.

No utilices ejemplos para introducir políticas ocultas.

La persona revisora debe comprender por qué la salida es correcta.

Preguntas de revisión:

- ¿Qué regla aplica?
- ¿Qué categoría alternativa podría confundirse?
- ¿Qué diferencia enseña?
- ¿La respuesta es inequívoca bajo la política?

Si hay desacuerdo, aclara la regla primero.

**Una demostración no corrige una política mal definida.**

### 2.6. Evitar etiquetas incorrectas

Una etiqueta incorrecta puede perjudicar las respuestas posteriores.

Revisa todas las demostraciones antes de utilizarlas.

Para cada una, comprueba:

- Entrada completa.
- Regla aplicable.
- Categoría correcta.
- Ortografía consistente.
- Ausencia de inferencias innecesarias.
- Correspondencia con el formato.

La revisión por otra persona resulta útil.

No uses automáticamente una respuesta del modelo como referencia.

Si el modelo propone ejemplos, debes validarlos.

Una demostración generada no se convierte en correcta por estar bien redactada.

**La calidad del conjunto depende de su revisión.**

### 2.7. Mantener el formato consistente

Las demostraciones deben representar el formato que deseas obtener.

Si pides una tabla, define sus columnas.

Si pides JSON, utiliza JSON válido.

Si pides una etiqueta, no añadas comentarios dentro de algunas salidas.

La inconsistencia puede enseñar varias convenciones incompatibles.

Ejemplo problemático:

```text
Salida 1: Información
Salida 2: Es una incidencia porque hay un fallo.
Salida 3: {"tipo": "Sugerencia"}
```

Las tres salidas podrían transmitir formatos distintos.

Selecciona uno para la tarea.

**La coherencia estructural facilita una evaluación clara.**

### 2.8. Separar demostraciones y evaluación

Los ejemplos incluidos en el prompt no deben ser los mismos casos con los que mides resultados.

Repetirlos evalúa principalmente reproducción.

No demuestra aplicación a entradas nuevas.

Utilizaremos tres conjuntos:

- Demostraciones: incluidas en few-shot.
- Desarrollo: utilizadas para ajustar el diseño.
- Evaluación reservada: utilizadas al final.

No necesitas una infraestructura compleja.

Sí necesitas identificar a qué conjunto pertenece cada caso.

No muevas un fallo al conjunto de ejemplos y después cuentes su resolución como evaluación independiente.

Eso cambia las condiciones de la prueba.

**La separación protege la interpretación del resultado.**

### 2.9. Evitar filtraciones de respuesta

Una filtración ocurre cuando el prompt proporciona información que revela la respuesta evaluada.

Puede suceder de forma evidente o indirecta.

Ejemplos:

- Añadir la etiqueta al identificador.
- Incluir la respuesta esperada en un comentario.
- Reutilizar el mismo texto como demostración.
- Mostrar una tabla de referencia durante la ejecución.
- Incorporar pistas específicas del conjunto final.

La persona evaluadora puede conocer las respuestas.

El modelo no debe recibirlas como parte de la entrada nueva.

Conserva la referencia en un documento separado.

Comprueba el prompt completo antes de enviarlo.

**Una respuesta correcta con la solución incluida no demuestra la capacidad que queremos medir.**

### 2.10. Número y orden de demostraciones

No existe un número óptimo universal.

Empieza con un conjunto pequeño y justificado.

Después puedes probar ampliaciones.

La utilidad marginal puede disminuir.

Los ejemplos también ocupan contexto y requieren mantenimiento.

El orden puede influir en algunos modelos o tareas.

Para estudiar el orden, mantén el contenido y cambia solo su posición.

No concluyas un efecto general a partir de una ejecución.

Registra el orden exacto.

No mezcles ese experimento con cambios de reglas.

**Número y orden son decisiones que pueden evaluarse, no recetas fijas.**

### 2.11. Coste, longitud y mantenimiento

Few-shot normalmente añade contenido a la solicitud.

Eso puede aumentar el consumo de tokens.

En servicios con facturación por uso puede aumentar el coste.

También puede afectar al tiempo de respuesta.

El efecto real depende de la plataforma.

La reutilización o caché puede modificar las condiciones económicas.

No calcules precios sin datos del servicio.

Registra:

- Longitud si puedes medirla.
- Tiempo si lo has observado.
- Esfuerzo de mantenimiento.
- Calidad obtenida.
- Restricciones del entorno.

**Una mejora pequeña puede no justificar un diseño mucho más complejo.**

### 2.12. Plantilla de comparación

Utiliza esta ficha antes de ejecutar.

Completa las decisiones, no solo los títulos.

```text
Tarea:
Reglas:
Formato:
Criterios:

Condición A:
Zero-shot sin demostraciones.

Condición B:
Misma base con demostraciones identificadas.

Qué mantengo constante:
Qué cambia:
Conjunto de desarrollo:
Conjunto reservado:
Limitaciones conocidas:
```

---

## 3. Sesión práctica: comparar clasificación zero-shot y few-shot

La práctica principal utiliza solicitudes ficticias.

Las reglas están definidas para que podamos construir una referencia y revisar los resultados de forma independiente.

### 3.1. Agenda de los 90 minutos

La sesión combina explicación, ejecución y revisión.

Las ampliaciones no son obligatorias.

| Minutos | Actividad | Evidencia |
|---|---|---|
| 00–15 | Conceptos y demostración | Distinciones básicas |
| 15–25 | Preparación de reglas | Ficha de comparación |
| 25–40 | Zero-shot en desarrollo | Respuesta y revisión |
| 40–55 | Few-shot en desarrollo | Respuesta y revisión |
| 55–70 | Evaluación reservada | Resultados comparables |
| 70–82 | Revisión por parejas | Evidencias verificadas |
| 82–90 | Conclusión y entrega | Decisión documentada |

No es necesario repetir cada prueba muchas veces.

Las repeticiones pueden hacerse como ampliación.

Una ejecución por condición ofrece una observación limitada.

**No la presentaremos como una tasa general de fiabilidad.**

### 3.2. Preparar el entorno

Crea un documento para registrar la actividad.

Abre conversaciones nuevas cuando sea posible.

Anota:

```text
Participante:
Fecha:
Plataforma:
Modelo visible:
Conversación nueva:
Memoria o personalización conocida:
Herramientas conocidas:
Parámetros visibles:
```

No actives búsqueda ni otras herramientas para esta clasificación.

La tarea se resuelve con el texto proporcionado.

Si no puedes desactivarlas, registra su estado.

No inventes datos del entorno.

**La comparación necesita condiciones conocidas.**

### 3.3. Política de clasificación

Utilizaremos cuatro categorías.

Las definiciones son parte de la tarea.

| Categoría | Regla |
|---|---|
| Incidencia | Describe un fallo concreto de funcionamiento o acceso |
| Información | Solicita un dato o procedimiento sin describir un fallo |
| Sugerencia | Propone una modificación o mejora |
| No determinada | No aporta información suficiente para aplicar otra categoría |

Aplicaremos esta prioridad cuando existan varios componentes:

1. Incidencia.
2. Sugerencia.
3. Información.
4. No determinada.

Esta prioridad es una política didáctica.

No representa una recomendación universal para atención al cliente.

**Las respuestas correctas dependen de estas reglas explícitas.**

### 3.4. Aclaraciones de la política

Una pregunta sobre un fallo continúa siendo Incidencia.

Por ejemplo, preguntar cómo resolver un acceso fallido.

Una propuesta acompañada de una consulta será Sugerencia si no hay fallo.

Una solicitud vaga será No determinada.

No debemos inferir un problema a partir de “ayuda”.

Tampoco debemos confundir una mención de un recurso con una incidencia.

Para revisar, identifica primero si se describe un fallo.

Después comprueba si hay propuesta.

Después comprueba si hay solicitud informativa.

Finalmente utiliza No determinada si falta contenido.

La prioridad evita exigir varias etiquetas.

**Clasificamos según el texto y la política, no según palabras aisladas.**

### 3.5. Conjunto de demostraciones

Estas entradas se utilizarán únicamente en few-shot.

No forman parte de la puntuación.

```text
E01
Entrada: La página muestra un error al iniciar sesión.
Salida: Incidencia

E02
Entrada: ¿Cuál es la duración del curso?
Salida: Información

E03
Entrada: Propongo añadir ejercicios con documentos largos.
Salida: Sugerencia

E04
Entrada: Necesito ayuda.
Salida: No determinada
```

Cada ejemplo representa una categoría.

Comprueba su corrección antes de continuar.

### 3.6. Justificar las demostraciones

Anota qué enseña cada ejemplo.

No basta con decir que son variados.

E01 muestra un fallo concreto.

E02 muestra una pregunta sin fallo.

E03 muestra una propuesta explícita.

E04 muestra información insuficiente.

El conjunto cubre las cuatro categorías.

No cubre todavía todos los casos de prioridad.

Podríamos añadir un caso fronterizo en otra versión.

Para la comparación inicial mantendremos estos cuatro.

Así evitamos modificar el experimento durante la ejecución.

**Documentar una carencia no obliga a cambiar inmediatamente el diseño.**

### 3.7. Conjunto de desarrollo

Utiliza estas ocho solicitudes para la primera comparación.

```text
D01: El archivo se descarga vacío.
D02: ¿Dónde puedo consultar el programa?
D03: Sugiero incluir una pausa adicional.
D04: Tengo una consulta.
D05: No puedo abrir el enlace; ¿cómo lo soluciono?
D06: Sería útil añadir subtítulos. ¿Está previsto?
D07: ¿Cómo puedo cambiar mi contraseña?
D08: La aplicación se cierra al cargar el documento.
```

No incluyen las respuestas.

Copia los textos sin modificarlos.

Los identificadores no codifican categorías.

Guarda esta entrada como un archivo separado.

**El conjunto permite observar casos directos y casos con prioridad.**

### 3.8. Referencia del conjunto de desarrollo

Esta referencia sirve para la revisión humana.

No la incluyas en el prompt ejecutado.

| Caso | Categoría | Motivo |
|---|---|---|
| D01 | Incidencia | Descarga defectuosa |
| D02 | Información | Pregunta por ubicación |
| D03 | Sugerencia | Propone una modificación |
| D04 | No determinada | Consulta sin contenido |
| D05 | Incidencia | Describe un fallo |
| D06 | Sugerencia | Propuesta con consulta |
| D07 | Información | Procedimiento sin fallo descrito |
| D08 | Incidencia | Cierre de aplicación |

Revisa la referencia con otra persona si es posible.

Si hay desacuerdo, vuelve a las reglas.

No modifiques etiquetas para coincidir con el modelo.

**La referencia debe establecerse independientemente de la salida.**

### 3.9. Prompt zero-shot

Utiliza esta base para la condición A.

Inserta después las solicitudes de desarrollo.

```text
Clasifica cada solicitud con una sola categoría.

REGLAS
Incidencia: describe un fallo concreto de funcionamiento o acceso.
Información: solicita un dato o procedimiento sin describir un fallo.
Sugerencia: propone una modificación o mejora.
No determinada: no aporta información suficiente.

Si hay varios componentes, aplica esta prioridad:
Incidencia > Sugerencia > Información > No determinada.

No inventes detalles.
Devuelve únicamente una tabla con identificador y categoría.

SOLICITUDES
[Inserta aquí las solicitudes]
```

Guarda el prompt completo.

### 3.10. Ejecutar zero-shot en desarrollo

Envía la condición A en una conversación nueva.

Conserva la respuesta completa.

Comprueba primero la estructura.

Después comprueba cada categoría.

Registra:

- Casos omitidos.
- Identificadores duplicados.
- Etiquetas no permitidas.
- Categorías incorrectas.
- Texto adicional no solicitado.

Un error de formato no siempre implica una categoría incorrecta.

Documenta ambas dimensiones por separado.

No corrijas la salida original.

Puedes añadir una tabla de revisión.

**La evidencia debe mostrar lo recibido, no una versión reparada.**

### 3.11. Prompt few-shot

Construye la condición B a partir de la misma base.

No cambies las reglas ni el formato.

La estructura será:

```text
[Inserta aquí la misma instrucción y las mismas reglas]

EJEMPLOS RESUELTOS
E01: La página muestra un error al iniciar sesión.
Categoría: Incidencia

E02: ¿Cuál es la duración del curso?
Categoría: Información

E03: Propongo añadir ejercicios con documentos largos.
Categoría: Sugerencia

E04: Necesito ayuda.
Categoría: No determinada

SOLICITUDES NUEVAS
[Inserta aquí las mismas solicitudes de desarrollo]
```

Sustituye todos los marcadores.

### 3.12. Ejecutar few-shot en desarrollo

Abre otra conversación.

Envía la condición B completa.

Guarda la respuesta.

Aplica exactamente la misma revisión.

No añadas criterios para favorecer una estrategia.

Comprueba que el modelo no devuelva las demostraciones.

Comprueba que resuelva solo D01 a D08.

Registra cualquier diferencia relevante.

Si ambas condiciones cumplen, anota un empate en esta muestra.

Si few-shot empeora, anota el fallo concreto.

Si mejora, identifica dónde.

**El resultado de la técnica no se presupone antes de ejecutar.**

### 3.13. Matriz de comparación en desarrollo

Completa una fila por entrada.

Utiliza la referencia ya definida.

| Caso | Referencia | Zero-shot | Few-shot |
|---|---|---|---|
| D01 | Incidencia | Registrar | Registrar |
| D02 | Información | Registrar | Registrar |
| D03 | Sugerencia | Registrar | Registrar |
| D04 | No determinada | Registrar | Registrar |
| D05 | Incidencia | Registrar | Registrar |
| D06 | Sugerencia | Registrar | Registrar |
| D07 | Información | Registrar | Registrar |
| D08 | Incidencia | Registrar | Registrar |

Añade observaciones después de la tabla.

Cuenta aciertos sin incluir demostraciones.

Revisa también formato y completitud.

**La matriz permite localizar diferencias, no solo resumir una puntuación.**

### 3.14. Ajustes antes de la evaluación final

Puedes realizar una revisión usando el conjunto de desarrollo.

Si la haces, documenta qué cambias.

La evaluación reservada debe ejecutarse después de congelar las versiones.

No ajustes tras consultar sus resultados y presentes la nueva puntuación como independiente.

Opciones válidas:

- Mantener las dos versiones iniciales.
- Corregir una ambigüedad común en ambas.
- Crear una nueva comparación documentada.
- Añadir un ejemplo y evaluar una nueva versión.

Para la práctica básica recomendamos mantener las versiones iniciales.

Así la diferencia continúa siendo la presencia de cuatro demostraciones.

No incorpores D01 a D08 como ejemplos.

**El conjunto de desarrollo orienta decisiones; el reservado comprueba la versión elegida.**

### 3.15. Conjunto de evaluación reservada

Utiliza estas doce entradas al final.

No incluyas su referencia en la solicitud.

```text
T01: El vídeo no reproduce sonido.
T02: ¿Qué materiales necesitamos?
T03: Propongo publicar una guía de repaso.
T04: Buenas tardes.
T05: La descarga falla y sugiero ofrecer otro formato.
T06: Sería útil una sesión de preguntas. ¿Cuándo podría hacerse?
T07: ¿Cómo se solicita un certificado?
T08: El formulario no permite enviar la respuesta.
T09: Quiero comentar algo.
T10: ¿Dónde está el enlace a la grabación?
T11: Sugiero ampliar el plazo de entrega.
T12: No puedo entrar. ¿Qué navegador recomiendan?
```

Mantén los identificadores.

### 3.16. Referencia de evaluación reservada

Esta tabla es para la revisión posterior.

No se envía al modelo.

| Caso | Categoría | Regla aplicada |
|---|---|---|
| T01 | Incidencia | Fallo de reproducción |
| T02 | Información | Consulta de materiales |
| T03 | Sugerencia | Propuesta de guía |
| T04 | No determinada | Saludo sin solicitud |
| T05 | Incidencia | Fallo con propuesta |
| T06 | Sugerencia | Propuesta con pregunta |
| T07 | Información | Consulta de procedimiento |
| T08 | Incidencia | Fallo del formulario |
| T09 | No determinada | Comentario no especificado |
| T10 | Información | Consulta de ubicación |
| T11 | Sugerencia | Propuesta de plazo |
| T12 | Incidencia | Fallo con pregunta |

Comprueba especialmente los casos con prioridad.

### 3.17. Ejecutar la evaluación reservada

Ejecuta ambas condiciones con T01 a T12.

Utiliza conversaciones nuevas cuando sea posible.

No cambies las instrucciones entre las dos ejecuciones.

Sustituye únicamente las solicitudes.

Guarda ambos prompts completos.

Guarda ambas respuestas completas.

Revisa contra la referencia reservada.

Cuenta los casos correctamente clasificados.

Identifica los errores por categoría.

Comprueba estructura y completitud.

No mezcles resultados de desarrollo y evaluación en una sola cifra sin distinguirlos.

No incluyas E01 a E04 en el recuento.

**La evaluación final debe conservar la separación entre conjuntos.**

### 3.18. Calcular y comunicar resultados

Puedes expresar el resultado como aciertos sobre casos evaluados.

Ejemplo simulado:

```text
Zero-shot: 10 aciertos de 12 casos.
Few-shot: 11 aciertos de 12 casos.

Zero-shot: aproximadamente 83,33 %.
Few-shot: aproximadamente 91,67 %.
```

Estos números son ilustrativos.

Sustitúyelos por tus resultados reales.

La diferencia simulada es de un caso.

Equivale aproximadamente a 8,33 puntos porcentuales.

No equivale a una mejora general demostrada del sistema.

Una muestra tan pequeña exige prudencia.

**Comunica primero los recuentos y después la interpretación.**

### 3.19. Revisión por parejas

Intercambia tus evidencias.

La persona revisora debe comprobar:

- Que las reglas sean iguales.
- Que las entradas sean iguales.
- Que solo B incluya demostraciones.
- Que no se hayan filtrado respuestas.
- Que los recuentos sean correctos.
- Que las conclusiones respeten la muestra.

Anota una fortaleza metodológica.

Anota una limitación.

Si encontráis un error de referencia, revisad la política.

Si corregís la referencia, indicadlo en el documento.

No ocultéis el cambio.

**La revisión externa también evalúa el experimento, no solo al modelo.**

### 3.20. Conclusión de la práctica principal

Redacta una decisión breve.

Utiliza esta estructura:

```text
En esta tarea y con estos casos observé:

La diferencia principal fue:

Los ejemplos ayudaron o no ayudaron en:

El coste adicional conocido fue:

No puedo concluir todavía:

Para la siguiente versión utilizaría:

La siguiente comprobación sería:
```

La decisión puede favorecer cualquiera de los enfoques.

También puede recomendar continuar evaluando.

**Elige según evidencia y necesidades, no según el nombre de la técnica.**

---

## 4. Ampliaciones, evaluación y transferencia a otras tareas

Esta sección permite aplicar la metodología a extracción y estilo, además de documentar el entregable de la unidad.

Las ampliaciones no forman parte obligatoria de los 90 minutos.

### 4.1. Ampliación de extracción

El objetivo es extraer campos sin inventar valores.

Utiliza esta entrada:

```text
La sesión tendrá 14 participantes.
La duración prevista es de 90 minutos.
La modalidad será online.
El aula no aplica a esta solicitud.
La fecha todavía no está confirmada.
```

Define campos antes de ejecutar.

Puedes utilizar:

- Participantes.
- Duración.
- Modalidad.
- Fecha.

El aula se omite porque no pertenece al esquema elegido.

**Un esquema debe indicar qué se extrae y qué queda fuera.**

### 4.2. Zero-shot para extracción

Utiliza esta condición como referencia.

```text
Extrae los datos del texto.

Devuelve únicamente JSON con:
- participantes: entero o null
- duracion_minutos: entero o null
- modalidad: texto o null
- fecha: texto o null

Utiliza null si un dato no aparece o no está confirmado.
No inventes valores.
No añadas bloques Markdown.

TEXTO
[Inserta aquí el texto nuevo]
```

La política de fecha es específica de esta práctica.

Comprueba sintaxis y contenido.

**JSON válido no garantiza extracción correcta.**

### 4.3. Few-shot para extracción

Mantén las mismas reglas y añade demostraciones revisadas.

Ejemplos:

```text
Entrada:
Participarán 8 personas durante 60 minutos.
La sesión será presencial.
Fecha confirmada: 10 de diciembre de 2026.

Salida:
{"participantes":8,"duracion_minutos":60,
"modalidad":"presencial","fecha":"10 de diciembre de 2026"}

Entrada:
La sesión será online.
No conocemos todavía participantes, duración ni fecha.

Salida:
{"participantes":null,"duracion_minutos":null,
"modalidad":"online","fecha":null}
```

Después añade la entrada nueva.

No uses estos mismos ejemplos para medir la extracción.

### 4.4. Evaluar la extracción

Compara campo por campo.

No evalúes solo si el objeto se puede leer.

Criterios:

- Nombres de campos correctos.
- Tipos correctos.
- Valores fieles.
- Ausencias representadas como `null`.
- Fecha no inventada.
- Ausencia de texto adicional.

Para la entrada nueva, participantes debe ser 14.

Duración debe ser 90.

Modalidad debe ser online.

Fecha debe ser `null` bajo la política establecida.

El orden de propiedades no cambia necesariamente el significado.

**La estructura y la semántica requieren comprobaciones separadas.**

### 4.5. Ampliación de estilo

El objetivo es adaptar un texto sin perder contenido.

Define primero qué significa el estilo solicitado.

Por ejemplo:

- Frases breves.
- Tono profesional.
- Lenguaje directo.
- Sin promesas.
- Sin entusiasmo exagerado.

Utiliza esta entrada:

```text
La fecha de la sesión continúa pendiente.
Necesitamos confirmar el número de participantes.
Después prepararemos las opciones disponibles.
```

Las demostraciones deben conservar esa política.

No añadas compromisos al reescribir.

**Imitar estilo no autoriza modificar hechos.**

### 4.6. Demostraciones de estilo

Estas parejas muestran una transformación controlada.

No representan textos de autores ni organizaciones reales.

```text
Entrada:
Procederemos a comunicar las alternativas cuando dispongamos de los datos.

Salida:
Enviaremos las alternativas cuando tengamos los datos.

Entrada:
Resulta necesario que se confirme previamente la duración prevista.

Salida:
Necesitamos confirmar la duración antes de continuar.
```

Los ejemplos reducen formalismo innecesario.

Mantienen condiciones y acciones.

No convierten posibilidades en garantías.

Revisa la salida nueva por fidelidad y estilo.

**Un cambio expresivo puede ser incorrecto si altera el compromiso.**

### 4.7. Ampliación sobre cantidad y orden

Puedes estudiar dos variables en pruebas separadas.

Primera prueba: número de ejemplos.

Segunda prueba: orden de ejemplos.

Para cantidad, compara:

- Ningún ejemplo.
- Un ejemplo justificado.
- Cuatro ejemplos.

Para orden, conserva los mismos cuatro y cambia su secuencia.

Mantén reglas y entradas.

Utiliza un conjunto reservado distinto si ya ajustaste con el anterior.

Registra todas las condiciones.

No selecciones únicamente la ejecución más favorable.

Una muestra pequeña ofrece información exploratoria.

**Cambiar varias variables simultáneamente impide atribuir el resultado a una sola.**

### 4.8. Errores frecuentes

Los problemas de diseño suelen repetirse.

Reconocerlos facilita corregirlos.

Errores habituales:

- Crear un zero-shot incompleto.
- Añadir reglas solo a few-shot.
- Utilizar ejemplos mal etiquetados.
- Reutilizar demostraciones como evaluación.
- Cambiar formato entre condiciones.
- Incluir respuestas esperadas en el prompt.
- Ajustar después de ver la evaluación reservada.
- Generalizar a partir de pocos casos.
- Ignorar el coste de mantenimiento.
- Presentar resultados simulados como reales.

Cada error afecta a una parte diferente del proceso.

**Revisa primero el experimento antes de atribuir el problema al modelo.**

### 4.9. Entregable de la unidad

Entrega una comparación documentada.

No necesitas un informe extenso.

Debe incluir:

1. Ficha del entorno.
2. Tarea y reglas.
3. Criterios de aceptación.
4. Prompt zero-shot completo.
5. Prompt few-shot completo.
6. Demostraciones y justificación.
7. Conjuntos de desarrollo y evaluación.
8. Respuestas originales.
9. Matriz de resultados.
10. Decisión y limitaciones.

Las ampliaciones pueden añadirse como anexos.

**No entregues únicamente el prompt que obtuvo mejor resultado.**

### 4.10. Checklist y rúbrica formativa

Revisa la documentación antes de enviarla.

Las comprobaciones principales son:

- [ ] La tarea es la misma.
- [ ] Las reglas son iguales.
- [ ] Los ejemplos están revisados.
- [ ] Los conjuntos están separados.
- [ ] No hay respuestas filtradas.
- [ ] Las salidas originales están guardadas.
- [ ] Los recuentos están comprobados.
- [ ] La decisión tiene evidencia.

La evaluación considera diseño, revisión y transparencia.

Una comparación sin mejora puede estar correctamente realizada.

Una puntuación alta no compensa un experimento mal definido.

Documenta también lo que no conoces del entorno.

**La calidad del trabajo depende de la validez de sus conclusiones.**

### 4.11. Recursos relacionados

Utiliza las plantillas del curso para continuar.

Estos recursos apoyan documentación y evaluación.

- [Plantillas](../plantillas/index.md)
- [Ficha de prompt](../plantillas/ficha-de-prompt.md)
- [Registro de versiones](../plantillas/registro-de-versiones.md)
- [Matriz de evaluación](../plantillas/matriz-de-evaluacion.md)
- [Checklist de seguridad](../plantillas/checklist-de-seguridad.md)
- [Proyecto final](../proyecto-final/index.md)

Mantén las demostraciones junto a su justificación.

Versiona cambios en reglas y ejemplos.

Conserva los resultados originales.

No transfieras una conclusión a otra tarea sin nuevas pruebas.

**La reutilización exige comprobar que las condiciones siguen siendo pertinentes.**

### 4.12. Ideas esenciales para avanzar

Zero-shot no incluye demostraciones resueltas.

Few-shot incorpora unas pocas demostraciones dentro del contexto.

Ambos enfoques necesitan tareas claras.

Few-shot no equivale a fine-tuning.

Los ejemplos deben ser correctos y pertinentes.

Las reglas no deberían quedar ocultas en las demostraciones.

El conjunto de evaluación debe permanecer separado.

Una comparación justa mantiene constantes las condiciones relevantes.

La exactitud debe revisarse junto con formato y completitud.

Los ejemplos añaden contenido y mantenimiento.

Un resultado favorable no demuestra fiabilidad general.

**La mejor estrategia es la que aporta valor comprobable para la tarea y el entorno evaluados.**