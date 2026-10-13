# Descomposición y verificación

Descomponer una tarea consiste en dividirla en operaciones más pequeñas, con entradas y resultados reconocibles.

Verificar consiste en comprobar esos resultados mediante criterios, fuentes y procedimientos adecuados.

Ambas prácticas permiten diseñar interacciones con modelos de lenguaje que sean más fáciles de revisar.

No garantizan que desaparezcan los errores.

Sí pueden ayudar a localizar dónde aparecen, evitar que pasen inadvertidos y decidir qué hacer antes de continuar.

Esta unidad desarrolla una metodología para separar extracción, cálculo, interpretación y redacción.

También distingue la revisión realizada por un modelo de la comprobación apoyada en evidencia independiente.

El objetivo es producir resultados útiles sin confundir una explicación convincente con una validación.

**Una tarea bien descompuesta permite inspeccionar sus resultados intermedios y detener el proceso cuando falta información o aparece un error relevante.**

!!! info "Alcance de esta documentación"
    La sesión lectiva dura una hora.
    Esta página incluye fundamentos, un laboratorio obligatorio y ampliaciones.
    Durante la sesión se completa únicamente el recorrido señalado en la agenda.
    Las actividades adicionales sirven como consulta o práctica posterior.

## 1. Fundamentos de la descomposición y la verificación

Esta sección establece qué significa dividir una tarea y cómo seleccionar comprobaciones que aporten evidencia.

La finalidad no es crear más pasos por costumbre, sino organizar el trabajo de forma que pueda revisarse.

### 1.1. Ficha de la unidad

La unidad pertenece al segundo día del curso.

| Elemento | Descripción |
|---|---|
| Jornada | Día 2 · Técnicas y formatos |
| Unidad | Descomposición y verificación |
| Duración lectiva | 1 hora |
| Modalidad | Explicación, demostración y práctica |
| Resultado | Flujo breve con comprobaciones documentadas |

Se requiere familiaridad con la anatomía del prompt.

No se requiere programación.

Una interfaz conversacional autorizada es suficiente para las actividades obligatorias.

Las operaciones numéricas se comprobarán con una calculadora o por un procedimiento independiente.

Los datos utilizados son ficticios.

**La evaluación reconoce el diseño del proceso y la calidad de sus comprobaciones.**

### 1.2. Objetivos de aprendizaje

Los objetivos describen acciones que podrás demostrar al terminar.

Al finalizar podrás:

- Identificar operaciones distintas dentro de una solicitud.
- Dividir una tarea en subtareas con resultados observables.
- Definir entradas y salidas para cada etapa.
- Establecer condiciones para continuar o detenerse.
- Comprobar fidelidad a una fuente.
- Revisar operaciones numéricas sencillas.
- Distinguir datos, cálculos, hipótesis y recomendaciones.
- Documentar errores y limitaciones.

No se exige obtener una salida perfecta en todos los casos.

Se exige reconocer qué puedes verificar y qué queda pendiente.

**Una limitación bien identificada forma parte de un resultado útil.**

### 1.3. Qué es descomponer una tarea

Descomponer significa separar un trabajo en operaciones con funciones diferentes.

Cada operación debe tener un propósito reconocible.

También debe producir un resultado que otra etapa pueda utilizar.

Una solicitud amplia puede contener varias tareas:

- Localizar información.
- Extraer datos.
- Resolver contradicciones.
- Calcular indicadores.
- Interpretar resultados.
- Redactar una síntesis.

Estas operaciones no necesitan ejecutarse siempre por separado.

La separación resulta útil cuando facilita la comprobación.

**El criterio principal es la revisabilidad, no el número de etapas.**

### 1.4. Descomposición funcional

La descomposición funcional divide el trabajo según el tipo de operación.

Es una forma útil de comenzar.

Por ejemplo:

```text
Tarea general:
Preparar un resumen de resultados.

Descomposición:
1. Extraer los datos relevantes.
2. Comprobar su correspondencia con la fuente.
3. Calcular los indicadores solicitados.
4. Redactar el resumen con los datos verificados.
```

Cada etapa aplica criterios distintos.

La extracción se comprueba contra el documento.

El cálculo se comprueba mediante operaciones.

La redacción se comprueba por fidelidad, utilidad y formato.

**Separar funciones evita evaluar todo con una impresión general.**

### 1.5. Descomposición por documentos o fragmentos

Otra posibilidad es dividir el material de entrada.

Puede ser útil cuando hay varios documentos o secciones extensas.

Cada fragmento debe conservar suficiente contexto.

No conviene separar una cifra de su unidad o de su encabezado.

Tampoco conviene perder una nota que modifica su interpretación.

Antes de dividir, identifica:

- Límites de secciones.
- Relaciones entre tablas.
- Definiciones compartidas.
- Fechas y periodos.
- Excepciones.

Después será necesario integrar los resultados.

**Fragmentar información puede facilitar el procesamiento y también introducir pérdidas de contexto.**

### 1.6. Descomposición por decisiones

Algunas tareas requieren tomar decisiones sucesivas.

La siguiente acción depende del resultado anterior.

Ejemplo:

```text
Si la fecha está confirmada:
Inclúyela en la ficha.

Si la fecha es una propuesta:
Conserva ese estado.

Si aparecen dos fechas incompatibles:
Señala el conflicto y solicita confirmación.
```

Esta estructura evita tratar todos los casos de la misma manera.

Las condiciones deben ser explícitas.

También debe estar definido qué hacer con una entrada no prevista.

**Una bifurcación útil describe tanto el criterio como la acción resultante.**

### 1.7. Qué es verificar

Verificar es comprobar una afirmación o un resultado frente a una referencia adecuada.

No consiste solamente en pedir otra respuesta.

Una verificación puede utilizar:

- El documento original.
- Una operación independiente.
- Una regla de clasificación.
- Un esquema de datos.
- Una prueba de funcionamiento.
- Una revisión humana autorizada.

El método depende del requisito.

No todo puede comprobarse con el mismo procedimiento.

La referencia también puede contener errores.

**Verificar exige identificar qué se comprueba y con qué evidencia.**

### 1.8. Validación estructural y verificación de contenido

Una salida puede ser correcta en su estructura y equivocada en sus valores.

También puede contener información correcta en un formato inutilizable.

En esta unidad distinguiremos dos comprobaciones.

| Comprobación | Pregunta |
|---|---|
| Estructural | ¿La salida tiene los campos y tipos requeridos? |
| De contenido | ¿Los valores y afirmaciones son correctos? |
| De alcance | ¿Se limita al trabajo autorizado? |
| De utilidad | ¿Sirve al destinatario previsto? |

Esta distinción es operativa.

La terminología puede variar en otros contextos.

Lo importante es no sustituir una comprobación por otra.

**Un JSON válido no demuestra que sus cifras sean verdaderas.**

### 1.9. Datos, cálculos e interpretaciones

Estos elementos requieren controles diferentes.

Un dato debe localizarse en una fuente.

Un cálculo debe utilizar datos adecuados y una operación correcta.

Una interpretación debe respetar lo que la evidencia permite concluir.

Ejemplo:

```text
Dato:
Se resolvieron 110 solicitudes de 120 recibidas.

Cálculo:
110 dividido entre 120, multiplicado por 100.

Interpretación limitada:
Se resolvió aproximadamente el 91,67 % de las solicitudes recibidas.
```

No puede deducirse automáticamente satisfacción o productividad.

**Una operación correcta no autoriza cualquier conclusión.**

### 1.10. Hechos, hipótesis y recomendaciones

La redacción debe distinguir categorías de afirmaciones.

Un hecho está respaldado por la fuente disponible.

Una hipótesis propone una explicación pendiente de contraste.

Una recomendación propone una acción.

Podemos pedir que aparezcan en secciones separadas.

Pero debemos revisar si la clasificación es adecuada.

Una frase prudente no convierte una hipótesis en un hecho.

Una recomendación puede ser razonable sin estar demostrada.

El destinatario debe conocer esa diferencia.

En tareas de alto impacto, puede requerirse revisión especializada.

**La separación evita que una propuesta se interprete como un resultado confirmado.**

### 1.11. Revisión del propio modelo

Un modelo puede revisar una respuesta que ha generado.

Esa revisión puede detectar ciertos errores.

También puede repetirlos o justificar una salida incorrecta.

No debemos tratarla como validación independiente.

La revisión mejora cuando recibe:

- Criterios explícitos.
- Fuente original.
- Campos que comprobar.
- Instrucciones para señalar discrepancias.
- Un formato de incidencias.

Incluso con esos elementos, sigue necesitando evaluación.

Una respuesta que dice “todo correcto” no aporta evidencia suficiente.

**La autorrevisión es una ayuda, no una garantía.**

### 1.12. Revisión con otro modelo

Otro modelo puede aportar una perspectiva diferente.

También puede compartir errores con el primero.

La coincidencia entre respuestas no demuestra verdad.

Los sistemas pueden haber aprendido patrones similares.

Además, ambos pueden recibir la misma información equivocada.

Para obtener una comprobación útil, proporciona:

- Fuente.
- Requisitos.
- Resultado que revisar.
- Método esperado.
- Límites de la revisión.

No uses una votación como sustituto de evidencia.

**El acuerdo entre modelos debe contrastarse con referencias adecuadas.**

### 1.13. Explicación verificable y razonamiento interno

No necesitamos acceder al razonamiento interno detallado para comprobar muchos resultados.

Podemos solicitar una justificación breve y observable.

Por ejemplo:

- Datos utilizados.
- Operación aplicada.
- Fragmento de evidencia.
- Supuesto relevante.
- Condición de validez.

Una explicación extensa puede contener errores.

También puede presentar una justificación que no refleja de forma fiable el proceso interno.

Prioriza soportes que otra persona pueda contrastar.

No pidas una narración exhaustiva como prueba de rigor.

**La verificabilidad depende de evidencia y operaciones comprobables.**

### 1.14. Cuándo compensa descomponer

La descomposición puede resultar útil cuando hay varias operaciones diferentes.

También cuando un error inicial puede afectar a todo el resultado.

Señales para considerarla:

- Varias fuentes.
- Cálculos derivados.
- Requisitos contradictorios.
- Campos obligatorios.
- Consecuencias operativas.
- Necesidad de trazabilidad.
- Integración con otras herramientas.

Una tarea sencilla puede resolverse en una sola interacción.

Separarla demasiado puede aumentar coste y complejidad.

**Descompón cuando el beneficio de control justifique el trabajo adicional.**

### 1.15. Riesgos de dividir demasiado

Cada etapa introduce una nueva transferencia de información.

Esa transferencia puede perder detalles.

También puede introducir cambios de formato o significado.

Riesgos frecuentes:

- Copiar una cifra incorrectamente.
- Omitir una condición.
- Cambiar una unidad.
- Perder un identificador.
- Utilizar una versión desactualizada.
- Duplicar registros.

El número de etapas no equivale a calidad.

Conviene mantener resultados compactos y completos.

Las transferencias necesitan comprobación.

**Más pasos pueden significar más puntos de fallo.**

### 1.16. Principio de continuidad condicionada

Una etapa no debería continuar automáticamente si falta un requisito crítico.

Define una condición de paso.

Ejemplo:

```text
Continuar:
Los datos necesarios están presentes y no hay contradicciones críticas.

Detener:
Falta el denominador del indicador solicitado.

Resultado al detener:
Indicar qué dato falta y no calcular el porcentaje.
```

La detención puede afectar solo a una parte del trabajo.

Las operaciones no afectadas pueden continuar si es seguro.

**Saber detenerse es una capacidad del diseño.**

---

## 2. Diseño de flujos: entradas, salidas y puntos de control

Esta sección convierte los fundamentos en una estructura de trabajo reutilizable.

El objetivo es que cada etapa tenga un contrato claro y una comprobación proporcionada.

### 2.1. Definir la tarea completa

Antes de dividir, describe el resultado final.

No empieces enumerando pasos sin conocer el propósito.

Completa:

```text
Necesito obtener:
La persona destinataria es:
El resultado se utilizará para:
Las fuentes disponibles son:
Un error relevante sería:
```

Estas respuestas ayudan a decidir dónde verificar.

También permiten excluir operaciones innecesarias.

No toda la reflexión debe enviarse al modelo.

Puede mantenerse en la ficha de diseño.

**La descomposición debe servir al resultado final.**

### 2.2. Dibujar un mapa de etapas

Utiliza un esquema sencillo.

No necesitas una herramienta de diagramación.

Ejemplo:

```text
Documento original
      ↓
Extracción
      ↓
Comprobación de datos
      ↓
Cálculo verificado
      ↓
Síntesis
      ↓
Revisión final
```

Añade rutas de detención si son necesarias.

Identifica qué etapas pueden realizarse sin el modelo.

**El mapa representa el flujo de trabajo, no el razonamiento interno del sistema.**

### 2.3. Definir un contrato por etapa

Un contrato describe qué recibe y qué produce una etapa.

También establece límites.

Utiliza estos campos:

- Nombre.
- Propósito.
- Entrada.
- Salida.
- Restricciones.
- Criterios de aceptación.
- Acción ante fallo.

El contrato puede documentarse en una tabla.

No necesita convertirse en un formato técnico complejo.

Su utilidad está en evitar expectativas implícitas.

Comprueba que la salida anterior sea compatible con la entrada siguiente.

**Las conexiones entre etapas también forman parte del diseño.**

### 2.4. Contrato de extracción

La extracción recupera información de una fuente.

No debe añadir análisis no solicitado.

Ejemplo:

```text
Entrada:
Informe original.

Salida:
Tabla de indicadores, valores, unidades y evidencia.

Restricción:
No completar datos ausentes.

Aceptación:
Cada valor coincide con un fragmento de la fuente.

Ante fallo:
Señalar el campo y detener los cálculos que dependan de él.
```

La evidencia puede ser un fragmento breve.

No necesita reproducir todo el documento.

**La extracción debe conservar significado y procedencia.**

### 2.5. Contrato de cálculo

El cálculo utiliza datos previamente revisados.

Debe identificar la operación y la base.

Ejemplo:

```text
Entrada:
Valores confirmados de recibidas y resueltas.

Salida:
Proporción de solicitudes resueltas.

Aceptación:
Datos adecuados, operación correcta y redondeo definido.

Ante fallo:
No publicar el indicador.
```

La calculadora comprueba la operación.

La persona revisora comprueba la interpretación de los datos.

Son controles distintos.

**No calcules con valores que siguen en conflicto.**

### 2.6. Contrato de interpretación

La interpretación relaciona resultados con el propósito.

Debe limitarse a lo que la evidencia permite.

Entrada:

- Datos revisados.
- Indicadores comprobados.
- Contexto autorizado.

Salida:

- Hallazgos.
- Limitaciones.
- Hipótesis identificadas, si se permiten.

La aceptación requiere revisar inferencias.

No basta con que el texto resulte coherente.

Una tendencia no demuestra una causa.

Un indicador aislado no describe todo el desempeño.

**La interpretación debe conservar las condiciones de validez.**

### 2.7. Contrato de redacción

La redacción transforma material revisado en una salida útil.

Debe respetar el contenido disponible.

Puede adaptar:

- Orden.
- Extensión.
- Vocabulario.
- Encabezados.
- Presentación.

No debe cambiar:

- Cifras.
- Unidades.
- Estados.
- Periodos.
- Grado de certeza.

**La adaptación expresiva no autoriza alterar hechos.**

### 2.8. Comprobaciones automáticas y humanas

Algunas propiedades pueden comprobarse con reglas simples.

Otras requieren interpretación.

| Tipo de comprobación | Ejemplo |
|---|---|
| Sintaxis | El JSON puede analizarse |
| Tipos | Participantes es un entero |
| Regla numérica | Resueltas no supera recibidas bajo la definición acordada |
| Fidelidad | El dato corresponde a la fuente |
| Utilidad | La síntesis sirve a la reunión |

Una regla numérica necesita una definición válida.

En algunos procesos pueden resolverse solicitudes de periodos anteriores.

No impongas una igualdad sin revisar el contexto.

**Las validaciones deben reflejar el significado real de los datos.**

### 2.9. Comprobar unidades

Una cifra aislada es insuficiente.

Debe conservar su unidad.

Ejemplos de unidades relevantes:

- Horas.
- Minutos.
- Euros.
- Personas.
- Solicitudes.
- Porcentaje.

También debe conservar su periodo.

Seis horas de primera respuesta no son seis horas de resolución.

Una conversión necesita una operación explícita.

No cambies una unidad solo para uniformar la tabla.

**El valor, la unidad y el concepto deben revisarse juntos.**

### 2.10. Comprobar denominadores

Muchos errores de porcentaje proceden de una base incorrecta.

Antes de calcular, pregunta:

- ¿Qué representa el numerador?
- ¿Qué representa el denominador?
- ¿Pertenecen al mismo periodo?
- ¿Describen la misma población?
- ¿Se permiten comparaciones directas?

No uses el total más cercano por comodidad.

Una proporción debe tener una definición.

La interpretación depende de esa definición.

Si falta el denominador, señala la ausencia.

No inventes una base de comparación.

**Un porcentaje sin base identificada es difícil de verificar.**

### 2.11. Definir redondeo y precisión

El redondeo afecta a la presentación.

Conviene establecerlo cuando hay indicadores.

Ejemplo:

```text
Presenta porcentajes con dos decimales.
Conserva los valores originales para la comprobación.
```

No confundas precisión de presentación con exactitud de datos.

Dos decimales no demuestran una medición precisa.

Si el dato original es una estimación, conserva esa condición.

Los porcentajes redondeados pueden no sumar exactamente cien.

No corrijas cifras arbitrariamente para forzar una suma.

**El redondeo debe ser coherente y documentado.**

### 2.12. Trazabilidad de resultados

La trazabilidad permite relacionar una afirmación con su origen.

Utiliza identificadores sencillos.

Por ejemplo:

- D01: documento.
- E01: extracción.
- C01: cálculo.
- S01: síntesis.
- F01: fallo.

No necesitas numerar cada palabra.

Sí conviene identificar resultados relevantes.

Guarda la fuente original.

Relaciona versiones cuando haya cambios.

No reutilices un identificador para contenidos distintos.

**La trazabilidad facilita revisar y corregir sin reconstruir todo el proceso.**

### 2.13. Gestión de errores

Un fallo debe tener una respuesta definida.

Posibles acciones:

- Corregir.
- Repetir.
- Pedir información.
- Excluir un indicador.
- Detener una etapa.
- Escalar a revisión especializada.

La acción depende del impacto.

No reintentes indefinidamente sin cambiar condiciones.

Un nuevo intento puede repetir el mismo problema.

Establece un límite razonable para la práctica.

Documenta qué sigue pendiente.

**Gestionar un error no significa ocultarlo en una nueva respuesta.**

### 2.14. Evitar propagación de errores

Un resultado intermedio equivocado puede contaminar las etapas posteriores.

La redacción puede hacer el error más convincente.

Introduce controles antes de operaciones dependientes.

Ejemplo:

```text
Dato no verificado:
Tiempo medio de resolución: 6 horas.

Riesgo:
Calcular una mejora de resolución inexistente.

Control:
Comparar el nombre del indicador con la fuente antes de calcular.
```

El control debe comprobar significado, no solo cifra.

No copies automáticamente todas las salidas a la siguiente etapa.

**La verificación temprana puede evitar correcciones más costosas.**

### 2.15. Una interacción o varias

La descomposición puede expresarse en una sola solicitud.

También puede ejecutarse mediante varias interacciones.

Una sola solicitud puede ser suficiente para tareas pequeñas.

Varias interacciones permiten inspeccionar resultados antes de continuar.

Pero añaden transferencias y tiempo.

Elige según:

- Complejidad.
- Riesgo.
- Necesidad de intervención.
- Herramientas.
- Coste.
- Facilidad de revisión.

No asumas que varias llamadas son siempre superiores.

**La arquitectura del flujo también debe evaluarse.**

### 2.16. Plantilla general de flujo

Utiliza esta ficha como punto de partida.

Adáptala al caso.

```text
TAREA FINAL
[Resultado y destinatario]

ETAPAS
[Nombre, entrada y salida de cada una]

VERIFICACIONES
[Referencia y método por etapa]

CONDICIONES DE CONTINUIDAD
[Qué debe cumplirse antes de avanzar]

GESTIÓN DE FALLOS
[Qué corregir, detener o escalar]

EVIDENCIAS
[Archivos y versiones que se conservarán]
```

---

## 3. Laboratorio obligatorio: extraer, calcular y sintetizar

La práctica principal utiliza un informe sintético de operaciones.

El objetivo es comparar una solicitud integrada con un flujo descompuesto y documentar las comprobaciones.

### 3.1. Agenda de la hora

La sesión incluye una demostración y una práctica breve.

Las ampliaciones quedan fuera del recorrido obligatorio.

| Minutos | Actividad | Evidencia |
|---|---|---|
| 00–10 | Fundamentos y demostración | Mapa inicial |
| 10–18 | Solicitud integrada | Línea base |
| 18–30 | Extracción y comprobación | Tabla verificada |
| 30–40 | Cálculo independiente | Indicadores |
| 40–50 | Síntesis y revisión | Resultado final |
| 50–60 | Comparación y entrega | Conclusión |

No buscamos medir fiabilidad general.

La comparación ofrece observaciones sobre un caso.

Una respuesta integrada puede cumplir perfectamente.

El flujo descompuesto también puede fallar.

**La conclusión debe respetar esas posibilidades.**

### 3.2. Situación de trabajo

Trabajas en un equipo ficticio de operaciones.

Una responsable necesita preparar una reunión.

Dispones de un informe breve.

Debes producir:

- Un resumen.
- La proporción de solicitudes resueltas.
- El cambio en primera respuesta.
- Una lista de datos pendientes.

No tienes otras fuentes.

No debes recomendar contratación.

No debes explicar causas no documentadas.

La reunión necesita distinguir resultados y limitaciones.

**El propósito es informar, no decidir una reorganización.**

### 3.3. Documento de entrada

Utiliza este informe completo.

```text
INFORME SINTÉTICO DE OPERACIONES
Periodo: primer trimestre

Se recibieron 120 solicitudes:
- 60 consultas de información.
- 40 incidencias técnicas.
- 20 sugerencias.

De las 120 solicitudes recibidas en este trimestre,
se resolvieron 110 durante el periodo.
Diez quedaron pendientes al cierre.

El tiempo medio de primera respuesta fue de 6 horas.
En el trimestre anterior había sido de 8 horas.

No se dispone de datos de satisfacción ni de costes operativos.
Se propone analizar las causas de las solicitudes pendientes.
```

La definición de la población está indicada.

### 3.4. Preparación de la referencia

Antes de ejecutar, revisa manualmente el informe.

Anota los valores esperados.

Son:

- Recibidas: 120.
- Resueltas: 110.
- Pendientes: 10.
- Primera respuesta actual: 6 horas.
- Primera respuesta anterior: 8 horas.

Las categorías suman 120.

Resueltas y pendientes corresponden a las recibidas del trimestre.

No hay datos de satisfacción.

No hay costes.

No se conocen causas.

**Esta referencia humana no debe modificarse para coincidir con la respuesta del modelo.**

### 3.5. Solicitud integrada

Ejecuta esta primera condición.

```text
Prepara una síntesis del informe para una responsable de operaciones.

Incluye:
- Resultados principales.
- Porcentaje de solicitudes resueltas.
- Cambio absoluto y relativo de primera respuesta.
- Datos pendientes.
- Próximo paso propuesto.

Utiliza únicamente el informe.
No atribuyas causas ni resultados no documentados.
Presenta porcentajes con dos decimales.

INFORME
[Inserta aquí el informe completo]
```

Sustituye el marcador antes de enviar.

### 3.6. Guardar la línea base

Conserva la respuesta completa.

No la corrijas antes de registrarla.

Anota:

```text
Condición: integrada
Fecha:
Modelo visible:
Conversación nueva:

Cifras correctas:
Cifras incorrectas:
Confusiones de significado:
Información añadida:
Aspectos no comprobados:
```

La revisión puede realizarse al final.

No necesitas repetir la solicitud si aparece un fallo.

El fallo forma parte de la evidencia.

**La línea base no tiene que ser mala para que la comparación sea útil.**

### 3.7. Etapa 1: extracción

Abre otra conversación cuando sea posible.

Utiliza este prompt.

```text
Extrae los datos necesarios para analizar el informe.

Devuelve una tabla con:
- Indicador.
- Valor.
- Unidad.
- Periodo o población.
- Evidencia breve.

Incluye recibidas, resueltas, pendientes,
primera respuesta actual y primera respuesta anterior.

No calcules porcentajes.
No interpretes causas.
Indica los datos no disponibles.

INFORME
[Inserta aquí el informe completo]
```

Guarda la salida como extracción inicial.

### 3.8. Verificar la extracción

Compara cada fila con la fuente.

No continúes automáticamente.

Comprueba:

- Valor.
- Unidad.
- Nombre del indicador.
- Periodo.
- Población.
- Evidencia.

La extracción debe hablar de primera respuesta.

Debe conservar el trimestre correspondiente.

Si un valor es incorrecto, corrígelo en una copia identificada.

Mantén la salida original.

Registra quién realizó la corrección.

**La tabla corregida no debe confundirse con la generación original.**

### 3.9. Tabla de referencia

Esta tabla muestra los datos que deben quedar verificados.

No constituye una ejecución del modelo.

| Indicador | Valor | Unidad | Condición |
|---|---:|---|---|
| Recibidas | 120 | Solicitudes | Trimestre actual |
| Resueltas | 110 | Solicitudes | De las recibidas en el trimestre |
| Pendientes | 10 | Solicitudes | Al cierre |
| Primera respuesta actual | 6 | Horas | Trimestre actual |
| Primera respuesta anterior | 8 | Horas | Trimestre anterior |

La fuente no aporta satisfacción.

Tampoco costes.

Esas ausencias deben permanecer visibles.

**La tabla reúne valores y significado.**

### 3.10. Etapa 2: definir operaciones

Antes de calcular, define las operaciones.

Utiliza esta ficha.

```text
Proporción resuelta:
Numerador: 110 solicitudes resueltas.
Denominador: 120 solicitudes recibidas.

Cambio absoluto de primera respuesta:
Valor anterior menos valor actual.

Reducción relativa:
Cambio absoluto dividido entre valor anterior.

Presentación:
Porcentajes con dos decimales.
```

La base de la reducción es 8 horas.

No es 6.

El cambio describe primera respuesta.

**Definir la operación ayuda a detectar errores antes de ejecutarla.**

### 3.11. Etapa 2: cálculo independiente

Realiza las operaciones con una calculadora.

También puedes comprobarlas manualmente.

Resultados de referencia:

```text
Proporción resuelta:
110 / 120 × 100 = 91,666...

Presentación:
91,67 %

Disminución absoluta:
8 - 6 = 2 horas

Disminución relativa:
2 / 8 × 100 = 25 %
```

No utilices la calculadora para decidir el significado del indicador.

Esa revisión corresponde a la definición de datos.

### 3.12. Comprobar interpretación de cálculos

Los resultados admiten conclusiones limitadas.

Podemos afirmar:

- Se resolvió aproximadamente el 91,67 % de las solicitudes recibidas.
- La primera respuesta media disminuyó 2 horas.
- La disminución relativa fue del 25 % respecto al trimestre anterior.

No podemos afirmar automáticamente:

- La satisfacción aumentó.
- Los costes disminuyeron.
- La productividad mejoró un 25 %.
- La resolución fue más rápida.
- Los pendientes se deben a falta de personal.

Revisa que la redacción no sustituya un concepto por otro.

La mejora de un indicador no describe todo el servicio.

**Interpretar exige conservar límites de evidencia.**

### 3.13. Etapa 3: preparar la síntesis

Utiliza únicamente los datos revisados.

Añade las ausencias del documento.

Prompt:

```text
Redacta una síntesis para una responsable de operaciones.

Utiliza únicamente los datos verificados incluidos abajo.
No añadas causas, satisfacción, costes ni compromisos.
Conserva el significado de primera respuesta.

Presenta:
- Resumen de hasta 120 palabras.
- Tres hallazgos.
- Datos pendientes.
- Próximo paso propuesto en el informe.

DATOS VERIFICADOS
[Inserta la tabla y los cálculos revisados]

LIMITACIONES Y PROPUESTA
[Inserta las ausencias y el próximo paso de la fuente]
```

### 3.14. Revisar la síntesis

La revisión final comprueba que no se hayan introducido nuevos errores.

Busca:

- Cifras cambiadas.
- Unidades omitidas.
- Indicadores renombrados.
- Porcentajes alterados.
- Causas inventadas.
- Recomendaciones no autorizadas.

Comprueba también el formato.

Si el límite de palabras es estricto, cuéntalas.

No asumas cumplimiento por apariencia.

La redacción puede omitir información esencial.

Puede añadir una conclusión excesiva.

Conserva el resultado original antes de corregir.

**Los datos verificados pueden deteriorarse durante la síntesis.**

### 3.15. Comparar las dos condiciones

Compara la solicitud integrada y el flujo descompuesto.

Utiliza criterios comunes.

| Criterio | Integrada | Descompuesta |
|---|---|---|
| Fidelidad | Registrar | Registrar |
| Cálculos | Registrar | Registrar |
| Significado | Registrar | Registrar |
| Ausencias | Registrar | Registrar |
| Facilidad de revisión | Registrar | Registrar |

No compares solo estilo.

Registra también trabajo adicional.

Si ambas cumplen, indica empate en contenido.

La descomposición puede facilitar trazabilidad sin mejorar exactitud en este caso.

**Describe beneficios y costes observados.**

### 3.16. Conclusión de la sesión

Cierra el laboratorio con una reflexión breve.

Utiliza esta estructura.

```text
En la condición integrada observé:

En la condición descompuesta observé:

La verificación que aportó más valor fue:

El trabajo adicional consistió en:

No puedo concluir todavía:

Para esta tarea utilizaría:

La siguiente prueba sería:
```

La decisión puede favorecer cualquiera de las condiciones.

**La elección debe responder al caso y a sus evidencias.**

---

## 4. Ampliaciones, evaluación y reutilización

Esta sección desarrolla casos adicionales y organiza el entregable.

Las ampliaciones permiten practicar condiciones que el laboratorio principal no cubre.

### 4.1. Ampliación: informe contradictorio

Utiliza esta fuente sintética.

```text
Resumen:
Se recibieron 100 solicitudes.
Se resolvieron 90.

Tabla de cierre:
Recibidas: 120.
Resueltas: 95.

No se indica qué versión es definitiva.
```

No hay una base inequívoca para un único porcentaje.

Descompón extracción y resolución del conflicto.

La salida debe conservar ambos conjuntos.

No elijas uno por estar en una tabla.

**Una fuente contradictoria puede impedir calcular un indicador confirmado.**

### 4.2. Verificación de contradicciones

Diseña una ficha de incidencias.

Incluye:

- Campo.
- Valores encontrados.
- Ubicación.
- Impacto.
- Información requerida.

El indicador de resolución queda pendiente.

Puedes mostrar cálculos condicionales si la tarea lo permite.

Deben identificarse como escenarios.

No los presentes como resultado confirmado.

La primera acción será solicitar la versión válida.

El resto del documento puede procesarse si no depende del conflicto.

**La detención debe relacionarse con la dependencia afectada.**

### 4.3. Ampliación: denominador ausente

Utiliza esta entrada.

```text
Durante el periodo se resolvieron 75 solicitudes.

No se indica cuántas solicitudes se recibieron.
Tampoco se indica si las resueltas pertenecen al mismo periodo.
```

Solicita una proporción de resolución.

La respuesta correcta debe reconocer que falta información.

No debe usar 75 como denominador.

No debe inferir el total.

La salida puede listar los datos necesarios.

La verificación consiste en revisar ausencia y población.

**No todos los indicadores solicitados pueden calcularse con los datos disponibles.**

### 4.4. Ampliación: conversión de unidades

Utiliza esta fuente.

```text
Periodo anterior:
Primera respuesta media de 120 minutos.

Periodo actual:
Primera respuesta media de 1,5 horas.
```

Primero normaliza unidades.

120 minutos equivalen a 2 horas.

La disminución es de 0,5 horas.

Equivale a 30 minutos.

La reducción relativa es del 25 %.

Comprueba conversión y base por separado.

**Una comparación requiere unidades compatibles.**

### 4.5. Ampliación: acciones de reunión

Utiliza estas notas ficticias.

```text
Sara enviará el borrador el 12 de noviembre.
El equipo revisará los indicadores.

No se ha asignado quién actualizará la plantilla.
La siguiente reunión será el 20 de noviembre.

No se ha fijado una fecha límite para revisar indicadores.
```

Descompón:

1. Extraer acciones.
2. Revisar responsables y fechas.
3. Preparar una tabla final.

No conviertas la reunión en fecha límite.

**La extracción debe conservar compromisos explícitos.**

### 4.6. Verificar acciones y responsables

La tabla debe distinguir datos ausentes.

Campos recomendados:

- Acción.
- Responsable.
- Fecha.
- Estado.
- Evidencia.

Sara aparece vinculada al borrador.

El equipo aparece vinculado a indicadores.

La plantilla queda sin responsable.

La revisión de indicadores queda sin fecha límite.

No asignes funciones por plausibilidad.

La tabla requiere revisión antes de distribuirse.

**Organizar trabajo no autoriza crear compromisos.**

### 4.7. Ampliación: datos estructurados

La descomposición también puede aplicarse a JSON.

Define primero el esquema.

Ejemplo:

```json
{
  "recibidas": 120,
  "resueltas": 110,
  "pendientes": 10
}
```

Comprueba sintaxis antes de usar valores.

Después comprueba tipos.

Después comprueba correspondencia con la fuente.

Finalmente aplica reglas semánticas justificadas.

No confundas análisis sintáctico con verificación factual.

**La validación debe cubrir varias capas.**

### 4.8. Comprobación opcional con Python

Esta práctica técnica no es obligatoria.

El código usa únicamente datos locales ficticios.

```python
datos = {
    "recibidas": 120,
    "resueltas": 110,
    "pendientes": 10,
}

campos = ("recibidas", "resueltas", "pendientes")

for campo in campos:
    valor = datos[campo]
    if type(valor) is not int or valor < 0:
        raise ValueError(f"Valor inválido en {campo}")

if datos["resueltas"] + datos["pendientes"] != datos["recibidas"]:
    raise ValueError("La suma no coincide con las recibidas")
```

La igualdad solo es válida bajo la definición del laboratorio.

### 4.9. Límites de las reglas automáticas

Una regla puede funcionar en el ejemplo y ser incorrecta en otro proceso.

Por ejemplo, pueden resolverse solicitudes antiguas.

También pueden existir cancelaciones.

La suma de resueltas y pendientes puede necesitar otras categorías.

Antes de automatizar, define:

- Población.
- Periodo.
- Estados.
- Exclusiones.
- Reglas de transición.

La programación no elimina esa necesidad.

Un control incorrecto puede rechazar datos válidos.

**La semántica precede a la automatización.**

### 4.10. Entregable de la unidad

Entrega un documento con el laboratorio principal.

Debe incluir:

1. Ficha del entorno.
2. Tarea final.
3. Mapa de etapas.
4. Fuente utilizada.
5. Respuesta integrada.
6. Extracción original.
7. Comprobaciones y correcciones.
8. Operaciones verificadas.
9. Síntesis final.
10. Comparación.
11. Limitaciones.

Las ampliaciones pueden añadirse como anexos.

**No entregues únicamente la síntesis final.**

### 4.11. Checklist de comprobación

Revisa antes de entregar.

Marca solo lo que puedas demostrar.

- [ ] La tarea está delimitada.
- [ ] Las etapas tienen entradas y salidas.
- [ ] Los datos conservan unidades.
- [ ] Los periodos están identificados.
- [ ] Los denominadores están justificados.
- [ ] Los cálculos se comprobaron independientemente.
- [ ] Los errores originales están guardados.
- [ ] Las correcciones están identificadas.
- [ ] La síntesis no añade afirmaciones externas.
- [ ] Las condiciones de detención están definidas.
- [ ] Las limitaciones están documentadas.

### 4.12. Rúbrica formativa

La evaluación considera diseño y evidencia.

No se premia el número de pasos.

| Dimensión | Inicial | Adecuada | Sólida para esta unidad |
|---|---|---|---|
| Descomposición | Pasos vagos | Funciones separadas | Contratos claros |
| Verificación | Impresiones | Algunas referencias | Métodos apropiados |
| Cálculos | Sin base | Operaciones visibles | Datos y base comprobados |
| Errores | Ocultos | Identificados | Gestión documentada |
| Conclusión | General | Limitada al caso | Beneficios y límites claros |

Una respuesta correcta puede tener una revisión insuficiente.

Una respuesta errónea puede generar un análisis valioso.

Los comentarios deben indicar cómo mejorar.

La rúbrica se aplica al trabajo presentado.

**No certifica fiabilidad para cualquier tarea.**

### 4.13. Preguntas de repaso

Responde con tus propias palabras.

Justifica las diferencias.

- ¿Qué aporta separar extracción y redacción?
- ¿Cuándo conviene mantener una sola interacción?
- ¿Qué diferencia hay entre revisión y evidencia independiente?
- ¿Por qué dos modelos pueden compartir un error?
- ¿Qué debe comprobarse antes de calcular un porcentaje?
- ¿Qué hacer si falta el denominador?
- ¿Por qué importa conservar unidades?
- ¿Qué significa detener una etapa?
- ¿Cómo puede propagarse un error?
- ¿Qué no demuestra una salida correcta?
- ¿Cuándo una regla automática necesita revisión?

**Comprender el método implica saber cuándo adaptarlo.**

### 4.14. Orientaciones para el docente

Prioriza comprobaciones observables.

Evita presentar la descomposición como técnica infalible.

Intervenciones útiles:

- “¿Qué produce esta etapa?”
- “¿Dónde aparece ese dato?”
- “¿Qué representa el denominador?”
- “¿Qué condición permite continuar?”
- “¿Esta conclusión está sustentada?”
- “¿Quién realizó la corrección?”
- “¿Qué no podéis concluir todavía?”

No fuerces errores si la salida integrada cumple.

Utiliza los ejemplos sintéticos para practicar incidencias.

Mantén las ampliaciones fuera de la hora obligatoria.

**La habilidad central es controlar el proceso con evidencia.**

### 4.15. Recursos relacionados

Continúa documentando con las plantillas del curso.

Estos recursos apoyan diseño, revisión y trazabilidad.

- [Plantillas](../plantillas/index.md)
- [Ficha de prompt](../plantillas/ficha-de-prompt.md)
- [Registro de versiones](../plantillas/registro-de-versiones.md)
- [Matriz de evaluación](../plantillas/matriz-de-evaluacion.md)
- [Checklist de seguridad](../plantillas/checklist-de-seguridad.md)
- [Proyecto final](../proyecto-final/index.md)

Relaciona cada evidencia con su versión.

Mantén fuentes originales y correcciones separadas.

Adapta el flujo al caso elegido.

No transfieras conclusiones sin nuevas pruebas.

**La documentación permite reutilizar decisiones y reconocer límites.**

### 4.16. Ideas esenciales para avanzar

Descomponer separa operaciones con funciones distintas.

Verificar contrasta resultados con referencias adecuadas.

Cada etapa necesita entradas y salidas claras.

Las transferencias pueden introducir errores.

La autorrevisión no equivale a comprobación independiente.

El acuerdo entre modelos no demuestra verdad.

Los cálculos necesitan datos, unidades y bases correctas.

La redacción debe conservar significado y certeza.

Una contradicción puede exigir detener una parte del flujo.

Más etapas no garantizan mejor calidad.

La conclusión debe reconocer beneficios, costes y límites.

**Un flujo útil permite saber qué se hizo, qué se comprobó y qué sigue pendiente antes de utilizar el resultado.**