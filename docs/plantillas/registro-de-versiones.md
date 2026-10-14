# Registro de versiones

El registro de versiones documenta cómo cambia una solución basada en prompts y qué efectos se observan después de cada modificación.

No es únicamente una lista de fechas.

Relaciona una versión identificable con un cambio concreto, su motivo, las comprobaciones realizadas y la decisión posterior.

Su objetivo es **permitir que otra persona reconstruya la evolución del proyecto sin depender de explicaciones informales**.

Esta página desarrolla la plantilla del curso e incorpora ejemplos originales, procedimientos de comparación y actividades prácticas.

Los ejemplos utilizan datos sintéticos.

Los resultados ilustrativos se identifican como simulados.

Una expectativa de mejora no debe registrarse como un efecto observado.

Una versión nueva tampoco debe recomendarse solo porque sea la más reciente.

El recorrido básico puede realizarse con una interfaz de modelo de lenguaje y un editor de texto.

No requiere programación ni un sistema especializado de control de versiones.

!!! info "Regla principal"
    Documenta cada cambio y su efecto observado.
    Si todavía no se ha comprobado, registra el resultado como pendiente.
    Conserva las versiones anteriores y las respuestas originales.
    Relaciona cada conclusión con sus evidencias.

!!! warning "Límite del registro"
    Un historial completo no demuestra corrección universal.
    Una mejora local puede introducir regresiones.
    La aceptación formativa no autoriza un despliegue profesional.
    Los datos, permisos y responsables necesitan revisión contextual.

---

## 1. Propósito y alcance del registro

El historial conecta diseño, ejecución, evaluación y mantenimiento.

Su utilidad depende de describir el componente que realmente cambió.

### 1.1. Qué es una versión

Una versión identifica un contenido concreto que puede recuperarse.

- Puede corresponder a un prompt.
- Puede identificar una política.
- Puede representar un esquema.
- Puede describir un conjunto integrado.

La etiqueta debe relacionarse con materiales disponibles.

**Una versión es una referencia a contenido, no una promesa de calidad.**

### 1.2. Qué documenta el registro

Cada entrada explica una transición dentro del proyecto.

- Qué contenido cambió.
- Por qué se modificó.
- Cómo se comprobó.
- Qué decisión se tomó.

El registro puede enlazar documentos más extensos.

**El historial resume la evolución; las evidencias sostienen sus conclusiones.**

### 1.3. Para qué sirve durante el curso

El registro convierte la iteración en aprendizaje revisable.

- Conserva la línea base.
- Permite comparar alternativas.
- Hace visibles los errores.
- Justifica la versión seleccionada.

También permite reconocer cambios que no aportaron mejoras.

**Un intento rechazado puede aportar aprendizaje útil si queda documentado.**

### 1.4. Qué no debe confundirse con una versión

Otros objetos necesitan identificadores distintos.

- Un caso de prueba.
- Una ejecución.
- Una respuesta regenerada.
- Una incidencia.

Repetir una ejecución sin modificar el componente no crea necesariamente otra versión.

**Versionar contenido y registrar observaciones son operaciones diferentes.**

### 1.5. Alcance de las conclusiones

El resultado debe describir exactamente lo comprobado.

- La tarea evaluada.
- Los casos utilizados.
- Los criterios revisados.
- Las condiciones conocidas.

No extiendas una conclusión a contextos ausentes de la batería.

**“Mejoró en estos casos” es más preciso que “ahora funciona siempre”.**

---

## 2. Plantilla base y campos de registro

La estructura inicial contiene versión, fecha, cambio, motivo y resultado.

Puede ampliarse mediante referencias sin convertir la tabla en un documento ilegible.

### 2.1. Tabla original del curso

Esta tabla conserva los cinco campos del adjunto.

| **Versión** | **Fecha** | **Cambio** | **Motivo** | **Resultado** |
|---|---|---|---|---|
| v1 | Por registrar | Versión inicial | Línea base | Pendiente de evaluación |

La fila es una plantilla.

- No declara una ejecución.
- No presupone aceptación.
- No asigna una fecha ficticia.
- No anuncia una mejora.

**Completa el resultado después de consultar las evidencias.**

### 2.2. Campo versión

La etiqueta debe identificar el componente evaluado.

- Utiliza una convención estable.
- Evita etiquetas duplicadas.
- Relaciona la versión con su archivo.
- Distingue candidata y recomendada.

El nombre del archivo puede incorporar el identificador y la versión.

**No utilices una etiqueta para varios contenidos distintos.**

### 2.3. Campo fecha

La fecha debe corresponder al evento que se registra.

- Creación de la versión.
- Incorporación del cambio.
- Evaluación posterior.
- Decisión sobre su estado.

Si estos eventos no coinciden, documenta sus fechas por separado.

**Una fecha de edición no demuestra que el cambio haya sido probado.**

### 2.4. Campos cambio y motivo

Estos campos responden preguntas diferentes.

- Cambio: qué se modificó.
- Motivo: qué necesidad lo originó.
- Cambio: operación sobre el componente.
- Motivo: observación, requisito o decisión.

Una descripción como “mejorar el prompt” no concreta ninguno de los dos.

**El motivo explica la intervención; el cambio describe su contenido.**

### 2.5. Campo resultado

El resultado debe distinguir expectativa y observación.

- Pendiente de prueba.
- Observado en casos identificados.
- No concluyente.
- Rechazado o aceptado con alcance.

Añade referencias a la matriz o a las ejecuciones.

**No registres el efecto esperado como si ya se hubiera observado.**

---

## 3. Identificación de componentes y convención de versiones

La convención ayuda a localizar materiales y comprender relaciones.

Debe ser sencilla, consistente y adecuada al tamaño del proyecto.

### 3.1. Identificadores estables

El identificador representa la función del componente.

- `P-01`: extractor de requisitos.
- `P-02`: preparador de borradores.
- `POL-01`: política de interpretación.
- `SCH-01`: esquema de salida.

La versión se añade sin cambiar innecesariamente el identificador.

**La función permanece reconocible mientras evoluciona su contenido.**

### 3.2. Convención sencilla

Una secuencia corta puede ser suficiente para comenzar.

- `v1`: línea base.
- `v2`: primera modificación.
- `v3`: modificación posterior.
- `v4`: nueva candidata.

Esta opción coincide con el espíritu de la plantilla inicial.

**Una numeración mayor no significa una valoración mejor.**

### 3.3. Convención ampliada

Un proyecto puede necesitar distinguir etapas de desarrollo.

- `v0.1`: candidata inicial.
- `v0.2`: candidata revisada.
- `v1.0`: referencia recomendada localmente.
- `v1.1`: cambio posterior identificado.

Los criterios de transición deben definirse en el proyecto.

**La numeración no certifica preparación para producción.**

### 3.4. Versionado semántico adaptado

Una convención de tres partes puede utilizarse si se explican sus reglas.

- Cambio mayor: contrato incompatible.
- Cambio menor: capacidad compatible añadida.
- Corrección: ajuste sin cambio previsto de contrato.
- Estado adicional: candidata o retirada.

La compatibilidad de prompts puede ser difícil de establecer.

**No adoptes una convención compleja sin poder justificar sus categorías.**

### 3.5. Nombres de archivo

Los nombres deben permitir localizar el objeto exacto.

```text
P-01-v0.1.md
P-01-v0.2.md
POL-01-v1.0.md
SCH-01-v1.0.json
SIS-01-v0.3-manifiesto.md
```

Evita nombres como `final-ultimo-definitivo`.

Comprueba que el contenido coincide con la etiqueta.

**Una ruta clara facilita reconstrucción y comparación.**

---

## 4. Línea base y condiciones iniciales

La línea base es el punto de partida de una comparación.

Debe existir antes de afirmar que una versión mejora a otra.

### 4.1. Qué contiene la línea base

El conjunto inicial necesita materiales identificables.

- Prompt completo.
- Política aplicable.
- Contrato de salida.
- Casos y referencias.

También debe conservar sus observaciones, aunque sean desfavorables.

**La línea base no tiene que ser buena; tiene que ser interpretable.**

### 4.2. Registro del entorno

Las condiciones conocidas ayudan a comprender resultados.

- Modelo visible.
- Plataforma utilizada.
- Tipo de interfaz.
- Configuración disponible.

Registra como desconocida la información que no se muestra.

**No inventes parámetros predeterminados para completar el historial.**

### 4.3. Contexto de conversación

La ejecución puede depender de información adicional.

- Mensajes anteriores.
- Instrucciones personalizadas.
- Memoria conocida.
- Herramientas activas.

Una conversación nueva no garantiza aislamiento completo.

**Documenta el procedimiento utilizado y sus límites.**

### 4.4. Resultado inicial

La línea base puede mostrar cumplimiento parcial.

- Criterios satisfechos.
- Criterios incumplidos.
- Casos no ejecutados.
- Dudas de interpretación.

El resultado inicial debe separarse de los cambios posteriores.

**No reescribas el pasado para que la evolución parezca más limpia.**

### 4.5. Ficha de línea base

Este bloque es una plantilla de registro.

```text
Identificador de línea base:
Componentes y versiones:
Fecha:
Entorno conocido:
Casos previstos:
Casos ejecutados:
Referencias:
Resultados por criterio:
Incidencias:
Limitaciones:
```

**Los campos pendientes permanecen visibles.**

---

## 5. Clasificación de cambios y motivos

Clasificar una modificación ayuda a elegir las comprobaciones necesarias.

El tamaño del cambio textual no determina por sí solo su impacto.

### 5.1. Cambio documental

Una modificación puede mejorar la explicación sin alterar la instrucción ejecutada.

- Aclaración de una ficha.
- Corrección de una ruta.
- Descripción de una variable.
- Incorporación de una limitación.

Si cambia el procedimiento de uso, puede afectar a las ejecuciones futuras.

**No declares “sin impacto” únicamente porque el prompt permanezca igual.**

### 5.2. Cambio de instrucciones

La modificación puede alterar comportamiento esperado.

- Nueva restricción.
- Cambio de prioridad.
- Aclaración de una transformación.
- Incorporación de un ejemplo.

Debe conservarse el texto anterior y el nuevo.

**Una palabra como “solo” puede cambiar significativamente el contrato.**

### 5.3. Cambio de entrada o salida

El contrato puede evolucionar de forma incompatible.

- Nuevo campo obligatorio.
- Tipo diferente.
- Catálogo modificado.
- Política de ausencia distinta.

La siguiente etapa necesita comprobar compatibilidad.

**Un prompt correcto puede dejar de integrarse si cambia su interfaz.**

### 5.4. Cambio de entorno

El comportamiento puede variar sin editar el prompt.

- Otro modelo.
- Otra plataforma.
- Herramientas nuevas.
- Personalización diferente.

Registra esta transición como un cambio de condiciones.

**No atribuyas automáticamente una diferencia al texto de la instrucción.**

### 5.5. Cambio de alcance

La tarea puede incorporar responsabilidades nuevas.

- Otro destinatario.
- Datos reales.
- Nuevo idioma.
- Acciones externas.

Este cambio necesita revisar requisitos, riesgos y autorización.

**Una ampliación de alcance no es una simple mejora de redacción.**

---

## 6. Observación, hipótesis y efecto esperado

El motivo de un cambio debe partir de una necesidad identificable.

La hipótesis orienta la comprobación sin fingir certeza sobre la causa.

### 6.1. Observación inicial

La observación describe lo que ocurrió.

- Caso identificado.
- Fragmento de la fuente.
- Fragmento de la respuesta.
- Criterio afectado.

Evita explicaciones causales en este primer registro.

**“Se perdió la aproximación” describe mejor el hecho que “el modelo no entendió”.**

### 6.2. Hipótesis de causa

La hipótesis propone una explicación posible.

- Regla insuficientemente explícita.
- Ejemplo incompatible.
- Contrato incompleto.
- Dependencia del contexto previo.

Puede haber varias explicaciones plausibles.

**La hipótesis no demuestra qué ocurrió dentro del modelo.**

### 6.3. Propuesta de modificación

El cambio debe ser concreto y localizable.

- Añadir una regla.
- Eliminar una contradicción.
- Corregir un ejemplo.
- Separar una etapa.

Relaciona la modificación con el criterio afectado.

**No combines cambios independientes si necesitas interpretar sus efectos.**

### 6.4. Efecto esperado

La expectativa debe poder contrastarse.

- Conservar un estado.
- Reducir una omisión concreta.
- Evitar una clave adicional.
- Mantener una condición pendiente.

No establezcas mejoras universales sin un método para comprobarlas.

**El efecto esperado se escribe antes de observar la nueva salida.**

### 6.5. Plantilla de hipótesis

Este ejemplo es docente y no representa un resultado real.

```text
Observación:
En CAS-02 se omite la condición aproximada.

Hipótesis:
La regla no distingue suficientemente valor y estado.

Cambio propuesto:
Separar ambos campos y exigir conservar aproximaciones.

Efecto esperado:
CAS-02 mantiene 12 con estado aproximado.

Comprobación:
Repetir CAS-02 y revisar casos normales y ausentes.
```

**La conclusión se añadirá después de ejecutar.**

---

## 7. Comparación de versiones y resultados observados

Comparar exige mantener condiciones pertinentes y declarar diferencias.

Una respuesta favorable aislada no demuestra una mejora estable.

### 7.1. Casos comunes

La comparación utiliza entradas equivalentes entre versiones.

- Mismo contenido.
- Mismos identificadores cuando corresponda.
- Mismas referencias.
- Mismos criterios.

Los casos nuevos deben identificarse como una ampliación de cobertura.

**No compares versiones mediante baterías diferentes sin explicar la diferencia.**

### 7.2. Condiciones comparables

El entorno debe mantenerse cuando resulte posible.

- Modelo conocido.
- Procedimiento de conversación.
- Herramientas activas.
- Configuración disponible.

Las condiciones desconocidas limitan la interpretación.

**Comparabilidad no significa control perfecto de todos los factores.**

### 7.3. Repeticiones y variación

Las respuestas pueden variar aunque no cambie la instrucción.

- Define cuántos intentos realizarás.
- Conserva intentos pertinentes.
- Distingue repetición y fallo técnico.
- Registra variación observada.

No selecciones silenciosamente la salida más favorable.

**La política de repeticiones debe establecerse antes de evaluar.**

### 7.4. Resultado por criterio

El efecto debe describirse de forma localizada.

- Conserva aproximaciones.
- Sigue omitiendo presupuesto.
- Mejora estructura.
- Introduce una condición no autorizada.

El resultado global necesita reglas de aceptación.

**“Mejoró” debe indicar qué criterio cambió y cuál permaneció igual.**

### 7.5. Tabla de comparación

Esta tabla es una plantilla pendiente de ejecución.

| **Caso** | **Versión A** | **Versión B** | **Interpretación** |
|---|---|---|---|
| CAS-01 | No evaluada | No evaluada | Pendiente |
| CAS-02 | No evaluada | No evaluada | Pendiente |
| CAS-03 | No evaluada | No evaluada | Pendiente |

La interpretación debe consultar respuestas y criterios.

**La tabla no declara resultados favorables por anticipado.**

---

## 8. Regresión, aceptación y estados de uso

Una corrección necesita comprobar que no deteriora otros requisitos.

El estado recomendado debe corresponder a evidencias, no a expectativas.

### 8.1. Qué es una regresión

Una regresión es un deterioro respecto a un requisito previamente satisfecho.

- Aparece una omisión nueva.
- Se altera un estado.
- Se rompe el formato.
- Se añade un compromiso.

Puede observarse en un caso que antes cumplía.

**Resolver el fallo inicial no elimina la necesidad de revisar otros criterios.**

### 8.2. Batería de regresión

Selecciona casos relacionados con el cambio.

- Caso que motivó la modificación.
- Caso normal.
- Caso con ausencia.
- Caso de riesgo relevante.

La cobertura debe justificarse según el componente.

**No existe una cifra universal de pruebas suficiente para cualquier proyecto.**

### 8.3. Estados de evaluación

Los estados deben distinguir observación y pendiente.

- `cumple`.
- `no_cumple`.
- `no_evaluado`.
- `pendiente_de_aclaracion`.

El estado `no_aplica` puede utilizarse con justificación.

**Una prueba omitida no se considera favorable.**

### 8.4. Estados de uso

La decisión sobre utilización es distinta del resultado de una prueba.

- Candidata.
- Recomendada para un alcance.
- Sustituida.
- Retirada.

Una entrada ejecutada puede seguir sin ser recomendable.

**La última candidata no reemplaza automáticamente la versión vigente.**

### 8.5. Decisión de aceptación

La decisión debe identificar contenido y condiciones.

- Versión aceptada.
- Alcance permitido.
- Restricciones.
- Pendientes y responsable.

La recepción documental no implica aceptación.

**La aceptación formativa no autoriza datos reales ni operaciones externas.**

---

## 9. Evidencias, trazabilidad y manifiesto del sistema

El historial debe relacionar cambios con objetos consultables.

Una conclusión sin evidencia localizada resulta difícil de auditar.

### 9.1. Identificadores de evidencia

Utiliza convenciones que distingan funciones.

- `CAS-01`: caso.
- `EJ-001`: ejecución.
- `REF-01`: referencia.
- `INC-01`: incidencia.

Estos objetos se relacionan con componente y versión.

**Una ejecución no debe utilizarse como identificador de versión.**

### 9.2. Respuestas originales

La salida debe conservarse antes de editarla.

- Contenido pertinente completo.
- Identificador de ejecución.
- Advertencias visibles.
- Errores observados.

Las correcciones humanas se guardan separadamente.

**Una respuesta corregida no sustituye la evidencia del incumplimiento original.**

### 9.3. Enlaces internos

Las referencias deben permitir abrir el material correcto.

- Rutas relativas consistentes.
- Nombres de archivo estables.
- Secciones identificables.
- Versiones explícitas.

Comprueba enlaces antes de entregar.

**Un enlace roto limita la auditabilidad del registro.**

### 9.4. Manifiesto integrado

Un sistema con varios componentes necesita identificar su combinación.

```text
Sistema: SIS-01-v0.3
Extractor: P-01-v0.2
Borrador: P-02-v0.1
Revisor: P-03-v0.1
Política: POL-01-v1.0
Esquema: SCH-01-v1.0
Batería: BAT-01-v0.2
Informe: INF-01-v0.3
Estado: pendiente de evaluación integrada
```

**Este bloque es ilustrativo y no declara una configuración real.**

### 9.5. Integridad del conjunto

La entrega debe coincidir con lo evaluado.

- Versiones compatibles.
- Políticas disponibles.
- Esquemas correctos.
- Evidencias relacionadas.

Una discrepancia necesita corrección o declaración explícita.

**No presentes como evaluado un conjunto diferente del que ejecutaste.**

---

## 10. Ejemplo docente · Evolución de un extractor

Este caso original utiliza solicitudes sintéticas de formación.

La evolución descrita sirve para practicar el registro y no representa pruebas realizadas.

### 10.1. Caso de uso y límites

La tarea consiste en organizar requisitos explícitos.

- Participantes.
- Modalidad.
- Duración.
- Fecha y presupuesto.

No confirma disponibilidad, aprueba condiciones ni envía comunicaciones.

**El alcance debe conservarse durante todas las versiones.**

### 10.2. Fuente común

Esta entrada permite revisar valores y estados.

```text
Participarán aproximadamente 12 personas.
La modalidad será presencial.
La duración indicada es de dos horas.
Proponemos el 18 de noviembre de 2026.
La fecha todavía no está confirmada.
```

El presupuesto está ausente.

La fecha es una propuesta, no una autorización.

**La referencia debe conservar aproximaciones y pendientes.**

### 10.3. Versión inicial

La candidata inicial contiene una instrucción insuficientemente definida.

```text
Resume los requisitos de esta solicitud.
Devuelve una respuesta breve.
Solicitud:
{{solicitud}}
```

Puede utilizarse como línea base exploratoria.

No establece todavía un contrato suficiente para recomendación.

**La debilidad documental debe registrarse antes de comparar resultados.**

### 10.4. Primera modificación

La segunda candidata delimita mejor la transformación.

```text
Extrae participantes, modalidad, duración, fecha y presupuesto.
Usa exclusivamente la solicitud.
Conserva aproximaciones y estados de fecha.
Representa ausencias como "no indicado".
Devuelve una tabla.
No confirmes disponibilidad ni condiciones.
Solicitud:
{{solicitud}}
```

La modificación necesita ejecución y evaluación.

**La mayor precisión textual es una hipótesis de mejora, no una prueba.**

### 10.5. Registro inicial del ejemplo

La tabla conserva pendientes en lugar de inventar observaciones.

| **Versión** | **Fecha** | **Cambio** | **Motivo** | **Resultado** |
|---|---|---|---|---|
| v1 | Por registrar | Resumen breve | Línea base | Pendiente |
| v2 | Por registrar | Campos y estados | Delimitar extracción | Pendiente |
| v3 | Por registrar | Por definir | Dependerá de evidencia | No creada |

La tercera fila no debe incorporarse al historial definitivo hasta existir.

**Una propuesta futura puede mantenerse en un listado separado.**

---

## 11. Ejemplos de resultados y decisiones simuladas

Los siguientes escenarios permiten practicar interpretación.

Todos los resultados de esta sección son simulados y deben conservar esa etiqueta.

### 11.1. Escenario A · Mejora localizada

La versión nueva conserva una aproximación perdida en la línea base.

- CAS-02 mejora en estado.
- El valor numérico permanece igual.
- No se observan cambios en modalidad.
- Otros casos siguen pendientes.

La decisión puede ser continuar con la evaluación.

**No procede declarar estabilidad general.**

### 11.2. Escenario B · Mejora con regresión

La versión nueva conserva estados, pero omite presupuesto explícito.

- El criterio de aproximación mejora.
- El criterio de completitud empeora.
- El caso normal presenta una omisión.
- La aceptación depende de requisitos obligatorios.

La decisión puede ser corregir antes de recomendar.

**No compenses una omisión crítica con una mejora distinta.**

### 11.3. Escenario C · Sin diferencia concluyente

Las versiones producen resultados variables en pocas repeticiones.

- Algunas ejecuciones cumplen.
- Otras incumplen el mismo criterio.
- No hay patrón suficiente.
- El entorno tiene condiciones desconocidas.

La conclusión puede mantenerse como no concluyente.

**La incertidumbre debe registrarse, no ocultarse mediante selección.**

### 11.4. Escenario D · Cambio de política

La expectativa cambia porque se modifica una regla autorizada.

- La versión anterior seguía otra política.
- La referencia debe versionarse.
- La comparación directa necesita explicación.
- El nuevo requisito requiere pruebas propias.

No se describe automáticamente como un fallo antiguo.

**Cambiar el criterio cambia el significado de la comparación.**

### 11.5. Redacción del resultado

Este bloque muestra una conclusión simulada proporcionada.

```text
Resultado simulado:
La candidata v2 conserva la aproximación en CAS-02.
CAS-01 mantiene los campos comprobados.
CAS-03 presenta una omisión de presupuesto.
La versión no se recomienda todavía.
Se propone una corrección localizada y nueva regresión.
No se ha evaluado uso con datos reales.
```

**La etiqueta de simulación debe permanecer junto al contenido.**

---

## 12. Actividades de sesión para el alumnado

Las sesiones convierten el historial en una práctica de diseño y evaluación.

Las propuestas son alternativas y sus tiempos incluyen transiciones.

### 12.1. Sesión de treinta minutos

La actividad crea un registro inicial y una hipótesis.

- Cinco minutos: tarea y contrato.
- Cinco minutos: línea base.
- Diez minutos: ejecución y revisión.
- Cinco minutos: hipótesis.
- Cinco minutos: historial y pendientes.

No incluye una batería completa.

**El resultado puede ser una candidata pendiente de modificación.**

### 12.2. Sesión de sesenta minutos

La actividad compara dos versiones sobre un alcance breve.

- Diez minutos: referencias.
- Quince minutos: línea base.
- Diez minutos: cambio localizado.
- Quince minutos: comparación.
- Diez minutos: decisión y registro.

Selecciona pocos casos bien definidos.

**La comparación debe conservar respuestas de ambas versiones.**

### 12.3. Sesión de noventa minutos

La propuesta incorpora regresión y revisión cruzada.

- Quince minutos: línea base.
- Quince minutos: evaluación inicial.
- Quince minutos: modificación.
- Treinta minutos: pruebas y regresión.
- Quince minutos: revisión y cierre.

Las ampliaciones requieren otro bloque.

**El tiempo limitado no justifica marcar pruebas inexistentes.**

### 12.4. Trabajo por parejas

Los roles ayudan a contrastar interpretación.

- Una persona modifica el componente.
- Otra comprueba referencias.
- La primera conserva ejecuciones.
- La segunda revisa el resultado.

Ambas registran desacuerdos y decisión.

**El acuerdo necesita criterios y evidencia, no solo preferencia compartida.**

### 12.5. Auditoría cruzada

Otra pareja intenta reconstruir la evolución sin ayuda continua.

- Localiza la línea base.
- Encuentra el cambio.
- Consulta una ejecución.
- Explica la decisión.

La ayuda oral necesaria se registra como mejora.

**La auditabilidad se comprueba mediante consulta efectiva del expediente.**

---

## 13. Ejercicios de diagnóstico del historial

Los ejercicios siguientes muestran errores frecuentes de registro.

El alumnado debe corregirlos sin inventar evidencias ausentes.

### 13.1. Ejercicio: “mejoras varias”

Una fila no explica qué cambió.

- Divide modificaciones independientes.
- Identifica campos afectados.
- Añade motivos concretos.
- Relaciona pruebas existentes.

Si no hay evidencia suficiente, conserva el resultado pendiente.

**Una descripción detallada no permite reconstruir pruebas que nunca se realizaron.**

### 13.2. Ejercicio: fecha nueva, contenido antiguo

El archivo cambia de etiqueta, pero conserva exactamente la instrucción anterior.

- Comprueba contenido.
- Identifica si hubo cambio documental.
- Corrige la descripción.
- Evita atribuir una mejora inexistente.

Una actualización administrativa puede registrarse como tal.

**Cambiar el nombre no modifica el comportamiento esperado.**

### 13.3. Ejercicio: resultado elegido entre intentos

La tabla conserva únicamente la salida más favorable.

- Revisa política de repeticiones.
- Localiza intentos disponibles.
- Corrige recuentos.
- Declara evidencia perdida.

Si no pueden recuperarse observaciones, limita la conclusión.

**La selección silenciosa puede exagerar el efecto del cambio.**

### 13.4. Ejercicio: cambio múltiple

Una candidata modifica prompt, modelo y referencia simultáneamente.

- Identifica factores cambiados.
- Evita atribución causal única.
- Diseña una comparación adicional.
- Registra límites del resultado.

El conjunto puede ser útil, aunque no permita aislar efectos.

**Utilidad observada y explicación causal son cuestiones diferentes.**

### 13.5. Ejercicio: historial reconstruido de memoria

El equipo intenta recuperar fechas y resultados sin archivos.

- Registra que la reconstrucción es retrospectiva.
- Conserva solo hechos comprobables.
- Señala incertidumbres.
- No fabrica respuestas.

Puede recuperarse parte del recorrido, no necesariamente todo.

**La memoria del equipo no equivale a una ejecución conservada.**

---

## 14. Reversión, seguridad y mantenimiento

El registro debe permitir recuperar una versión anterior cuando sea apropiado.

La reversión también necesita comprobar compatibilidad y condiciones actuales.

### 14.1. Qué significa revertir

Revertir consiste en volver a un contenido identificado.

- Recuperar un prompt anterior.
- Restaurar una política.
- Recuperar un esquema compatible.
- Reestablecer una combinación del manifiesto.

La versión anterior debe estar disponible.

**Volver atrás no garantiza que el contexto actual siga siendo compatible.**

### 14.2. Condiciones de reversión

La decisión necesita revisar consecuencias.

- Datos ya transformados.
- Etapas dependientes.
- Permisos actuales.
- Aprobaciones vinculadas.

Una operación externa realizada no se deshace al restaurar el prompt.

**Contenido reversible y efectos reversibles son categorías diferentes.**

### 14.3. Secretos e información sensible

El historial puede conservar accidentalmente datos que no deben compartirse.

- No incluir claves.
- Minimizar identificadores.
- Revisar capturas.
- Controlar acceso a copias.

Un sistema de versiones puede conservar contenido eliminado de la vista actual.

**Retirar un secreto del último archivo no demuestra su eliminación del historial.**

### 14.4. Incidencias y retirada

Un fallo relevante puede suspender una recomendación.

- Identifica la versión afectada.
- Registra alcance conocido.
- Define medidas autorizadas.
- Establece condiciones de retorno.

La recuperación necesita comprobación posterior.

**No cierres una incidencia únicamente porque el archivo vuelve a abrirse.**

### 14.5. Mantenimiento continuo

El historial debe revisarse cuando cambian condiciones importantes.

- Modelo o plataforma.
- Datos o destinatario.
- Políticas.
- Herramientas y permisos.

La frecuencia depende del contexto y de las reglas aplicables.

**No inventes periodos universales de revisión para cualquier solución.**

---

## 15. Checklist final, entrega y continuidad

El cierre verifica que la evolución puede reconstruirse y que las conclusiones son proporcionadas.

Una entrega puede quedar pendiente si faltan evidencias relevantes.

### 15.1. Checklist de identidad

Comprueba la coherencia de las versiones.

- [ ] Cada etiqueta identifica contenido.
- [ ] Las fechas corresponden a eventos.
- [ ] Los archivos son localizables.
- [ ] La versión recomendada está señalada.

Las versiones retiradas deben distinguirse claramente.

**El historial debe corresponder a los materiales disponibles.**

### 15.2. Checklist de comparación

Comprueba el respaldo de los efectos observados.

- [ ] Existe línea base.
- [ ] Las referencias están identificadas.
- [ ] Las respuestas originales se conservan.
- [ ] Las regresiones se revisaron o declararon pendientes.

Las diferencias de entorno deben ser visibles.

**Una mejora declarada necesita criterios y evidencias relacionadas.**

### 15.3. Criterios de calidad documental

La revisión valora claridad, respaldo y utilidad.

| **Dimensión** | **Inicial** | **Adecuada** | **Sólida** |
|---|---|---|---|
| Identidad | Etiquetas ambiguas | Contenido localizable | Componentes relacionados |
| Cambio | Descripción genérica | Modificación concreta | Impacto y dependencias |
| Resultado | Impresión general | Evidencia disponible | Comparación y regresión |
| Decisión | Estado confuso | Alcance indicado | Responsable y pendientes |

La rúbrica es formativa y no certifica producción.

**Los comentarios deben señalar mejoras realizables.**

### 15.4. Entregable del alumnado

La entrega reúne registro y materiales relacionados.

- Historial cumplimentado.
- Versiones conservadas.
- Ejecuciones y referencias.
- Decisión final y limitaciones.

La cantidad exigida depende de la actividad o del proyecto.

**No atribuyas al curso umbrales que no se hayan establecido.**

### 15.5. Recursos y síntesis

Consulta los documentos relacionados para mantener coherencia.

- [Ficha de prompt](ficha-de-prompt.md).
- [Matriz de evaluación](matriz-de-evaluacion.md).
- [Biblioteca de prompts](biblioteca-de-prompts.md).
- [Checklist de seguridad](checklist-de-seguridad.md).

Relaciona el historial con el [proyecto final](../proyecto-final/index.md).

**Documentar versiones significa mostrar qué cambió, por qué cambió y qué permiten concluir las pruebas, sin confundir una expectativa con un efecto observado.**