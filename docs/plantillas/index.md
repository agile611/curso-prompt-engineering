# Plantillas

Las plantillas del curso organizan la documentación necesaria para definir, diseñar, evaluar y mantener soluciones basadas en prompts.

Esta página es el índice ampliado de esos materiales.

Su función es explicar qué contiene cada documento, cuándo corresponde consultarlo y cómo se relaciona con los demás.

No incluye prácticas ni instrucciones de laboratorio.

Los procedimientos detallados, los formularios y los criterios específicos se encuentran en las páginas enlazadas.

El conjunto permite conservar la relación entre una necesidad, una instrucción, una ejecución y una decisión.

**Las plantillas aportan estructura documental; las evidencias permiten justificar las conclusiones.**

Una plantilla completa no demuestra por sí sola que una solución funcione.

Tampoco autoriza el tratamiento de datos reales ni el despliegue de una aplicación.

Los estados, las versiones, las limitaciones y los responsables deben quedar identificados.

!!! info "Orientación de consulta"
    Comienza por la ficha de caso de uso para comprender la necesidad.
    Consulta la ficha de prompt para describir cada componente.
    Utiliza la matriz y el registro para localizar evaluación y evolución.
    Mantén el checklist de seguridad relacionado con todo el expediente.

!!! warning "Alcance documental"
    Este índice describe las funciones de las plantillas disponibles.
    No declara que existan pruebas realizadas o controles implementados.
    Los resultados deben respaldarse mediante evidencias consultables.
    Las autorizaciones dependen del contexto real de utilización.

---

## 1. Propósito del conjunto de plantillas

Los seis materiales cubren funciones complementarias dentro del proyecto.

Cada uno responde preguntas distintas y evita concentrar toda la información en un único documento.

### 1.1. Delimitación de la necesidad

La definición del caso establece qué problema se aborda.

- Problema concreto.
- Usuario destinatario.
- Entradas disponibles.
- Resultado esperado.
- Exclusiones del alcance.

La referencia principal es la [Ficha de caso de uso](ficha-de-caso-de-uso.md).

### 1.2. Descripción de la instrucción

La documentación técnica explica cómo funciona cada componente.

- Identificación.
- Tarea.
- Contexto.
- Restricciones.
- Contrato de salida.

La referencia principal es la [Ficha de prompt](ficha-de-prompt.md).

### 1.3. Organización de componentes

La biblioteca facilita localizar instrucciones y sus condiciones de uso.

- Nombre funcional.
- Objetivo.
- Técnica.
- Versión.
- Ubicación.

La referencia principal es la [Biblioteca de prompts](biblioteca-de-prompts.md).

### 1.4. Comprobación de resultados

La evaluación relaciona expectativas con observaciones.

- Casos de prueba.
- Entradas.
- Referencias.
- Resultados observados.
- Cumplimiento por criterio.

La referencia principal es la [Matriz de evaluación](matriz-de-evaluacion.md).

### 1.5. Evolución y protección

El mantenimiento y la seguridad conservan decisiones que pueden cambiar con el tiempo.

- Cambios de contenido.
- Motivos de modificación.
- Efectos observados.
- Controles comprobados.
- Limitaciones y pendientes.

Las referencias son el [Registro de versiones](registro-de-versiones.md) y el [Checklist de seguridad](checklist-de-seguridad.md).

---

## 2. Directorio principal de materiales

Este directorio identifica la función central de cada página.

Las descripciones orientan la consulta sin sustituir el contenido de las plantillas.

### 2.1. Acceso directo

La siguiente tabla reúne los seis materiales del índice.

| **Plantilla** | **Función principal** | **Información central** |
|---|---|---|
| [Ficha de caso de uso](ficha-de-caso-de-uso.md) | Delimitar la necesidad | Problema, destinatario y alcance |
| [Ficha de prompt](ficha-de-prompt.md) | Documentar un componente | Instrucción, entradas y contrato |
| [Biblioteca de prompts](biblioteca-de-prompts.md) | Organizar componentes | Índice, versiones y ubicaciones |
| [Matriz de evaluación](matriz-de-evaluacion.md) | Registrar comprobaciones | Expectativas, observaciones y cumplimiento |
| [Registro de versiones](registro-de-versiones.md) | Explicar la evolución | Cambios, motivos y resultados |
| [Checklist de seguridad](checklist-de-seguridad.md) | Revisar condiciones de protección | Datos, permisos, validación y supervisión |

La tabla distingue funciones; no establece que alguna revisión se haya realizado.

### 2.2. Consulta por pregunta

La pregunta que necesita resolverse determina el documento pertinente.

- Necesidad: ficha de caso.
- Instrucción: ficha de prompt.
- Localización: biblioteca.
- Resultado: matriz.
- Cambio: registro de versiones.

Las preguntas sobre protección corresponden al checklist de seguridad.

### 2.3. Consulta por objeto

Cada material tiene un objeto documental principal.

- Caso de uso.
- Componente de instrucción.
- Conjunto de componentes.
- Evaluación de ejecuciones.
- Evolución de versiones.

La seguridad puede abarcar todos esos objetos dentro de un alcance definido.

### 2.4. Consulta por decisión

Las plantillas aportan información para decisiones diferentes.

- Delimitar una tarea.
- Seleccionar una instrucción.
- Interpretar una respuesta.
- Recomendar una versión.
- Restringir una operación.

La documentación apoya la decisión, pero no reemplaza a su responsable.

### 2.5. Consulta de referencias relacionadas

Los enlaces internos permiten ampliar una descripción sin duplicarla.

- El caso referencia requisitos.
- La ficha referencia pruebas.
- La biblioteca referencia fichas.
- El historial referencia cambios.
- El checklist referencia evidencias.

Una referencia útil debe conducir al objeto y a la versión correctos.

---

## 3. Ficha de caso de uso

La ficha de caso describe la necesidad que da sentido al proyecto.

Debe reflejar la tarea actual y no únicamente la intención inicial.

### 3.1. Finalidad de la página

La [Ficha de caso de uso](ficha-de-caso-de-uso.md) establece el marco funcional.

- Nombre del caso.
- Problema que resuelve.
- Usuario destinatario.
- Entradas disponibles.
- Salida esperada.

Su contenido orienta las decisiones técnicas posteriores.

### 3.2. Alcance y exclusiones

La delimitación evita atribuir al sistema funciones no previstas.

- Operaciones incluidas.
- Operaciones excluidas.
- Fuentes admitidas.
- Condiciones de utilización.
- Casos fuera del alcance.

Las exclusiones deben conservarse en las instrucciones y en los permisos.

### 3.3. Criterios de éxito

Los criterios expresan qué condiciones permiten considerar útil el resultado.

- Fidelidad a la fuente.
- Información obligatoria.
- Conservación de estados.
- Interpretabilidad para el destinatario.
- Ausencia de compromisos indebidos.

Los criterios específicos dependen de la tarea descrita.

### 3.4. Riesgos y revisión humana

La ficha identifica condiciones que requieren protección o intervención.

- Consecuencias de un error.
- Información sensible.
- Decisiones pendientes.
- Campos de revisión.
- Autoridad necesaria.

La supervisión debe describirse mediante funciones y condiciones concretas.

### 3.5. Relaciones documentales

El caso de uso actúa como referencia funcional del conjunto.

- La ficha de prompt desarrolla operaciones.
- La biblioteca organiza componentes.
- La matriz comprueba requisitos.
- El registro conserva cambios.
- El checklist examina riesgos y controles.

Si cambia el caso, deben revisarse las relaciones afectadas.

---

## 4. Ficha de prompt

La ficha técnica documenta una instrucción identificable y sus condiciones de ejecución.

Su contenido debe permitir distinguir diseño, observación y recomendación.

### 4.1. Identificación del componente

La [Ficha de prompt](ficha-de-prompt.md) conserva los datos de identidad.

- Nombre.
- Versión.
- Responsable.
- Modelo o plataforma.
- Fecha.

La identidad debe coincidir con los materiales realmente utilizados.

### 4.2. Descripción del diseño

El diseño explica la operación que realiza el componente.

- Tarea.
- Usuario destinatario.
- Contexto pertinente.
- Datos de entrada.
- Restricciones.

Una descripción clara permite reconocer incompatibilidades antes de ejecutar.

### 4.3. Contrato de salida

El contrato define qué resultado admite el componente.

- Formato.
- Campos.
- Tipos.
- Estados.
- Criterios de aceptación.

La corrección estructural no demuestra por sí sola fidelidad semántica.

### 4.4. Texto de la instrucción

El bloque de prompt conserva el contenido que gobierna la operación.

- Objetivo explícito.
- Variables identificadas.
- Fuentes delimitadas.
- Reglas disponibles.
- Límites de actuación.

La plantilla abstracta y el prompt completado deben distinguirse.

### 4.5. Observaciones y referencias

Las observaciones resumen lo aprendido sin reemplazar los registros completos.

- Casos evaluados.
- Resultados por criterio.
- Incidencias.
- Limitaciones.
- Cambios pendientes.

Las conclusiones deben relacionarse con ejecuciones y versiones concretas.

---

## 5. Biblioteca de prompts

La biblioteca permite localizar componentes y conocer su estado.

No debe confundirse con una colección indiferenciada de mensajes útiles.

### 5.1. Función del índice

La [Biblioteca de prompts](biblioteca-de-prompts.md) organiza las entradas disponibles.

- Nombre.
- Objetivo.
- Técnica.
- Versión.
- Ubicación.

Cada fila debe conducir a documentación suficiente para interpretar la entrada.

### 5.2. Alcance del término probado

Una entrada probada necesita evidencia de una ejecución revisada.

- Entrada conservada.
- Prompt completado.
- Respuesta original.
- Referencia identificada.
- Resultado de evaluación.

La etiqueta no implica funcionamiento universal ni autorización operativa.

### 5.3. Estados de las entradas

Los estados ayudan a seleccionar componentes sin confundir su trayectoria.

- Borrador.
- Candidata.
- Evaluada.
- Recomendada para un alcance.
- Sustituida o retirada.

Las condiciones de transición deben estar definidas en el proyecto.

### 5.4. Navegación y selección

La biblioteca puede organizarse por funciones y contratos.

- Extracción.
- Resumen.
- Redacción.
- Clasificación.
- Revisión.

Las categorías orientan la búsqueda, pero no acreditan compatibilidad.

### 5.5. Dependencias y mantenimiento

Una entrada puede depender de otras piezas documentales.

- Política de interpretación.
- Esquema de salida.
- Registro validado.
- Componente anterior.
- Procedimiento de revisión.

La recomendación debe reconsiderarse cuando cambian dependencias relevantes.

---

## 6. Matriz de evaluación

La matriz registra comprobaciones y permite interpretar diferencias entre expectativas y respuestas.

Su alcance debe corresponder a la tarea y a la versión evaluadas.

### 6.1. Estructura básica

La [Matriz de evaluación](matriz-de-evaluacion.md) relaciona cinco campos principales.

- Caso.
- Entrada.
- Resultado esperado.
- Resultado observado.
- Cumplimiento.

El resultado observado requiere una ejecución, no una respuesta ilustrativa.

### 6.2. Identificación de la prueba

La evaluación necesita condiciones conocidas para interpretar sus resultados.

- Versión del prompt.
- Modelo o plataforma.
- Fecha.
- Identificador de ejecución.
- Referencia utilizada.

Los parámetros desconocidos deben permanecer declarados como desconocidos.

### 6.3. Cobertura del alcance

La batería representa condiciones pertinentes para el caso.

- Situaciones normales.
- Información ambigua.
- Datos ausentes.
- Contradicciones.
- Condiciones extremas.

La diversidad necesita una justificación relacionada con requisitos y riesgos.

### 6.4. Lectura de resultados

La matriz debe separar unidades y estados de comprobación.

- Casos previstos.
- Casos ejecutados.
- Ejecuciones evaluadas.
- Criterios aplicables.
- Pendientes de aclaración.

Un porcentaje sin denominador puede inducir conclusiones incorrectas.

### 6.5. Relación con decisiones

Los resultados respaldan una decisión proporcionada.

- Continuidad con límites.
- Corrección.
- Ampliación de pruebas.
- Reducción del alcance.
- Retirada de una candidata.

La aceptación de una entrega no implica preparación para producción.

---

## 7. Registro de versiones

El historial explica qué cambió, por qué cambió y qué ocurrió después.

Su función es conservar una evolución reconstruible.

### 7.1. Estructura principal

El [Registro de versiones](registro-de-versiones.md) conserva cinco campos básicos.

- Versión.
- Fecha.
- Cambio.
- Motivo.
- Resultado.

El motivo y el resultado deben distinguirse claramente.

### 7.2. Identidad del contenido

Una versión representa un componente que puede recuperarse.

- Prompt.
- Política.
- Esquema.
- Procedimiento.
- Conjunto integrado.

Una etiqueta no debe identificar contenidos diferentes sin declaración explícita.

### 7.3. Naturaleza del cambio

La clasificación orienta las comprobaciones necesarias.

- Cambio documental.
- Cambio de instrucciones.
- Cambio de contrato.
- Cambio de entorno.
- Cambio de alcance.

Un cambio breve puede tener consecuencias funcionales importantes.

### 7.4. Efecto esperado y observado

La expectativa debe separarse de la evidencia posterior.

- Hipótesis de mejora.
- Casos de comprobación.
- Resultados obtenidos.
- Regresiones.
- Incertidumbres.

Un efecto pendiente no debe presentarse como una mejora demostrada.

### 7.5. Versión recomendada y recuperación

El historial ayuda a localizar la referencia vigente.

- Candidata actual.
- Versión recomendada.
- Versión sustituida.
- Motivo de retirada.
- Condiciones de recuperación.

Restaurar un archivo no revierte necesariamente acciones externas realizadas.

---

## 8. Checklist de seguridad

El checklist revisa condiciones de protección de la solución.

Su contenido abarca datos, fuentes, salidas, capacidades y supervisión.

### 8.1. Datos permitidos

El [Checklist de seguridad](checklist-de-seguridad.md) examina la información utilizada.

- Naturaleza sintética.
- Anonimización justificada.
- Finalidad.
- Minimización.
- Autorización contextual.

Sustituir nombres por códigos no garantiza anonimato.

### 8.2. Secretos y acceso

La revisión debe evitar exposición y acceso innecesario.

- Credenciales.
- Tokens.
- Claves privadas.
- Información restringida.
- Permisos de consulta.

La protección debe incluir entradas, salidas, capturas y registros.

### 8.3. Fuentes y límites de confianza

El contenido externo aporta información, no autoridad.

- Documentos.
- Mensajes.
- Páginas.
- Fragmentos recuperados.
- Respuestas de servicios.

Una fuente pertinente puede contener errores o instrucciones de desviación.

### 8.4. Validación y supervisión

Los resultados requieren controles adecuados antes de utilizarse.

- Validación estructural.
- Revisión semántica.
- Comprobación de compromisos.
- Intervención humana.
- Condiciones de detención.

Nombrar un revisor no demuestra que exista revisión efectiva.

### 8.5. Alcance de la protección

El checklist debe registrar controles y límites reales.

- Implementación.
- Comprobación.
- Evidencia.
- Riesgo residual.
- Decisión responsable.

Un prompt por sí solo no constituye una barrera suficiente.

---

## 9. Relaciones entre las plantillas

La coherencia del conjunto depende de referencias consistentes.

Los documentos deben complementarse sin contradecirse ni copiar información de forma divergente.

### 9.1. Del problema al componente

La necesidad debe mantener continuidad con la instrucción.

- Problema definido.
- Operación seleccionada.
- Entrada compatible.
- Resultado útil.
- Restricciones conservadas.

La ficha de prompt desarrolla una parte del caso de uso.

### 9.2. Del componente a la prueba

El contrato técnico orienta qué debe comprobar la matriz.

- Campos.
- Tipos.
- Estados.
- Transformaciones.
- Operaciones excluidas.

Una prueba pertinente necesita una relación con un requisito.

### 9.3. De la prueba al cambio

La evaluación puede motivar una modificación documentada.

- Discrepancia observada.
- Criterio afectado.
- Hipótesis.
- Cambio propuesto.
- Comprobación posterior.

El historial no debe atribuir una causa que la evidencia no demuestra.

### 9.4. Del cambio a la biblioteca

La evolución afecta al estado y a la selección de entradas.

- Nueva candidata.
- Recomendación actualizada.
- Limitación añadida.
- Dependencia modificada.
- Versión retirada.

La biblioteca debe señalar la referencia vigente, no solo la última edición.

### 9.5. Seguridad como relación transversal

La protección no pertenece únicamente al cierre del proyecto.

- Selección de datos.
- Diseño de instrucciones.
- Configuración de herramientas.
- Validación de respuestas.
- Conservación de registros.

El checklist debe corresponder al alcance y a la versión del conjunto.

---

## 10. Objetos, estados y vocabulario documental

El uso consistente de términos evita mezclar diseño y observación.

Cada objeto necesita una identidad y una función reconocibles.

### 10.1. Objetos principales

El expediente debe distinguir sus piezas.

- Caso de uso.
- Prompt.
- Caso de prueba.
- Ejecución.
- Incidencia.

Una ejecución no constituye una nueva versión si el contenido no cambia.

### 10.2. Expectativa y observación

Estos términos representan momentos distintos de la evaluación.

- Expectativa: resultado previsto.
- Referencia: criterio de comparación.
- Observación: respuesta obtenida.
- Dictamen: interpretación de la comparación.
- Decisión: acción autorizada posterior.

La expectativa debe existir antes de valorar la respuesta.

### 10.3. Estados de comprobación

Los estados deben reflejar el grado real de revisión.

- Cumple.
- No cumple.
- No evaluado.
- No aplica.
- Pendiente de aclaración.

El estado no aplica necesita una justificación vinculada al alcance.

### 10.4. Estados de utilización

La recomendación describe condiciones diferentes de una comprobación.

- Borrador.
- Candidata.
- Recomendada con límites.
- Sustituida.
- Retirada.

Una entrada evaluada puede permanecer sin recomendación.

### 10.5. Estados de los controles

Las medidas de protección también necesitan distinguir intención y realidad.

- Propuesta.
- Implementada.
- Comprobada.
- Evidencia insuficiente.
- No disponible.

Un control propuesto no reduce por sí solo el riesgo observado.

---

## 11. Organización del expediente de documentación

Las plantillas pueden mantenerse en archivos separados o en un documento integrado.

La estructura debe permitir consultar versiones, evidencias y decisiones.

### 11.1. Documento de apertura

El expediente necesita una entrada que explique su identidad.

- Nombre del proyecto.
- Propósito.
- Versión del conjunto.
- Estado de entrega.
- Índice de materiales.

El documento de apertura facilita navegación y evita interpretaciones equivocadas.

### 11.2. Materiales de diseño

Las decisiones funcionales y técnicas deben estar disponibles.

- Ficha de caso.
- Fichas de prompts.
- Políticas.
- Contratos.
- Dependencias.

Las reglas necesarias no deben quedar ocultas en mensajes antiguos.

### 11.3. Materiales de evaluación

Las conclusiones necesitan respaldo consultable.

- Casos.
- Entradas.
- Referencias.
- Respuestas originales.
- Resultados por criterio.

Una respuesta editada no reemplaza la evidencia de la ejecución.

### 11.4. Materiales de evolución y seguridad

El expediente conserva decisiones que afectan al uso.

- Historial.
- Incidencias.
- Checklist.
- Limitaciones.
- Responsables.

La información sensible debe minimizarse también dentro de estos registros.

### 11.5. Identidad del conjunto integrado

Una solución de varios componentes necesita indicar su combinación.

- Versión del sistema.
- Versiones de prompts.
- Versiones de políticas.
- Versión de la batería.
- Informe relacionado.

El conjunto entregado debe coincidir con el conjunto evaluado.

---

## 12. Consulta durante el recorrido del curso

Las plantillas acompañan las cinco jornadas sin convertirse en actividades independientes.

Su relevancia cambia según la etapa del aprendizaje.

### 12.1. 1 · Fundamentos

La primera jornada establece necesidad, tarea y línea base.

- Ficha de caso.
- Identificación inicial del prompt.
- Entradas y restricciones.
- Criterios preliminares.
- Registro de la versión inicial.

Consulta [1: Fundamentos](../dia-01-fundamentos/index.md).

### 12.2. 2 · Técnicas y formatos

La segunda jornada amplía estrategias y contratos.

- Ficha de prompt.
- Variables.
- Formatos.
- Biblioteca inicial.
- Historial de modificaciones.

Consulta [2: Técnicas y formatos](../dia-02-tecnicas/index.md).

### 12.3. 3 · Evaluación y seguridad

La tercera jornada conecta comprobación y protección.

- Matriz.
- Referencias.
- Incidencias.
- Checklist.
- Evidencias de comparación.

Consulta [3: Evaluación y seguridad](../dia-03-evaluacion-y-seguridad/index.md).

### 12.4. 4 · Aplicaciones profesionales

La cuarta jornada organiza componentes para tareas delimitadas.

- Caso actualizado.
- Biblioteca.
- Contratos entre etapas.
- Historial.
- Condiciones de revisión.

Consulta [4: Aplicaciones profesionales](../dia-04-aplicaciones/index.md).

### 12.5. 5 · Proyecto e integración

La quinta jornada consolida entrega, comunicación y transferencia.

- Identidad de la candidata.
- Evaluación integrada.
- Documentación consultable.
- Restricciones.
- Decisión final.

Consulta [5: Proyecto e integración](../dia-05-proyecto/index.md).

---

## 13. Orientación según función de consulta

Distintas personas necesitan localizar información diferente dentro del expediente.

El índice debe permitir esa consulta sin exigir conocimiento previo del proyecto.

### 13.1. Persona que define la necesidad

La consulta comienza por la pertinencia de la tarea.

- Problema.
- Destinatario.
- Alcance.
- Alternativas.
- Criterios de utilidad.

La referencia principal es la ficha de caso de uso.

### 13.2. Persona que opera el componente

La consulta debe explicar preparación y límites de ejecución.

- Versión.
- Variables.
- Entradas.
- Restricciones.
- Formato esperado.

La referencia principal es la ficha de prompt.

### 13.3. Persona que revisa resultados

La consulta necesita fuentes y criterios concretos.

- Entrada original.
- Referencia.
- Respuesta observada.
- Criterios.
- Incidencias.

La referencia principal es la matriz de evaluación.

### 13.4. Persona que mantiene la solución

La consulta debe permitir reconstruir cambios y dependencias.

- Historial.
- Motivos.
- Efectos observados.
- Regresiones.
- Versión recomendada.

Las referencias principales son el registro y la biblioteca.

### 13.5. Persona que autoriza o audita

La consulta necesita comprender evidencia, límites y responsabilidades.

- Alcance.
- Controles.
- Riesgos residuales.
- Pendientes.
- Decisión documentada.

La autorización debe corresponder a una versión y a operaciones determinadas.

---

## 14. Integridad, límites y navegación final

El conjunto debe seguir siendo comprensible después de la entrega.

La integridad documental permite reconocer qué está disponible y qué falta.

### 14.1. Coherencia de identidad

Los documentos deben referirse a los mismos componentes.

- Identificadores consistentes.
- Versiones correctas.
- Fechas pertinentes.
- Responsables identificados.
- Estados compatibles.

Una discrepancia debe corregirse o declararse explícitamente.

### 14.2. Coherencia de contenido

Los requisitos no deben cambiar de significado entre páginas.

- Alcance conservado.
- Restricciones compatibles.
- Variables definidas.
- Contratos relacionados.
- Criterios equivalentes.

Las referencias son preferibles a copias que puedan divergir.

### 14.3. Coherencia de evidencia

Las afirmaciones necesitan respaldo proporcionado.

- Ejecuciones conservadas.
- Referencias disponibles.
- Comparaciones identificadas.
- Reintentos visibles.
- Pendientes declarados.

Una plantilla cumplimentada no convierte una simulación en una prueba.

### 14.4. Continuidad y transferencia

Un contexto nuevo puede exigir reevaluación.

- Datos diferentes.
- Otro modelo.
- Nueva herramienta.
- Mayor autoridad.
- Distinto destinatario.

Reutilizar documentación no traslada automáticamente una autorización.

### 14.5. Navegación y síntesis

Los materiales disponibles cubren definición, diseño, evaluación y mantenimiento.

- [Ficha de caso de uso](ficha-de-caso-de-uso.md) y [Ficha de prompt](ficha-de-prompt.md).
- [Biblioteca de prompts](biblioteca-de-prompts.md).
- [Matriz de evaluación](matriz-de-evaluacion.md).
- [Registro de versiones](registro-de-versiones.md).
- [Checklist de seguridad](checklist-de-seguridad.md).

**Las plantillas resultan útiles cuando permiten comprender qué se diseñó, qué se comprobó, qué cambió y bajo qué límites puede utilizarse la solución.**