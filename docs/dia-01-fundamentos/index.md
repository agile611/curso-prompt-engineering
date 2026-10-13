# Día 1 · Fundamentos y anatomía de un buen prompt

La primera jornada del curso introduce las posibilidades y limitaciones de los modelos de lenguaje y establece una metodología para redactar instrucciones claras, pertinentes y verificables.

El objetivo es comprender qué información necesita un modelo para realizar una tarea y qué criterios permiten evaluar su respuesta.

El Prompt Engineering no consiste en memorizar fórmulas ni en escribir instrucciones cada vez más largas. Consiste en **definir una necesidad, comunicarla con precisión y comprobar el resultado**.

Esta página presenta el marco conceptual de la jornada. Los contenidos específicos se desarrollan en las unidades enlazadas.

## 1. Presentación de la jornada

La jornada proporciona una base para utilizar modelos de lenguaje con criterio y avanzar hacia aplicaciones más estructuradas.

### 1.1. Ficha general

Los contenidos están organizados para un nivel introductorio.

| Elemento | Descripción |
|---|---|
| Jornada | Día 1 · Fundamentos |
| Duración lectiva | 6 horas |
| Nivel | Introducción |
| Conocimientos previos | Familiaridad básica con una interfaz de LLM |
| Enfoque | Funcionamiento, diseño de instrucciones y evaluación |
| Finalidad | Establecer una metodología inicial de trabajo |

Las seis horas corresponden al tiempo lectivo. Las pausas se organizan aparte según la modalidad del curso.

### 1.2. Propósito

El propósito de esta jornada es pasar de una interacción basada en expectativas generales a una comunicación con requisitos reconocibles.

Para ello, distinguiremos tres dimensiones:

- **La tarea:** el trabajo que queremos realizar.
- **La instrucción:** la forma de comunicar ese trabajo al modelo.
- **La evaluación:** el procedimiento para comprobar si la respuesta cumple.

Estas dimensiones están relacionadas, pero no son equivalentes. Una instrucción bien redactada no garantiza una respuesta correcta, y una respuesta aparentemente correcta no demuestra que el diseño sea consistente.

### 1.3. Alcance

La jornada presenta los fundamentos necesarios para comprender y diseñar prompts.

No requiere programación, utilización de APIs ni conocimiento detallado de las arquitecturas matemáticas.

Tampoco pretende demostrar que un modelo puede resolver cualquier tarea de manera autónoma.

**La finalidad es desarrollar criterio para reconocer capacidades, límites y necesidades de verificación.**

---

## 2. Objetivos de aprendizaje

Los objetivos describen las capacidades que se desarrollarán durante la jornada.

Al finalizar podrás:

- Explicar de forma básica cómo genera respuestas un modelo de lenguaje.
- Distinguir entre modelo, aplicación y herramientas externas.
- Reconocer la influencia del contexto y del historial.
- Identificar las partes de un prompt.
- Diferenciar instrucciones, contexto y datos.
- Especificar restricciones y formato de salida.
- Reconocer ambigüedades y contradicciones.
- Transformar solicitudes generales en tareas verificables.
- Comprender la importancia de documentar versiones y resultados.
- Elegir un caso de uso con un alcance razonable.

### 2.1. Comprensión del funcionamiento

Comprenderás que la generación de texto depende de patrones aprendidos y de la información disponible durante la interacción.

También distinguirás entre producir una afirmación y verificarla.

### 2.2. Diseño de instrucciones

Reconocerás qué componentes ayudan a comunicar una tarea y cuándo resulta necesario hacerlos explícitos.

La claridad se entenderá como una combinación de precisión, pertinencia y coherencia.

### 2.3. Criterio de evaluación

Comprenderás por qué es necesario revisar el contenido, el cumplimiento y la utilidad de una respuesta por separado.

**Una buena presentación no sustituye la comprobación factual.**

---

## 3. Agenda y contenidos

La jornada sigue una progresión desde la comprensión inicial hasta la definición de una aplicación concreta.

### 3.1. Distribución del tiempo

Los cinco bloques mantienen la estructura general del curso.

| Bloque | Duración |
|---|---:|
| Introducción y diagnóstico | 1 h |
| Funcionamiento y limitaciones | 1 h |
| Anatomía del prompt | 1,5 h |
| Taller de prompts | 2 h |
| Caso de uso y entregable | 0,5 h |
| **Total** | **6 h** |

La secuencia conecta los fundamentos con el diseño y la documentación de instrucciones.

### 3.2. Introducción y diagnóstico

Esta unidad presenta el propósito del curso y el significado de trabajar con modelos de lenguaje de forma sistemática.

Sus contenidos principales son:

- Definición de Prompt Engineering.
- Diferencia entre preguntar y definir una tarea.
- Expectativas sobre el uso de IA.
- Importancia de establecer una referencia inicial.
- Relación entre intención, resultado y comprobación.

Consulta la unidad: [Introducción y diagnóstico](01-introduccion-y-diagnostico.md).

### 3.3. Funcionamiento y limitaciones

Esta unidad explica los conceptos que permiten interpretar el comportamiento del sistema.

Sus contenidos principales son:

- Modelo, producto y plataforma.
- Entrenamiento e inferencia.
- Tokens y generación de respuestas.
- Contexto, historial y memoria.
- Variabilidad.
- Herramientas externas.
- Información incorrecta o no sustentada.
- Limitaciones de actualidad y verificación.

Consulta la unidad: [Funcionamiento y limitaciones](02-funcionamiento-y-limitaciones.md).

### 3.4. Anatomía del prompt

Esta unidad organiza los componentes que permiten comunicar una tarea.

Sus contenidos principales son:

- Tarea y alcance.
- Contexto y destinatario.
- Datos de entrada.
- Restricciones.
- Formato de salida.
- Criterios de aceptación.
- Información ausente.
- Requisitos contradictorios.

Consulta la unidad: [Anatomía del prompt](03-anatomia-del-prompt.md).

### 3.5. Taller de prompts

Esta unidad desarrolla la metodología de mejora de instrucciones.

Su marco de trabajo incluye:

- Definición de una línea base.
- Identificación de problemas observables.
- Formulación de hipótesis de mejora.
- Comparación entre versiones.
- Comprobación de requisitos.
- Documentación de decisiones.
- Reconocimiento de los límites de una prueba.

Consulta la unidad: [Taller de prompts](04-taller-de-prompts.md).

### 3.6. Caso de uso y entregable

Esta unidad conecta el diseño de prompts con una necesidad concreta.

Sus contenidos principales son:

- Necesidad, tarea y solución.
- Persona destinataria.
- Datos disponibles.
- Resultado esperado.
- Alcance y exclusiones.
- Criterios de aceptación.
- Riesgos y controles.
- Diferencia entre resultado funcional y evidencia documental.

Consulta la unidad: [Caso de uso y entregable](05-caso-de-uso-y-entregable.md).

---

## 4. Marco conceptual de la jornada

Los siguientes principios atraviesan todos los bloques y sirven como referencia para las jornadas posteriores.

### 4.1. El prompt forma parte de un proceso

Un prompt es una entrada que orienta al modelo. Puede incluir instrucciones, contexto, datos y requisitos.

Sin embargo, el trabajo completo también comprende la selección de información, la configuración del entorno y la revisión del resultado.

**El prompt es un componente del proceso, no todo el proceso.**

### 4.2. La claridad depende de decisiones

Una instrucción clara requiere resolver cuestiones relevantes:

- Qué acción debe realizarse.
- Qué información puede utilizarse.
- Qué queda fuera del alcance.
- Cómo debe presentarse el resultado.
- Qué hacer cuando falten datos.

Añadir texto sin resolver estas cuestiones no necesariamente mejora el diseño.

### 4.3. El contexto debe ser pertinente

El contexto orienta la respuesta hacia una finalidad y un destinatario.

Su utilidad depende de que aporte información que modifique decisiones de contenido, profundidad o presentación.

Más contexto no significa automáticamente mejor contexto.

### 4.4. Las fuentes condicionan la respuesta

La calidad de los datos de entrada influye en la calidad del resultado.

Una fuente incompleta, ambigua o contradictoria puede impedir obtener una respuesta inequívoca.

El diseño debe reconocer esas condiciones en lugar de ocultarlas.

### 4.5. La ausencia de información debe conservarse

Un dato ausente no debe convertirse automáticamente en una suposición.

El tratamiento de la información incompleta debe definirse según la tarea y el formato.

Reconocer que falta información puede ser una respuesta correcta y útil.

### 4.6. Fluidez y exactitud son distintas

Los modelos pueden producir texto coherente que contenga errores.

El tono seguro, la estructura y la calidad expresiva no demuestran que una afirmación sea verdadera.

La revisión debe apoyarse en fuentes, operaciones comprobables y requisitos definidos.

### 4.7. Las herramientas requieren evidencia de uso

Una aplicación puede disponer de búsqueda, ejecución de código o consulta de documentos.

Su disponibilidad no demuestra que se hayan utilizado.

También debe distinguirse entre describir una acción y realizarla.

### 4.8. Una mejora necesita comprobación

Modificar una instrucción no demuestra que haya mejorado.

La comparación debe considerar los requisitos y las condiciones de ejecución.

Cuando cambian varios elementos a la vez, la diferencia observada no puede atribuirse con seguridad a uno solo.

### 4.9. Las conclusiones deben respetar las pruebas

Una pequeña muestra permite observar comportamientos concretos.

No demuestra fiabilidad general, ausencia de errores ni compatibilidad con cualquier entorno.

**La precisión de una conclusión depende de reconocer también lo que no se ha comprobado.**

### 4.10. La responsabilidad permanece en el uso

Las instrucciones pueden orientar al modelo, pero no sustituyen los controles de privacidad, seguridad y autorización.

La revisión debe ajustarse al impacto de la tarea y a las consecuencias de una respuesta incorrecta.

---

## 5. Documentación y continuidad

Los resultados de esta jornada constituyen una base que evolucionará durante el resto del curso.

### 5.1. Entregables previstos

La jornada contempla los siguientes entregables:

- Una plantilla reutilizable de prompt.
- Tres prompts mejorados.
- La ficha del caso de uso del proyecto final.

Los requisitos y las actividades correspondientes se desarrollan en las unidades específicas.

La documentación debe distinguir entre instrucciones, respuestas y valoraciones.

### 5.2. Recursos necesarios

Los recursos generales son:

- Acceso a una interfaz de LLM autorizada.
- Un documento de referencia sin datos sensibles.
- Un espacio para conservar versiones y resultados.
- [Ficha de prompt](../plantillas/ficha-de-prompt.md).
- [Ficha de caso de uso](../plantillas/ficha-de-caso-de-uso.md).

Las condiciones de privacidad y las funciones disponibles deben revisarse según la plataforma utilizada.

### 5.3. Recursos relacionados

Estas páginas apoyan la documentación y la evaluación:

- [Plantillas](../plantillas/index.md).
- [Registro de versiones](../plantillas/registro-de-versiones.md).
- [Matriz de evaluación](../plantillas/matriz-de-evaluacion.md).
- [Checklist de seguridad](../plantillas/checklist-de-seguridad.md).
- [Proyecto final](../proyecto-final/index.md).

Las plantillas organizan el trabajo, pero necesitan adaptarse a cada tarea.

### 5.4. Relación con las siguientes jornadas

Los fundamentos del día 1 se ampliarán progresivamente.

| Jornada | Enfoque |
|---|---|
| Día 1 | Fundamentos y anatomía del prompt |
| Día 2 | Técnicas y formatos |
| Día 3 | Evaluación y seguridad |
| Día 4 | Aplicaciones |
| Día 5 | Proyecto e integración |

La plantilla, los prompts y el caso de uso podrán cambiar conforme aparezcan nuevos requisitos y evidencias.

**La base de todo el curso es la misma: definir con claridad, comprobar con criterio y mejorar con evidencia.**