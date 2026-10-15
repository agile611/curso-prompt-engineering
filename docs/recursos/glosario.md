# Glosario

Este glosario reúne los conceptos necesarios para comprender, diseñar, evaluar y documentar soluciones basadas en prompts.

Amplía los términos del material original y los relaciona con las decisiones habituales del curso de Prompt Engineering.

Las definiciones buscan precisión sin exigir conocimientos previos de programación.

Cada término incluye su significado, aplicaciones y distinciones que ayudan a evitar interpretaciones incorrectas.

El vocabulario debe servir para describir lo que realmente se ha diseñado y comprobado.

**Conocer un término no equivale a haber implementado o validado la capacidad que describe.**

Los ejemplos son originales y utilizan información sintética.

Las actividades de sesión permiten practicar el uso de los conceptos en situaciones delimitadas.

Las respuestas de referencia son materiales docentes, no resultados obtenidos mediante ejecuciones reales.

El recorrido básico puede completarse con una interfaz autorizada y un editor de texto.

Las actividades técnicas son adaptables a los conocimientos del grupo.

!!! info "Cómo consultar el glosario"
    Busca primero el concepto relacionado con tu tarea.
    Revisa sus distinciones antes de utilizarlo en una conclusión.
    Mantén los términos consistentes entre fichas, pruebas e informes.
    Consulta las prácticas finales para aplicar el vocabulario.

!!! warning "Límite de las definiciones"
    Los productos pueden utilizar nombres comerciales diferentes.
    Las capacidades dependen del modelo, la aplicación y su configuración.
    Este glosario no autoriza datos, herramientas ni operaciones.
    Una definición no sustituye una comprobación del entorno utilizado.

---

## 1. Modelos de lenguaje y aplicaciones

Estos términos distinguen el modelo que genera contenido de la aplicación que organiza su utilización.

### 1.1. LLM

**LLM** significa *Large Language Model*: modelo de lenguaje de gran tamaño.

- Se entrena para reconocer patrones y generar secuencias de lenguaje.
- Puede realizar tareas diferentes mediante instrucciones y contexto.
- Sus capacidades dependen del entrenamiento y del entorno de utilización.

Un LLM no consulta necesariamente una fuente externa cuando responde.

**Distinción clave:** una respuesta fluida no demuestra conocimiento verificado.

### 1.2. Modelo generativo

Un **modelo generativo** produce contenido a partir de una entrada y de los patrones aprendidos.

- Puede generar texto, imágenes u otras modalidades.
- La salida no tiene que ser una copia de un material concreto.
- El proceso puede producir variantes ante entradas similares.

Los modelos generativos forman una categoría más amplia que los LLM.

**Distinción clave:** generar contenido no equivale a validar su corrección.

### 1.3. Aplicación basada en un modelo

Una **aplicación basada en un modelo** combina generación con interfaz, reglas y otros componentes.

- Puede incorporar instrucciones que el usuario no ve.
- Puede limitar herramientas y operaciones.
- Puede almacenar contexto o conectar documentos.

El comportamiento observado pertenece al conjunto de la aplicación.

**Distinción clave:** no atribuyas al modelo una función realizada por otro componente.

### 1.4. Sistema basado en prompts

Un **sistema basado en prompts** utiliza instrucciones como parte de una solución organizada.

- Define entradas, transformaciones y salidas.
- Puede incluir varios modelos o etapas.
- Necesita evaluación, documentación y controles adecuados.

Un mensaje aislado puede formar parte del sistema, pero no lo describe entero.

**Distinción clave:** diseñar un prompt y diseñar un sistema son tareas relacionadas, no idénticas.

---

## 2. Unidades de procesamiento y límites

Estos conceptos explican cómo se representa la información y por qué existen límites de entrada y salida.

### 2.1. Token

Un **token** es una unidad de representación que utiliza el modelo para procesar contenido.

- Puede corresponder a una palabra, parte de ella o un signo.
- Su segmentación depende del tokenizador.
- No existe una equivalencia fija entre palabras y tokens.

En otros tipos de contenido, la representación puede seguir mecanismos diferentes.

**Distinción clave:** contar palabras no permite conocer exactamente el número de tokens.

### 2.2. Tokenizador

Un **tokenizador** transforma contenido en unidades que el modelo puede manejar.

- Divide el texto según reglas o vocabularios determinados.
- Asigna identificadores a las unidades resultantes.
- Puede producir segmentaciones diferentes entre modelos.

Una misma frase puede ocupar cantidades distintas de tokens según el sistema.

**Distinción clave:** la segmentación depende del modelo, no solo del idioma.

### 2.3. Ventana de contexto

La **ventana de contexto** es la capacidad de contenido que el modelo puede considerar en una interacción.

- Incluye información disponible para producir la respuesta.
- Su límite depende del modelo y del servicio.
- Los límites de entrada y salida pueden diferenciarse.

La aplicación puede reservar parte de esa capacidad para instrucciones adicionales.

**Distinción clave:** que una interfaz acepte un archivo no demuestra que se utilice íntegramente.

### 2.4. Truncamiento

El **truncamiento** ocurre cuando una entrada o una salida se recorta.

- Puede deberse a límites del modelo o de la aplicación.
- Puede eliminar información necesaria para la tarea.
- Debe distinguirse de una omisión dentro de una respuesta completa.

Una respuesta interrumpida necesita interpretarse según sus condiciones.

**Distinción clave:** no atribuyas un fallo semántico sin comprobar si faltó contenido procesable.

---

## 3. Prompts e instrucciones

El prompt reúne contenido utilizado para orientar una generación, pero sus partes pueden tener funciones diferentes.

### 3.1. Prompt

Un **prompt** es el conjunto de instrucciones y datos proporcionados al modelo para una tarea.

- Puede incluir objetivo, contexto, fuentes y restricciones.
- Puede contener ejemplos de entrada y salida.
- Puede proceder de varios mensajes o capas de la aplicación.

En el curso, se documenta el texto visible y las condiciones conocidas.

**Distinción clave:** el mensaje del usuario no siempre representa todo el contexto efectivo.

### 3.2. Instrucción

Una **instrucción** indica una operación, una restricción o una condición de respuesta.

- “Extrae los requisitos” define una acción.
- “No confirmes disponibilidad” establece un límite.
- “Devuelve una tabla” especifica presentación.

Las instrucciones deben ser compatibles entre sí y con el alcance.

**Distinción clave:** una instrucción expresa una expectativa, no demuestra su cumplimiento.

### 3.3. Contexto

El **contexto** es la información disponible que ayuda a interpretar y resolver la tarea.

- Puede incluir antecedentes pertinentes.
- Puede incorporar documentos y mensajes anteriores.
- Puede contener preferencias o reglas de la aplicación.

Añadir contexto irrelevante puede dificultar la interpretación de la entrada.

**Distinción clave:** contexto suficiente no significa contexto máximo.

### 3.4. Restricción

Una **restricción** delimita contenido, transformaciones u operaciones permitidas.

- Puede prohibir inferencias no autorizadas.
- Puede limitar el formato de salida.
- Puede excluir decisiones o acciones externas.

Las restricciones de alto impacto necesitan controles adicionales cuando corresponda.

**Distinción clave:** una prohibición escrita no constituye una barrera técnica suficiente.

---

## 4. Plantillas, variables y preparación

Estos términos permiten reutilizar instrucciones sin ocultar qué valores se emplearon en cada ejecución.

### 4.1. Plantilla de prompt

Una **plantilla de prompt** conserva reglas estables y espacios para información variable.

- Separa la tarea de sus entradas concretas.
- Facilita reutilización y mantenimiento.
- Debe identificar los marcadores que necesita completar.

Una plantilla puede utilizarse con distintos casos dentro del alcance documentado.

**Distinción clave:** reutilizable no significa adecuada para cualquier entrada.

### 4.2. Variable

Una **variable** representa un contenido que puede cambiar entre ejecuciones.

- `solicitud` puede contener un mensaje sintético.
- `expediente_id` identifica un caso.
- `catalogo` puede aportar categorías autorizadas.

Cada variable necesita significado, formato y tratamiento de ausencia.

**Distinción clave:** el nombre de una variable no basta para definirla.

### 4.3. Marcador

Un **marcador** señala dónde debe introducirse un valor en una plantilla.

- Puede representarse como `{{solicitud}}`.
- Su sintaxis depende del procedimiento utilizado.
- No todos los servicios lo sustituyen automáticamente.

En una interfaz manual, el operador puede necesitar reemplazarlo explícitamente.

**Distinción clave:** un marcador visible no es necesariamente una variable resuelta.

### 4.4. Prompt completado

El **prompt completado** es la instrucción con los valores concretos utilizados.

- Permite reconstruir una ejecución.
- Conserva la fuente introducida.
- Debe relacionarse con la versión de la plantilla.

La plantilla y el prompt completado son objetos documentales diferentes.

**Distinción clave:** guardar solo la plantilla no demuestra qué información se envió.

---

## 5. Estrategias de formulación

Las estrategias organizan la instrucción para una dificultad concreta y necesitan evaluación posterior.

### 5.1. Zero-shot

**Zero-shot** describe una instrucción sin ejemplos de resolución de la tarea.

- Puede contener reglas detalladas.
- Puede especificar formato y restricciones.
- Puede utilizar documentos como datos de entrada.

La ausencia de ejemplos no implica ausencia de contexto.

**Distinción clave:** zero-shot no significa “prompt breve” ni “sin instrucciones”.

### 5.2. Few-shot

**Few-shot** describe una instrucción acompañada de algunos ejemplos pertinentes.

- Los ejemplos muestran patrones de resolución.
- Deben respetar las reglas del contrato.
- Su selección puede influir en el resultado.

El número adecuado depende de la tarea y de la evaluación.

**Distinción clave:** añadir ejemplos no garantiza mejora ni elimina errores.

### 5.3. One-shot

**One-shot** describe una instrucción que incluye un ejemplo de resolución.

- Puede aclarar un formato sencillo.
- Puede mostrar una transformación difícil de describir.
- Debe evitar introducir reglas contradictorias.

Un ejemplo puede ser insuficiente para representar variantes relevantes.

**Distinción clave:** un patrón mostrado no constituye cobertura de todos los casos.

### 5.4. Asignación de rol

La **asignación de rol** describe una perspectiva o función para orientar la respuesta.

- Puede indicar destinatario y tono.
- Puede ayudar a delimitar una operación.
- No concede credenciales ni autoridad real.

“Actúa como revisor” debe acompañarse de criterios concretos.

**Distinción clave:** un rol textual no transforma al modelo en profesional acreditado.

---

## 6. Descomposición y operaciones lingüísticas

Estos conceptos describen transformaciones que conviene distinguir antes de diseñar un flujo.

### 6.1. Descomposición de tareas

La **descomposición** divide una operación amplia en etapas identificables.

- Puede separar extracción y redacción.
- Permite revisar resultados intermedios.
- Añade contratos y dependencias entre componentes.

Cada etapa necesita una condición de avance y de detención.

**Distinción clave:** más etapas no significan automáticamente mayor fiabilidad.

### 6.2. Extracción

La **extracción** recupera información presente en una fuente según reglas definidas.

- Identifica requisitos o entidades.
- Conserva valores relevantes.
- Puede incluir evidencia localizada.

Las normalizaciones deben estar autorizadas por la política.

**Distinción clave:** extraer no permite completar ausencias mediante suposiciones.

### 6.3. Resumen

Un **resumen** reduce contenido manteniendo información pertinente para una finalidad.

- Selecciona hechos principales.
- Puede reorganizar su presentación.
- Necesita conservar condiciones importantes.

Su calidad depende del destinatario y del criterio de relevancia.

**Distinción clave:** resumir no equivale a eliminar incertidumbres o contradicciones.

### 6.4. Clasificación

La **clasificación** asigna una entrada a categorías según un catálogo o criterio.

- Necesita definiciones de categorías.
- Puede admitir varias etiquetas.
- Puede incluir una ruta de revisión.

El contrato debe aclarar si las categorías son excluyentes.

**Distinción clave:** clasificar no autoriza resolver ni modificar la solicitud.

---

## 7. Generación, revisión y corrección

Estas operaciones producen o examinan contenido, pero no deben confundirse con aprobación.

### 7.1. Borrador

Un **borrador** es una propuesta de contenido pendiente de revisión.

- Puede facilitar la preparación documental.
- Debe conservar datos y restricciones.
- Necesita identificación si se modifica después.

Un borrador puede ser útil aunque requiera correcciones.

**Distinción clave:** presentar un texto bien redactado no equivale a aprobarlo.

### 7.2. Reescritura

La **reescritura** transforma la expresión de un contenido siguiendo condiciones.

- Puede cambiar tono o estructura.
- Puede adaptar el nivel de detalle.
- Debe conservar hechos cuando así lo exige la tarea.

La política debe indicar qué modificaciones semánticas admite.

**Distinción clave:** mejorar el estilo no permite inventar beneficios o compromisos.

### 7.3. Revisión asistida

La **revisión asistida** utiliza un modelo para localizar posibles discrepancias.

- Puede comparar fuentes y borradores.
- Puede identificar criterios afectados.
- Puede producir falsas alarmas u omitir errores.

Sus observaciones necesitan comprobación proporcional al riesgo.

**Distinción clave:** el informe del revisor también es una salida que debe evaluarse.

### 7.4. Corrección humana

Una **corrección humana** modifica un resultado después de revisarlo.

- Debe conservarse la salida original.
- Debe identificarse la intervención.
- Puede requerir una nueva comprobación.

La corrección forma parte del proceso, no del resultado original del modelo.

**Distinción clave:** una edición posterior no convierte retroactivamente una respuesta defectuosa en válida.

---

## 8. Formatos y contratos de datos

Los formatos ayudan a organizar contenido, mientras que el contrato establece condiciones de validez.

### 8.1. Contrato de salida

El **contrato de salida** define estructura y significado admitidos para el resultado.

- Identifica campos o secciones.
- Establece tipos y valores permitidos.
- Describe ausencias, estados y condiciones bloqueantes.

Puede aplicarse a texto, tablas o datos estructurados.

**Distinción clave:** el contrato va más allá de pedir un formato visual.

### 8.2. JSON

**JSON** es un formato textual para representar datos estructurados.

- Utiliza objetos, listas y valores.
- Exige reglas sintácticas concretas.
- Puede facilitar el intercambio entre componentes.

Solicitar JSON no demuestra que la aplicación lo valide.

**Distinción clave:** un JSON válido puede incumplir el esquema o contener información falsa.

### 8.3. Esquema

Un **esquema** describe la estructura admitida para unos datos.

- Define campos obligatorios.
- Establece tipos y restricciones.
- Puede prohibir claves adicionales.

Un esquema puede revisarse manualmente o mediante validadores.

**Distinción clave:** validar estructura no demuestra fidelidad a la fuente.

### 8.4. Valor nulo

Un **valor nulo** representa ausencia de valor según el contrato.

- En JSON se expresa como `null`.
- No equivale a cero ni a texto vacío.
- Su significado debe explicarse en la política.

Puede acompañarse de un estado para distinguir causas de ausencia.

**Distinción clave:** nulo no significa automáticamente desconocido, contradictorio o no aplicable.

---

## 9. Estados e interpretación de información

Los estados permiten conservar condiciones que una cifra o una fecha no expresan por sí solas.

### 9.1. Aproximación

Una **aproximación** indica que un valor no se presenta como exacto.

- “Aproximadamente 12” conserva una condición.
- El número y su estado pueden separarse.
- El tratamiento depende del contrato.

Eliminar la aproximación puede cambiar el significado del resultado.

**Distinción clave:** extraer 12 no basta si la tarea exige conservar “aproximadamente”.

### 9.2. Ausencia

La **ausencia** indica que la fuente no aporta una información requerida.

- Puede representarse mediante nulo.
- Puede acompañarse del estado `ausente`.
- No justifica completar el dato por inferencia.

El tratamiento debe diferenciarse de una entrada inválida.

**Distinción clave:** un campo ausente no equivale a una fuente vacía.

### 9.3. Ambigüedad

La **ambigüedad** permite más de una interpretación relevante.

- Puede afectar a una fecha incompleta.
- Puede aparecer en una categoría indefinida.
- Puede proceder de reglas insuficientes.

La solución puede necesitar aclaración o una representación indeterminada.

**Distinción clave:** una elección plausible no resuelve necesariamente la ambigüedad.

### 9.4. Contradicción

Una **contradicción** reúne afirmaciones incompatibles dentro del alcance interpretado.

- Dos cantidades pueden diferir sin prioridad.
- Dos fuentes pueden describir estados incompatibles.
- La política debe establecer cómo representarlas.

Una corrección explícita puede resolver una incompatibilidad previa.

**Distinción clave:** no trates toda actualización como contradicción sin resolver.

---

## 10. Fiabilidad y errores de contenido

Estos términos describen problemas de generación y condiciones de interpretación, no diagnósticos automáticos.

### 10.1. Alucinación

Una **alucinación** es contenido generado que parece plausible pero no está sustentado.

- Puede incluir hechos inventados.
- Puede presentar citas inexistentes.
- Puede atribuir condiciones que la fuente no contiene.

El término debe aplicarse con evidencia de la falta de respaldo.

**Distinción clave:** no toda diferencia de estilo ni todo desacuerdo es una alucinación.

### 10.2. Fidelidad

La **fidelidad** es la correspondencia entre una salida y la información autorizada.

- Conserva cifras y unidades.
- Mantiene condiciones y estados.
- Evita añadidos incompatibles.

Puede comprobarse aunque la redacción cambie.

**Distinción clave:** fidelidad semántica no exige siempre coincidencia literal.

### 10.3. Incertidumbre

La **incertidumbre** expresa límites en la información o en la conclusión.

- Puede proceder de fuentes incompletas.
- Puede surgir de resultados variables.
- Puede depender de condiciones desconocidas.

Debe representarse sin convertirla en certeza aparente.

**Distinción clave:** un tono seguro no reduce la incertidumbre real.

### 10.4. Sesgo

Un **sesgo** es una tendencia sistemática que puede afectar resultados o decisiones.

- Puede proceder de datos o categorías.
- Puede introducirse mediante ejemplos.
- Puede aparecer en criterios de evaluación.

Su revisión necesita contexto y evidencia pertinente.

**Distinción clave:** una observación aislada no siempre demuestra un patrón sistemático.

---

## 11. Recuperación de información y fuentes

Estos conceptos explican cómo puede incorporarse información externa sin asumir que toda fuente es correcta.

### 11.1. Fuente de verdad

Una **fuente de verdad** es la referencia autorizada para una comprobación determinada.

- Puede ser una solicitud original.
- Puede ser una política vigente.
- Puede ser un registro validado.

Debe identificarse quién establece su autoridad y alcance.

**Distinción clave:** autoridad documental y exactitud factual no son siempre equivalentes.

### 11.2. Recuperación de información

La **recuperación** localiza materiales pertinentes para una consulta.

- Puede utilizar búsqueda exacta.
- Puede utilizar similitud semántica.
- Puede seleccionar fragmentos de un conjunto documental.

La pertinencia recuperada necesita revisión según la tarea.

**Distinción clave:** recuperar un documento no demuestra que el contenido sea correcto.

### 11.3. RAG

**RAG** significa *Retrieval-Augmented Generation*: generación apoyada en recuperación de información.

- Recupera contenido antes o durante la respuesta.
- Incorpora materiales pertinentes al contexto.
- Puede facilitar respaldo y actualización de información.

La calidad depende de recuperación, fuentes, instrucciones y validación.

**Distinción clave:** utilizar RAG no elimina las alucinaciones ni la necesidad de revisión.

### 11.4. Embedding

Un **embedding** es una representación numérica de contenido utilizada para operaciones como similitud.

- Puede representar texto u otras modalidades.
- Permite comparar elementos en un espacio definido.
- Depende del modelo que lo produce.

La similitud no establece autoridad ni verdad.

**Distinción clave:** dos fragmentos cercanos semánticamente pueden contener afirmaciones incompatibles.

---

## 12. Herramientas, flujos y agentes

Las herramientas añaden capacidades cuyo uso requiere contratos y permisos adecuados.

### 12.1. Herramienta

Una **herramienta** es una capacidad externa que una aplicación puede utilizar.

- Consulta de documentos.
- Ejecución de código.
- Acceso a servicios o registros.

Su disponibilidad depende del entorno y de los permisos.

**Distinción clave:** el modelo no dispone necesariamente de las herramientas que menciona.

### 12.2. Llamada a función

Una **llamada a función** solicita una operación con argumentos estructurados.

- El modelo puede proponer argumentos.
- La aplicación puede validarlos.
- La ejecución puede ocurrir fuera del modelo.

El resultado necesita interpretación y gestión de errores.

**Distinción clave:** proponer una llamada no equivale a que la operación se haya ejecutado.

### 12.3. Flujo de trabajo

Un **flujo de trabajo** organiza etapas, entradas y condiciones de avance.

- Puede ser determinista.
- Puede incluir componentes generativos.
- Puede requerir decisiones humanas.

Las transiciones deben comprobar compatibilidad y autoridad.

**Distinción clave:** una secuencia de prompts no es un flujo validado por el mero hecho de ejecutarse.**

### 12.4. Agente

Un **agente** es un sistema que puede seleccionar pasos o herramientas para perseguir un objetivo.

- Su definición varía entre productos y proyectos.
- Puede operar con grados diferentes de autonomía.
- Necesita límites, supervisión y condiciones de finalización.

El término debe explicarse mediante capacidades concretas.

**Distinción clave:** llamar agente a una aplicación no demuestra autonomía segura.**

---

## 13. Evaluación y referencias

La evaluación compara resultados con condiciones definidas y debe mantener separadas expectativas y observaciones.

### 13.1. Caso de prueba

Un **caso de prueba** describe una situación concreta que se pretende comprobar.

- Identifica una entrada.
- Establece un objetivo.
- Incluye una expectativa o referencia.

Un caso puede utilizarse con varias versiones.

**Distinción clave:** varias ejecuciones del mismo caso no constituyen casos distintos.

### 13.2. Ejecución

Una **ejecución** es una observación concreta del comportamiento en unas condiciones.

- Utiliza una versión identificada.
- Recibe una entrada concreta.
- Produce una respuesta que debe conservarse.

Las repeticiones son nuevas observaciones.

**Distinción clave:** ejecutar no implica haber evaluado la respuesta.**

### 13.3. Referencia de evaluación

Una **referencia** expresa qué resultado se considera admisible según la tarea.

- Puede ser una salida exacta.
- Puede ser un conjunto de criterios.
- Puede admitir varias redacciones válidas.

Debe prepararse antes de valorar la generación.

**Distinción clave:** una respuesta docente de referencia no es una ejecución del modelo.**

### 13.4. Criterio de aceptación

Un **criterio de aceptación** establece una condición comprobable del resultado.

- Presencia de campos.
- Conservación de estados.
- Ausencia de compromisos no autorizados.

El criterio debe identificar un procedimiento de revisión.

**Distinción clave:** “respuesta buena” no define una comprobación suficiente.**

---

## 14. Métricas y estados de evaluación

Las métricas resumen observaciones cuando sus unidades y denominadores están claros.

### 14.1. Cumplimiento

El **cumplimiento** indica que un resultado satisface un criterio evaluado.

- Necesita una comprobación.
- Debe relacionarse con evidencia.
- Puede ser parcial según el conjunto de criterios.

El estado global depende de reglas definidas previamente.

**Distinción clave:** no evaluado no significa que cumple.**

### 14.2. Cobertura

La **cobertura** describe qué condiciones o requisitos están representados en la evaluación.

- Puede referirse a tipos de entrada.
- Puede referirse a riesgos.
- Puede referirse a requisitos.

Su suficiencia depende del contexto y del alcance.

**Distinción clave:** más casos no garantizan mayor diversidad relevante.**

### 14.3. Precisión y exhaustividad

La **precisión** y la **exhaustividad** son métricas utilizadas en tareas de clasificación o recuperación.

- Precisión: qué proporción de positivos identificados es correcta.
- Exhaustividad: qué proporción de positivos reales se identifica.
- Ambas necesitan definir la clase o unidad evaluada.

En algunos materiales, exhaustividad se denomina *recall*.

**Distinción clave:** una precisión alta puede coexistir con muchos casos relevantes omitidos.**

### 14.4. Tasa de cumplimiento

La **tasa de cumplimiento** resume resultados favorables dentro de un conjunto definido.

- Debe indicar el denominador.
- Debe declarar exclusiones.
- Debe separar pendientes de resultados evaluados.

Puede calcularse por ejecución o por criterio, pero no deben mezclarse.

**Distinción clave:** un porcentaje sin unidad no permite interpretar correctamente el resultado.**

---

## 15. Versionado y mantenimiento

El mantenimiento conserva identidad, evolución y condiciones de utilización de una solución.

### 15.1. Versionado

El **versionado** identifica y registra cambios de un prompt o sistema.

- Relaciona etiquetas con contenido recuperable.
- Conserva motivos de modificación.
- Documenta efectos observados.

La convención debe mantenerse consistente.

**Distinción clave:** una versión mayor no demuestra una mejora.**

### 15.2. Línea base

La **línea base** es el punto de partida utilizado para una comparación.

- Incluye contenido identificado.
- Conserva casos y referencias.
- Permite interpretar resultados posteriores.

No necesita ser la mejor candidata disponible.

**Distinción clave:** la línea base tiene que ser interpretable, no necesariamente satisfactoria.**

### 15.3. Regresión

Una **regresión** es un deterioro respecto a un requisito anteriormente satisfecho.

- Puede aparecer al corregir otro fallo.
- Puede romper formato o significado.
- Necesita casos de comprobación pertinentes.

La comparación debe conservar condiciones interpretables.

**Distinción clave:** resolver un problema no demuestra conservar todos los demás requisitos.**

### 15.4. Reversión

Una **reversión** recupera un contenido anterior identificado.

- Puede restaurar un prompt.
- Puede recuperar una política.
- Puede reestablecer una combinación compatible.

Las condiciones actuales necesitan nueva revisión.

**Distinción clave:** restaurar contenido no deshace necesariamente acciones externas realizadas.**

---

## 16. Seguridad y límites de confianza

La seguridad requiere distinguir fuentes, instrucciones y operaciones autorizadas.

### 16.1. Prompt injection

**Prompt injection** describe instrucciones en contenido no confiable que intentan desviar la tarea.

- Puede aparecer en documentos o mensajes.
- Puede intentar obtener información restringida.
- Puede solicitar acciones fuera del alcance.

Su tratamiento requiere controles de la aplicación y validación.

**Distinción clave:** una fuente relevante no adquiere autoridad para modificar el objetivo.**

### 16.2. Límite de confianza

Un **límite de confianza** separa componentes o contenidos con distinta autoridad.

- Instrucciones de la aplicación.
- Datos aportados por una fuente.
- Resultados de herramientas externas.

La separación debe reflejarse en el diseño y los permisos.

**Distinción clave:** un delimitador textual no constituye por sí solo aislamiento técnico.**

### 16.3. Mínimo privilegio

El **mínimo privilegio** limita acceso y operaciones a lo necesario para la tarea.

- Lectura sin escritura cuando basta.
- Acceso solo a recursos pertinentes.
- Exclusión de funciones no requeridas.

La configuración debe comprobarse en el entorno.

**Distinción clave:** pedir al modelo que no use una capacidad no equivale a retirarla.**

### 16.4. Riesgo residual

El **riesgo residual** es el riesgo que permanece después de aplicar controles.

- Puede incluir errores no detectados.
- Puede depender de entradas no cubiertas.
- Puede verse afectado por revisión insuficiente.

Su descripción debe reconocer límites de efectividad.

**Distinción clave:** implementar un control no demuestra que el riesgo desaparezca.**

---

## 17. Privacidad y responsabilidad humana

La protección de información y la supervisión requieren procedimientos concretos y autoridad adecuada.

### 17.1. Minimización de datos

La **minimización** utiliza solo información necesaria para una finalidad determinada.

- Reduce identificadores prescindibles.
- Excluye adjuntos ajenos a la tarea.
- Limita contenido en registros y capturas.

También afecta a las salidas conservadas.

**Distinción clave:** tener acceso a un dato no justifica utilizarlo.**

### 17.2. Anonimización y seudonimización

La **anonimización** busca impedir la identificación de personas; la **seudonimización** sustituye identificadores.

- Los códigos pueden seguir permitiendo vinculación.
- El contexto puede facilitar reidentificación.
- Las condiciones deben revisarse según el uso.

Cambiar nombres no basta para declarar anonimato.

**Distinción clave:** seudonimizar reduce exposición directa, pero no garantiza anonimización.**

### 17.3. Revisión humana

La **revisión humana** es una comprobación realizada por una persona con medios adecuados.

- Define campos obligatorios.
- Utiliza una fuente de verdad.
- Permite corregir, derivar o bloquear.

La persona necesita tiempo, acceso y autoridad.

**Distinción clave:** nombrar un revisor no demuestra que exista revisión efectiva.**

### 17.4. Autorización

Una **autorización** permite una operación dentro de condiciones determinadas.

- Debe identificar la acción admitida.
- Puede vincularse a una versión.
- Depende del contexto y del responsable competente.

La aprobación académica tiene alcance formativo.

**Distinción clave:** una salida convincente no concede permiso para actuar.**

---

## 18. Documentación y evidencias

La documentación explica el sistema; las evidencias permiten revisar lo que realmente ocurrió.

### 18.1. Trazabilidad

La **trazabilidad** relaciona requisitos, componentes, pruebas y decisiones.

- Un requisito referencia un criterio.
- Una prueba referencia una ejecución.
- Un cambio referencia una incidencia.

Los enlaces deben conducir a objetos disponibles.

**Distinción clave:** una lista de nombres no demuestra relaciones verificables.**

### 18.2. Evidencia

Una **evidencia** es un material que respalda una observación o conclusión concreta.

- Puede ser una respuesta original.
- Puede ser un registro de validación.
- Puede ser una revisión documentada.

Su suficiencia depende de la afirmación que sostiene.

**Distinción clave:** una captura aislada puede no contener condiciones necesarias de interpretación.**

### 18.3. Incidencia

Una **incidencia** registra una discrepancia o interrupción relevante.

- Describe qué se observó.
- Identifica el criterio afectado.
- Conserva acción y estado.

La hipótesis de causa debe mantenerse separada del hecho.

**Distinción clave:** una explicación posible no demuestra por qué ocurrió el fallo.**

### 18.4. Auditabilidad

La **auditabilidad** es la posibilidad de revisar el trabajo mediante materiales consultables.

- Permite localizar versiones.
- Conserva respuestas y referencias.
- Hace visibles pendientes y decisiones.

No exige una herramienta sofisticada por definición.

**Distinción clave:** documentación extensa no significa documentación fácil de auditar.**

---

## 19. Configuración, reproducibilidad y desempeño

Estos términos ayudan a describir condiciones de generación sin atribuirles garantías que no ofrecen.

### 19.1. Temperatura y top-p

La **temperatura** y **top-p** son parámetros de selección de salida disponibles en algunos entornos.

- La temperatura modifica la distribución utilizada para muestrear.
- Top-p limita la selección a un conjunto de probabilidad acumulada.
- Su exposición y aplicación dependen del servicio.

No todos los modelos o interfaces permiten configurarlos.

**Distinción clave:** reducir variación no demuestra veracidad ni determinismo completo.**

### 19.2. Reproducibilidad

La **reproducibilidad** permite reconstruir un procedimiento y revisar sus condiciones.

- Necesita versiones identificadas.
- Conserva entradas y configuración conocida.
- Declara factores desconocidos.

En sistemas generativos, repetir el procedimiento puede producir variaciones.

**Distinción clave:** reproducir condiciones no garantiza una respuesta idéntica.**

### 19.3. Latencia

La **latencia** es el tiempo asociado a obtener un resultado.

- Puede medirse hasta el primer contenido.
- Puede medirse hasta la respuesta completa.
- Puede incluir herramientas y etapas adicionales.

La unidad de medición debe declararse.

**Distinción clave:** respuesta rápida no equivale a proceso completo más eficiente.**

### 19.4. Eficiencia del proceso

La **eficiencia** relaciona resultados útiles con recursos y esfuerzo utilizados.

- Incluye preparación de entradas.
- Incluye revisión y corrección.
- Incluye mantenimiento pertinente.

La comparación necesita un punto de partida definido.

**Distinción clave:** ahorrar generación no demuestra ahorrar trabajo total.**

---

## 20. Sesiones prácticas de vocabulario

Las sesiones aplican los conceptos a situaciones sintéticas y producen materiales revisables.

### 20.1. Sesión de treinta minutos · Identificación de conceptos

La sesión comprueba que el grupo distingue objetos y operaciones.

- Cinco minutos: lectura de términos seleccionados.
- Diez minutos: identificación en un caso sintético.
- Diez minutos: contraste por parejas.
- Cinco minutos: corrección y cierre.

Caso docente:

```text
Un equipo prepara una plantilla con {{solicitud}}.
Completa el marcador con un mensaje sintético.
Ejecuta la versión v1 y conserva una respuesta.
Después modifica una restricción y crea v2.
```

El entregable identifica plantilla, marcador, prompt completado, ejecución y versión.

**Referencia docente:** modificar contenido y repetir una ejecución son operaciones distintas.

### 20.2. Sesión de sesenta minutos · Fuente, estado y evidencia

La sesión utiliza un extractor sencillo de requisitos.

- Diez minutos: tarea y política.
- Diez minutos: referencia previa.
- Quince minutos: preparación y ejecución.
- Quince minutos: revisión.
- Diez minutos: vocabulario y pendientes.

Entrada sintética:

```text
Participarán aproximadamente 12 personas.
La duración será de dos horas.
Proponemos el 18 de noviembre de 2026.
La fecha todavía no está confirmada.
```

Se esperan aproximación conservada, 120 minutos y fecha propuesta.

**El entregable separa referencia docente, respuesta observada y criterio de aceptación.**

### 20.3. Sesión de noventa minutos · Comparación y regresión

La sesión relaciona vocabulario con decisiones de mejora.

- Quince minutos: línea base y referencias.
- Quince minutos: ejecución inicial.
- Quince minutos: hipótesis y nueva versión.
- Treinta minutos: comparación y regresión.
- Quince minutos: documentación y cierre.

El grupo utiliza un caso normal, uno ausente y uno contradictorio.

El cambio debe responder a una discrepancia localizada.

Las condiciones diferentes del entorno deben declararse.

**El entregable distingue observación, hipótesis, efecto esperado y resultado comprobado.**

### 20.4. Revisión cruzada y síntesis

Otra pareja revisa los materiales sin explicaciones continuas del autor.

- Localiza las versiones y las entradas.
- Comprueba el uso de términos.
- Identifica evidencias y pendientes.
- Reconstruye una decisión.

Consulta [Plantillas](../plantillas/index.md) para organizar los registros.

Relaciona los conceptos con los requisitos del [Proyecto final](../proyecto-final/index.md).

**Utilizar bien el glosario significa describir con precisión qué se diseñó, qué se observó y qué permiten concluir las evidencias.**