# Ficha de caso de uso

La ficha de caso de uso describe una necesidad concreta antes de decidir qué instrucciones, técnicas o herramientas conviene utilizar.

Su función es conectar un problema realista con unas entradas disponibles, una salida útil y unos criterios de comprobación.

No es una descripción comercial de una solución.

Tampoco es un prompt ni una autorización para automatizar un proceso.

El objetivo es **delimitar una tarea que pueda diseñarse, evaluarse y revisarse de forma responsable**.

Esta página desarrolla la plantilla del curso y explica cómo completar cada campo.

Incluye ejemplos originales, propuestas de sesión y criterios para revisar las fichas entre compañeros.

Las actividades utilizan datos sintéticos.

Los resultados esperados son referencias docentes, no ejecuciones realizadas.

Las duraciones propuestas corresponden a sesiones alternativas y no deben sumarse automáticamente.

Una ficha puede terminar con pendientes si todavía falta información.

Lo importante es que esos pendientes sean visibles y permitan decidir qué hacer después.

!!! info "Uso de la plantilla"
    Completa la ficha antes de redactar la biblioteca de prompts.
    Actualízala cuando cambien el alcance, los datos o los requisitos.
    Conserva una versión identificable.
    Relaciona sus criterios con las pruebas del proyecto.

!!! warning "Límite de la ficha"
    Una ficha completa no demuestra que la solución funcione.
    Los resultados necesitan evaluación posterior.
    Los datos y las herramientas requieren autorización adecuada.
    La responsabilidad humana no se delega en el modelo.

---

## 1. Propósito y función de la ficha

La ficha establece un acuerdo de trabajo sobre qué se intenta resolver y qué queda fuera.

Ese acuerdo orienta las instrucciones, las pruebas y la documentación posterior.

### 1.1. Qué es un caso de uso

Un caso de uso describe una tarea situada en un contexto reconocible.

- Parte de una necesidad concreta.
- Identifica a quien utilizará el resultado.
- Describe información disponible.
- Define un resultado esperado.
- Establece límites de actuación.

No necesita una aplicación terminada para poder formularse.

**El caso de uso conecta necesidad, operación y resultado.**

### 1.2. Qué es la ficha

La ficha resume las decisiones esenciales sobre el caso.

- Explica el problema.
- Delimita entradas y salidas.
- Define criterios de éxito.
- Reconoce riesgos y limitaciones.
- Identifica revisión humana necesaria.

Puede mantenerse en un archivo o en una sección del expediente.

**Su valor está en la claridad del contenido, no en la complejidad del formato.**

### 1.3. Para qué sirve durante el curso

La ficha permite mantener coherencia entre actividades distintas.

- Orienta la primera instrucción.
- Justifica la selección de técnicas.
- Ayuda a elegir casos de prueba.
- Define qué debe revisar una persona.
- Apoya la decisión de entrega.

Debe consultarse cuando una mejora aparente cambia el alcance.

**Una respuesta atractiva puede ser inadecuada para el caso definido.**

### 1.4. Qué no debe prometer

La descripción debe evitar garantías que todavía no se han demostrado.

- Corrección universal.
- Ausencia completa de errores.
- Seguridad garantizada por el prompt.
- Ahorro de tiempo sin medición.
- Preparación automática para producción.

Las expectativas pueden registrarse como hipótesis pendientes.

**La ficha distingue intención, requisito y evidencia.**

### 1.5. Cuándo debe actualizarse

La ficha cambia cuando cambia una condición relevante del proyecto.

- Se incorpora otra fuente.
- Aparece un nuevo destinatario.
- Se modifica la salida.
- Se amplían permisos.
- Se descubre una limitación importante.

Cada actualización debe conservar su motivo y su versión.

**La ficha vigente debe describir el caso que realmente se evalúa.**

---

## 2. Estructura básica de la plantilla

Los ocho campos del documento base forman el núcleo de la ficha.

Los campos adicionales sirven para mejorar trazabilidad, no para sustituirlos.

### 2.1. Plantilla mínima

Esta estructura puede copiarse y completarse en un editor.

```markdown
# Ficha de caso de uso

- **Nombre del caso:**
- **Problema que resuelve:**
- **Usuario destinatario:**
- **Entradas disponibles:**
- **Salida esperada:**
- **Criterios de éxito:**
- **Riesgos y limitaciones:**
- **Revisión humana necesaria:**
```

**Los campos pendientes deben señalarse expresamente.**

### 2.2. Identificación complementaria

Una ficha compartida necesita reconocer su objeto y su estado.

- Identificador del caso.
- Versión de la ficha.
- Fecha de actualización.
- Responsable de elaboración.
- Estado de revisión.

Estos campos pueden aparecer al principio del documento.

**Identificar una versión no certifica su calidad.**

### 2.3. Estados recomendados

El estado permite comprender si la ficha está lista para orientar trabajo.

- Borrador.
- Pendiente de información.
- Revisada para diseño.
- Actualizada tras pruebas.
- Archivada o sustituida.

La transición necesita una razón comprensible.

**“Revisada para diseño” no equivale a “autorizada para operación”.**

### 2.4. Nivel de detalle

La extensión debe corresponder a la complejidad del caso.

- Una tarea breve puede necesitar pocas líneas.
- Una integración requiere más contexto.
- Las exclusiones deben ser explícitas.
- Los criterios deben ser comprobables.
- Los pendientes deben ser accionables.

Los anexos pueden contener contratos o políticas extensas.

**La ficha debe orientar sin obligar a adivinar.**

### 2.5. Regla de cumplimentación

Cada campo debe contener información pertinente y verificable cuando corresponda.

- Utiliza descripciones concretas.
- Evita afirmaciones promocionales.
- Separa hechos de hipótesis.
- Identifica lo desconocido.
- Revisa contradicciones entre campos.

No completes datos mediante intuición solo para cerrar el formulario.

**Una incertidumbre documentada es preferible a una precisión inventada.**

---

## 3. Nombre del caso y formulación del problema

El nombre facilita localizar la tarea.

El problema explica por qué merece atención sin presuponer que un modelo sea la solución adecuada.

### 3.1. Elegir un nombre funcional

El nombre debe describir una operación reconocible.

- Extractor de requisitos de formación.
- Preparador de borradores internos.
- Resumidor de notas de reunión.
- Clasificador de consultas sintéticas.
- Revisor de coherencia documental.

Evita nombres como “Asistente total” o “Automatización inteligente”.

**Un nombre concreto ayuda a mantener un alcance concreto.**

### 3.2. Describir el problema observable

La formulación debe explicar qué dificultad se encuentra en el trabajo.

- Información distribuida en varios párrafos.
- Campos ausentes difíciles de localizar.
- Diferencias entre propuestas y acuerdos.
- Tiempo de revisión variable.
- Errores de copia en registros manuales.

No es necesario afirmar una frecuencia sin datos.

**El problema se describe mediante situaciones, no mediante exageraciones.**

### 3.3. Separar problema y solución

Una necesidad puede admitir distintas respuestas.

- Cambiar una plantilla.
- Simplificar un procedimiento.
- Mejorar instrucciones humanas.
- Utilizar reglas deterministas.
- Incorporar apoyo de un modelo.

La ficha debe permitir comparar estas opciones.

**“Necesitamos un chatbot” describe una solución propuesta, no el problema.**

### 3.4. Reconocer consecuencias del problema

La relevancia depende de lo que ocurre cuando la tarea falla.

- Retrabajo.
- Información incompleta.
- Confusión del destinatario.
- Compromisos no autorizados.
- Decisiones basadas en datos incorrectos.

Distingue consecuencias observadas de consecuencias posibles.

**La consecuencia orienta la prioridad y la profundidad de revisión.**

### 3.5. Actividad: reescribir un problema ambiguo

La práctica parte de una declaración demasiado amplia.

- Entrada: “Queremos usar IA en formación”.
- Identifica una tarea concreta.
- Describe la dificultad actual.
- Señala quién la experimenta.
- Excluye objetivos que no puedan evaluarse.

El entregable contiene una formulación inicial y una revisada.

**La revisión debe mejorar precisión, no añadir terminología.**

---

## 4. Usuario destinatario y contexto de utilización

El destinatario determina qué resultado será útil y cómo debe presentarse.

La ficha también debe distinguir a quien opera la herramienta de quien recibe sus efectos.

### 4.1. Identificar al usuario principal

El usuario principal utiliza el resultado para una finalidad definida.

- Coordinación de formación.
- Revisión administrativa.
- Preparación documental.
- Análisis interno.
- Consulta de información.

Describe la función sin incluir nombres personales innecesarios.

**Un destinatario funcional suele ser suficiente para el diseño inicial.**

### 4.2. Distinguir funciones diferentes

Una misma solución puede involucrar varias personas.

- Operador del modelo.
- Usuario del resultado.
- Revisor de contenido.
- Responsable de autorización.
- Persona afectada por una comunicación.

Las funciones no tienen que corresponder siempre a personas distintas.

**La coincidencia de funciones no elimina la necesidad de definirlas.**

### 4.3. Describir el contexto de trabajo

El entorno ayuda a interpretar requisitos de utilidad.

- Canal de recepción.
- Lugar donde se consulta la salida.
- Frecuencia prevista de uso.
- Tiempo disponible para revisar.
- Herramientas autorizadas.

Lo desconocido se registra como pendiente de consulta.

**El contexto evita diseñar una salida útil solo en apariencia.**

### 4.4. Necesidades del destinatario

La ficha debe explicar qué necesita comprender o hacer la persona.

- Localizar información principal.
- Reconocer ausencias.
- Verificar evidencia.
- Identificar errores.
- Decidir el siguiente paso permitido.

No se presupone conocimiento técnico avanzado.

**La salida debe ser interpretable por su usuario real.**

### 4.5. Actividad: mapa de funciones

La práctica utiliza un preparador de borradores ficticio.

- Identifica quién introduce la solicitud.
- Define quién revisa la extracción.
- Señala quién recibe el borrador.
- Asigna la decisión de aprobación.
- Diferencia aprobación y envío.

El resultado es un mapa de funciones, no una asignación organizativa real.

**Las funciones pendientes deben permanecer visibles.**

---

## 5. Alcance, exclusiones y alternativas

La delimitación evita que el proyecto incorpore tareas nuevas sin revisar sus consecuencias.

Las exclusiones son parte del diseño, no una señal de fracaso.

### 5.1. Definir lo incluido

El alcance debe enumerar operaciones que el caso realmente contempla.

- Leer una entrada autorizada.
- Extraer campos definidos.
- Representar información ausente.
- Preparar un resultado revisable.
- Registrar observaciones.

Cada operación debe contribuir al problema seleccionado.

**Lo incluido necesita una relación clara con la salida esperada.**

### 5.2. Definir lo excluido

Las exclusiones impiden atribuir funciones no previstas.

- Confirmar disponibilidad.
- Aprobar presupuesto.
- Reservar recursos.
- Enviar comunicaciones.
- Modificar sistemas externos.

Estas exclusiones deben reflejarse en permisos y procedimientos.

**Una prohibición textual no sustituye retirar capacidades innecesarias.**

### 5.3. Condiciones de entrada al alcance

No todas las solicitudes son compatibles con la tarea.

- Idiomas evaluados.
- Formatos admitidos.
- Longitud de referencia.
- Fuentes permitidas.
- Categorías de información.

Los límites deben justificarse y comprobarse cuando corresponda.

**Una entrada fuera del alcance necesita una salida de error o derivación.**

### 5.4. Comparar alternativas

La ficha puede registrar opciones antes de escoger una estrategia.

- Procedimiento manual.
- Formulario estructurado.
- Reglas de validación.
- Plantilla documental.
- Apoyo de un modelo.

La comparación considera calidad, esfuerzo y riesgo.

**La opción más compleja no es necesariamente la más adecuada.**

### 5.5. Actividad: reducir un alcance excesivo

La propuesta inicial incluye gestión completa de una actividad.

- Recepción de solicitudes.
- Presupuestación.
- Reserva.
- Confirmación.
- Envío.

El alumnado selecciona una operación revisable y excluye las demás.

Debe explicar cómo se tratarán las peticiones fuera del alcance.

**Reducir alcance permite evaluar mejor una primera versión.**

---

## 6. Entradas disponibles y condiciones de datos

La ficha debe describir qué información existe y en qué condiciones puede utilizarse.

No debe confundir disponibilidad, pertinencia y autorización.

### 6.1. Inventario de entradas

El inventario identifica fuentes necesarias para la tarea.

- Texto de una solicitud.
- Tabla de requisitos.
- Documento de referencia.
- Política autorizada.
- Registro previamente validado.

Cada fuente debe tener una función definida.

**No se incorpora información únicamente porque esté disponible.**

### 6.2. Formatos y estructura

El formato afecta a la lectura y a la validación.

- Texto simple.
- Documento con secciones.
- Tabla.
- Archivo estructurado.
- Imagen, si está dentro del alcance.

La extracción de imágenes requiere comprobaciones propias.

**Una conversión de formato puede perder información relevante.**

### 6.3. Calidad y completitud

Las entradas pueden presentar problemas antes de utilizar el modelo.

- Campos ausentes.
- Valores incompatibles.
- Abreviaturas.
- Correcciones posteriores.
- Fragmentos ilegibles.

La ficha debe explicar cómo se representarán estas condiciones.

**Una fuente incompleta no autoriza completar datos por intuición.**

### 6.4. Autorización y minimización

Los datos deben corresponder a la finalidad y al entorno permitido.

- Preferencia por materiales sintéticos.
- Exclusión de identificadores innecesarios.
- Revisión de información confidencial.
- Ausencia de credenciales.
- Comprobación de acceso permitido.

Sustituir nombres por códigos no garantiza anonimato.

**Disponibilidad de un archivo no equivale a autorización para compartirlo.**

### 6.5. Actividad: inventario de una solicitud

La fuente docente contiene requisitos y detalles prescindibles.

- Identifica campos necesarios.
- Señala campos innecesarios.
- Describe formato.
- Registra ausencias.
- Propone una entrada minimizada.

No se utilizan documentos reales para demostrar minimización.

**La selección debe justificarse por la tarea definida.**

---

## 7. Salida esperada y contrato del resultado

La salida debe servir a una acción permitida y admitir revisión.

El contrato define tanto su presentación como el significado de sus campos.

### 7.1. Describir la utilidad de la salida

La ficha explica para qué se utilizará el resultado.

- Revisar requisitos.
- Preparar una aclaración.
- Comparar documentos.
- Identificar pendientes.
- Organizar información.

La salida no debe convertirse en una decisión que el alcance excluye.

**Utilidad y autoridad son dimensiones diferentes.**

### 7.2. Elegir el formato

El formato se selecciona según el consumidor del resultado.

- Texto breve para lectura.
- Lista para requisitos.
- Tabla para comparación.
- JSON para integración.
- Plantilla para documentación.

La disponibilidad técnica no obliga a escoger un formato complejo.

**El formato debe facilitar uso y comprobación.**

### 7.3. Definir campos y tipos

Las salidas estructuradas necesitan especificaciones explícitas.

- Nombre del campo.
- Tipo de dato.
- Carácter obligatorio.
- Valores permitidos.
- Representación de ausencia.

Una sintaxis válida no demuestra contenido correcto.

**El contrato estructural necesita validación semántica adicional.**

### 7.4. Conservar estados y evidencia

El resultado debe representar condiciones relevantes de la fuente.

- Exactitud o aproximación.
- Propuesta o confirmación.
- Ausencia.
- Contradicción.
- Fragmento de respaldo.

Una cifra correcta con un estado incorrecto sigue siendo un error.

**El significado incluye condiciones, no solo valores.**

### 7.5. Actividad: convertir una expectativa vaga

La petición inicial es “Devuelve un resumen útil”.

- Identifica destinatario.
- Define propósito.
- Establece partes obligatorias.
- Explica ausencias.
- Añade criterios de revisión.

El alumnado redacta un contrato antes de ejecutar.

**La expectativa debe permitir reconocer un incumplimiento.**

---

## 8. Criterios de éxito y método de comprobación

Los criterios traducen la utilidad esperada en condiciones observables.

Deben definirse antes de comparar respuestas.

### 8.1. Diferenciar objetivo y criterio

El objetivo describe el resultado general.

- Objetivo: organizar requisitos.
- Criterio: incluir campos obligatorios.
- Criterio: conservar aproximaciones.
- Criterio: representar ausencias.
- Criterio: evitar condiciones inventadas.

Un objetivo puede necesitar varios criterios.

**“Respuesta de calidad” no constituye un criterio suficiente.**

### 8.2. Clasificar criterios

La clasificación facilita elegir comprobaciones pertinentes.

- Estructurales.
- Semánticos.
- De seguridad.
- De utilidad.
- De funcionamiento del flujo.

Los requisitos críticos deben identificarse expresamente.

**Una buena presentación no compensa un compromiso no autorizado.**

### 8.3. Definir el método

Cada criterio necesita una forma de revisión.

- Validación de sintaxis.
- Comparación con la fuente.
- Comprobación de estados.
- Revisión por destinatario.
- Registro de tiempo y correcciones.

El método debe ser viable con las herramientas disponibles.

**Un criterio sin procedimiento puede quedarse en una impresión.**

### 8.4. Establecer umbrales y unidades

Las mediciones necesitan denominadores y condiciones.

- Casos evaluados.
- Ejecuciones realizadas.
- Campos comprobados.
- Errores críticos.
- Correcciones humanas.

Los umbrales se justifican según el contexto.

No se prescriben porcentajes universales para cualquier tarea.

**Un resultado agregado debe permitir comprender qué se contó.**

### 8.5. Tabla de criterios iniciales

Esta tabla es una referencia docente para un extractor.

| **Criterio** | **Método** | **Condición esperada** |
|---|---|---|
| Campos requeridos | Revisar contrato | Todos presentes |
| Fidelidad | Comparar fuente | Sin datos añadidos |
| Estados | Revisar evidencia | Aproximaciones conservadas |
| Ausencias | Comparar entrada | Sin valores inventados |

La tabla debe adaptarse antes de ejecutar.

**Las condiciones esperadas no representan resultados obtenidos.**

---

## 9. Riesgos, limitaciones y controles

La ficha debe reconocer qué puede fallar y qué medidas existen.

También debe distinguir controles implementados de propuestas pendientes.

### 9.1. Identificar riesgos pertinentes

El análisis parte de desviaciones relacionadas con la tarea.

- Inventar un dato.
- Omitir un requisito.
- Confundir una propuesta.
- Exponer información innecesaria.
- Introducir un compromiso.

Los riesgos deben describirse sin exageraciones.

**Un riesgo necesita una situación y una consecuencia comprensibles.**

### 9.2. Identificar limitaciones

Las limitaciones describen fronteras del sistema o de la evidencia.

- Solo se evaluaron textos breves.
- No se comprobaron adjuntos.
- La revisión es manual.
- La configuración completa no es visible.
- No existe integración de envío.

Estas formulaciones son ejemplos, no hechos del proyecto.

**La ficha registra únicamente las limitaciones que realmente corresponden.**

### 9.3. Describir controles

Los controles deben relacionarse con riesgos concretos.

- Minimización de datos.
- Contrato de salida.
- Validación independiente.
- Restricción de permisos.
- Revisión humana.

Cada control necesita un estado de implementación.

**Un control propuesto no reduce automáticamente el riesgo.**

### 9.4. Registrar riesgo residual

Después de aplicar controles puede persistir una desviación.

- Error no detectado.
- Interpretación ambigua.
- Revisión apresurada.
- Cambio de entorno.
- Fuente no representada en pruebas.

Las estimaciones deben seguir un método si se utilizan escalas.

**Reconocer incertidumbre permite decidir sin garantías ficticias.**

### 9.5. Actividad: relacionar riesgo y control

La práctica utiliza el riesgo de confirmar una fecha propuesta.

- Describe la desviación.
- Señala su consecuencia.
- Propone una restricción.
- Define una comprobación.
- Explica qué podría seguir fallando.

El entregable distingue diseño y efectividad observada.

**Escribir una regla no demuestra que el control funcione.**

---

## 10. Revisión humana y decisiones del flujo

La revisión debe ser ejecutable por una persona con información y autoridad suficientes.

No basta con escribir que “habrá supervisión”.

### 10.1. Definir puntos de intervención

El flujo necesita condiciones que activen revisión.

- Después de extracción.
- Antes de redactar.
- Ante contradicciones.
- Antes de compartir.
- Tras cambios relevantes.

La activación no debe depender solo de una alerta del modelo.

**Una puerta obligatoria puede existir fuera de la conversación.**

### 10.2. Definir qué se revisa

El protocolo debe señalar elementos concretos.

- Campos.
- Estados.
- Evidencias.
- Compromisos.
- Identificadores.

La revisión utiliza la fuente, no únicamente otra respuesta generada.

**El revisor necesita acceso al material que permite comprobar.**

### 10.3. Definir errores bloqueantes

Algunas discrepancias impiden continuar.

- Dato crítico inventado.
- Identificador incorrecto.
- Contradicción no tratada.
- Compromiso no autorizado.
- Fuente no permitida.

La ficha debe explicar la siguiente acción.

**Bloquear sin procedimiento de recuperación deja un flujo incompleto.**

### 10.4. Registrar aprobación y correcciones

La revisión debe quedar vinculada a un contenido.

- Versión revisada.
- Persona responsable.
- Correcciones realizadas.
- Operación autorizada.
- Fecha de decisión.

Una edición posterior puede requerir nueva revisión.

**Aprobar un borrador no autoriza necesariamente su envío.**

### 10.5. Actividad: protocolo para otra pareja

La práctica verifica claridad documental.

- Entrega fuente y salida.
- Facilita criterios.
- Pide comparar estados.
- Solicita registrar errores.
- Observa ayuda oral necesaria.

No se permite sustituir el protocolo por explicaciones continuas.

**La dificultad de uso revela pendientes de documentación.**

---

## 11. Ejemplo completo A · Requisitos de formación

Este ejemplo original muestra una ficha aplicada a extracción y preparación documental.

Su estado es docente y pendiente de ejecución.

### 11.1. Nombre, problema y destinatario

La tarea se limita a requisitos de una solicitud.

- Nombre: Preparador de requisitos de formación.
- Problema: información dispersa en texto.
- Usuario: coordinación de formación.
- Operador: participante del curso.
- Uso: revisión interna.

No se afirma ahorro de tiempo sin medición.

**El proyecto organiza información; no gestiona toda la actividad.**

### 11.2. Entradas y exclusiones

La fuente es una solicitud sintética.

- Aproximadamente 12 participantes.
- Modalidad presencial.
- Duración de dos horas.
- Fecha propuesta: 18 de noviembre de 2026.
- Presupuesto no indicado.

Se excluyen datos personales y operaciones externas.

**No se consulta disponibilidad ni se inventan condiciones.**

### 11.3. Salida esperada

El resultado combina valores y estados.

- Participantes: 12.
- Estado: aproximado.
- Modalidad: presencial.
- Duración: 120 minutos.
- Fecha: propuesta.

La conversión de horas a minutos está autorizada para este ejercicio.

**El presupuesto se representa como ausente.**

### 11.4. Criterios y revisión

La evaluación se realiza contra la fuente docente.

- Todos los campos están presentes.
- Las cifras conservan significado.
- La fecha no se confirma.
- El presupuesto no se completa.
- Los identificadores coinciden.

Una persona valida el registro antes de preparar un borrador.

**La referencia define expectativas, no resultados reales.**

### 11.5. Riesgos y decisión inicial

La ficha identifica condiciones de trabajo.

- Riesgo: convertir propuesta en acuerdo.
- Riesgo: perder aproximación.
- Control: revisión contra fuente.
- Limitación: casos sintéticos breves.
- Estado: candidata para pruebas.

Los controles deben comprobarse después de ejecutar.

**La ficha permite comenzar diseño, no autorizar uso externo.**

---

## 12. Ejemplo completo B · Notas de reunión

Este caso trabaja la diferencia entre información discutida y decisiones adoptadas.

La práctica utiliza notas inventadas y no requiere grabaciones reales.

### 12.1. Nombre y problema

La tarea resume contenido sin decidir por el equipo.

- Nombre: Organizador de notas de reunión.
- Problema: propuestas mezcladas con acuerdos.
- Usuario: responsable de seguimiento.
- Entrada: notas sintéticas.
- Uso: borrador interno.

La solución no evalúa desempeño personal.

**Resumir una reunión no implica establecer compromisos nuevos.**

### 12.2. Fuente docente

Las notas contienen estados diferenciados.

- Se propone revisar el calendario.
- Se acuerda preparar una lista de necesidades.
- No se asigna responsable de presupuesto.
- Se menciona una fecha tentativa.
- Queda pendiente confirmar recursos.

Cada afirmación debe conservar su condición.

**La ausencia de responsable no se resuelve por plausibilidad.**

### 12.3. Contrato de salida

La organización utiliza secciones claras.

- Temas tratados.
- Acuerdos explícitos.
- Propuestas.
- Pendientes.
- Información ausente.

Los responsables solo aparecen si están documentados.

**La salida no convierte conversación en aprobación.**

### 12.4. Criterios de éxito

La revisión compara cada sección con las notas.

- No se mezclan acuerdos y propuestas.
- No se añaden responsables.
- Las fechas conservan estado.
- Los pendientes son visibles.
- Cada acuerdo tiene respaldo.

Puede haber varias redacciones válidas.

**La coincidencia literal no es el criterio principal.**

### 12.5. Riesgos y supervisión

La revisión se centra en autoridad y fidelidad.

- Riesgo: inventar un acuerdo.
- Riesgo: asignar una responsabilidad.
- Control: comparación con notas.
- Limitación: no se evalúa transcripción.
- Revisor: persona con acceso a la fuente.

La aprobación externa queda fuera de la actividad.

**El resultado sigue siendo un borrador revisable.**

---

## 13. Ejemplo completo C · Clasificación de consultas

Este caso propone categorías para información sintética.

La clasificación no autoriza acceso ni ejecuta acciones.

### 13.1. Nombre y destinatario

La tarea ayuda a organizar consultas.

- Nombre: Clasificador de consultas internas.
- Problema: categorías utilizadas de forma inconsistente.
- Usuario: equipo de recepción.
- Entrada: consultas ficticias.
- Salida: categoría y justificación breve.

El sistema no resuelve automáticamente la solicitud.

**Clasificar y actuar son operaciones separadas.**

### 13.2. Categorías autorizadas

La actividad utiliza un catálogo limitado.

- Información.
- Documentación.
- Incidencia.
- Fuera del alcance.
- Revisión necesaria.

Cada categoría necesita una definición.

**Los nombres de categorías no bastan para establecer reglas.**

### 13.3. Entradas de prueba

La batería debe representar condiciones distintas.

- Consulta clara de información.
- Petición de documento.
- Descripción de fallo.
- Solicitud incompatible.
- Mensaje ambiguo.

Los casos son originales y no contienen datos reales.

**La ambigüedad debe poder derivarse a revisión.**

### 13.4. Criterios y salida

El contrato limita el resultado.

- Una categoría permitida.
- Justificación basada en el texto.
- Ausencia de datos añadidos.
- Derivación cuando corresponde.
- Ninguna acción externa.

No se exige certeza artificial.

**La política debe indicar qué hacer cuando faltan datos.**

### 13.5. Riesgos y límites

La ficha reconoce consecuencias posibles.

- Clasificación incorrecta.
- Derivación inadecuada.
- Exceso de confianza.
- Categorías insuficientes.
- Cambio del catálogo.

La revisión necesita actualizar referencias cuando cambian reglas.

**Una clasificación anterior no valida un catálogo nuevo.**

---

## 14. Sesiones prácticas para completar la ficha

Las propuestas permiten construir, revisar y mejorar fichas con tiempo definido.

La persona docente selecciona la sesión adecuada al momento del curso.

### 14.1. Sesión de treinta minutos

La actividad produce una ficha inicial.

- Cinco minutos: seleccionar tarea.
- Cinco minutos: describir problema y usuario.
- Diez minutos: entradas y salida.
- Cinco minutos: criterios y riesgos.
- Cinco minutos: revisión y pendientes.

No incluye una evaluación completa del modelo.

**El entregable es una ficha candidata, no una solución probada.**

### 14.2. Sesión de sesenta minutos

La actividad incorpora revisión cruzada.

- Diez minutos: necesidad y alternativas.
- Quince minutos: alcance y datos.
- Quince minutos: salida y criterios.
- Diez minutos: riesgos y supervisión.
- Diez minutos: intercambio y cierre.

Las transiciones están incluidas.

**La revisión debe conservar observaciones localizables.**

### 14.3. Sesión de noventa minutos

La propuesta relaciona ficha y primera comprobación.

- Quince minutos: ficha inicial.
- Quince minutos: contrato y referencia.
- Veinte minutos: instrucción y ejecución.
- Veinte minutos: evaluación y revisión.
- Veinte minutos: actualización y documentación.

Se utiliza una entrada sintética breve.

**La ficha actualizada distingue lo esperado de lo observado.**

### 14.4. Trabajo por parejas

Los roles permiten contrastar interpretación.

- Una persona redacta la ficha.
- Otra identifica ambigüedades.
- Ambas acuerdan criterios.
- Una conserva la ejecución.
- Otra revisa contra referencia.

Los desacuerdos se registran antes de resolverlos.

**El consenso debe apoyarse en reglas y evidencia.**

### 14.5. Cierre de la sesión

El cierre recoge decisiones y próximos pasos.

- Qué quedó definido.
- Qué sigue pendiente.
- Qué se ejecutó.
- Qué se observó.
- Qué necesita autorización adicional.

No se presenta una demostración como validación general.

**El resultado puede ser continuar, reducir alcance o detener.**

---

## 15. Revisión entre pares y errores frecuentes

La revisión comprueba si otra persona puede comprender el caso sin completar huecos.

Los comentarios deben señalar campos y mejoras concretas.

### 15.1. Preguntas de revisión

La pareja revisora utiliza preguntas orientadas a decisiones.

- ¿Qué problema concreto se aborda?
- ¿Quién utiliza el resultado?
- ¿Qué información está permitida?
- ¿Cómo se reconoce un error?
- ¿Quién puede detener el uso?

Las respuestas deben encontrarse en la ficha.

**La ayuda oral necesaria revela una mejora documental.**

### 15.2. Error: objetivo demasiado amplio

Una formulación extensa puede ocultar varias tareas.

- “Gestionar todos los procesos”.
- “Resolver cualquier consulta”.
- “Automatizar la comunicación”.
- “Mejorar toda la documentación”.
- “Eliminar errores humanos”.

La corrección consiste en seleccionar una operación evaluable.

**Un alcance menor puede producir una evidencia más sólida.**

### 15.3. Error: criterios subjetivos

Las preferencias generales dificultan comparar resultados.

- “Que sea bueno”.
- “Que parezca profesional”.
- “Que sea inteligente”.
- “Que resulte completo”.
- “Que no falle”.

Cada expresión debe transformarse en una condición observable.

**La claridad del criterio permite reconocer cumplimiento e incumplimiento.**

### 15.4. Error: supervisión genérica

Una referencia vaga no define un control efectivo.

- Revisor no identificado.
- Fuente no disponible.
- Tiempo insuficiente.
- Criterios ausentes.
- Autoridad de detención desconocida.

La corrección requiere procedimiento y responsables.

**“Lo revisará alguien” no constituye un protocolo.**

### 15.5. Rúbrica formativa

La rúbrica orienta observaciones sobre calidad documental.

| **Dimensión** | **Inicial** | **Adecuada** | **Sólida** |
|---|---|---|---|
| Problema | Amplio | Concreto | Consecuencias diferenciadas |
| Alcance | Ambiguo | Incluidos y excluidos | Condiciones de entrada |
| Contrato | Vago | Salida definida | Estados y evidencia |
| Revisión | Genérica | Procedimiento | Autoridad y versión |

La valoración no certifica una implementación.

**Los comentarios deben identificar una mejora realizable.**

---

## 16. Entrega, trazabilidad y continuidad

La ficha debe relacionarse con el resto del expediente.

Su cierre orienta el siguiente trabajo sin sustituir evaluación ni autorización.

### 16.1. Checklist de la ficha

Comprueba los campos antes de utilizarla como referencia.

- [ ] El problema está delimitado.
- [ ] El destinatario está identificado.
- [ ] Entradas y salida son compatibles.
- [ ] Los criterios admiten comprobación.
- [ ] Riesgos y revisión son visibles.

Los ocho campos originales deben estar completos o señalados como pendientes.

**Una casilla marcada representa una revisión realizada.**

### 16.2. Relación con otros materiales

La trazabilidad conecta decisiones y componentes.

- Ficha con biblioteca de prompts.
- Criterios con casos de prueba.
- Riesgos con controles.
- Salidas con revisión humana.
- Versiones con decisión de entrega.

Los identificadores facilitan reconstruir el recorrido.

**Un requisito sin prueba sigue sin estar evaluado.**

### 16.3. Entregable del alumnado

La entrega reúne ficha y observaciones relacionadas.

- Ficha identificada.
- Pendientes registrados.
- Revisión entre pares.
- Contrato o anexo cuando corresponda.
- Decisión de siguiente paso.

Las ejecuciones se incorporan solo si realmente se realizaron.

**La entrega distingue diseño, simulación y evidencia obtenida.**

### 16.4. Transferencia a un entorno profesional

Un contexto nuevo necesita revisión independiente.

- Necesidad laboral.
- Datos reales.
- Herramienta autorizada.
- Responsables.
- Criterios de piloto y detención.

La ficha formativa puede servir como punto de partida.

**Reutilizar el método no significa trasladar una autorización.**

### 16.5. Recursos y síntesis

Consulta los materiales relacionados del curso.

- [Plantillas](index.md).
- [Biblioteca de prompts](biblioteca-de-prompts.md).
- [Checklist de seguridad](checklist-de-seguridad.md).
- [Proyecto final](../proyecto-final/index.md).
- [Metodología](../guia-del-curso/metodologia.md).

La ficha comienza con una necesidad y termina con condiciones de trabajo claras.

**Un buen caso de uso permite saber qué resolver, cómo comprobarlo y cuándo no continuar.**