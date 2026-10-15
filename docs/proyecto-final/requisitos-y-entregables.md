# Requisitos y entregables

El proyecto final reúne las capacidades del curso en una solución delimitada, evaluada y documentada.

Cada equipo debe entregar materiales que permitan comprender qué problema aborda, cómo utiliza los prompts y qué resultados ha observado.

No basta con mostrar una respuesta satisfactoria.

La entrega debe permitir que otra persona reconstruya el trabajo, revise sus evidencias y conozca sus limitaciones.

Esta página desarrolla los requisitos del proyecto y explica cómo organizarlos en un expediente consultable.

También incluye ejemplos originales y sesiones de trabajo para preparar, revisar y consolidar la entrega.

Los ejemplos utilizan datos sintéticos.

Las referencias docentes indican resultados esperados, no respuestas obtenidas mediante ejecuciones reales.

**El objetivo es demostrar competencia en diseño, evaluación y documentación, no afirmar que un modelo acierta siempre.**

Cada equipo debe entregar los siguientes elementos:

- Un problema concreto y un usuario destinatario.
- Entradas, salidas y criterios de aceptación.
- Prompts documentados.
- Al menos dos versiones comparadas.
- Entre 8 y 10 casos de prueba.
- Resultados, limitaciones y medidas de privacidad.
- Instrucciones de uso y puntos de revisión humana.

Estos elementos deben describir la solución que realmente se entrega.

Las decisiones pendientes deben permanecer visibles.

!!! info "Condición de trazabilidad"
    Identifica las versiones que ejecutas.
    Conserva las entradas y las respuestas originales.
    Relaciona los resultados con criterios y evidencias.
    Distingue materiales ilustrativos de ejecuciones reales.

!!! warning "Límite de la entrega"
    La aceptación del proyecto es formativa.
    No autoriza un despliegue profesional.
    Los usos reales requieren revisar datos, herramientas, permisos y responsabilidades.
    Las conclusiones deben limitarse al alcance efectivamente evaluado.

---

## 1. Marco general de los requisitos

Los requisitos establecen el contenido mínimo de la entrega y orientan su revisión.

### 1.1. Qué significa completar el proyecto

Completar el proyecto implica presentar materiales suficientes para interpretar la solución.

- La necesidad está delimitada.
- Las instrucciones son identificables.
- Las pruebas están documentadas.
- La decisión final tiene respaldo.

**La finalización no depende únicamente de que el sistema produzca una respuesta atractiva.**

### 1.2. Requisitos y calidad de la evidencia

La presencia de un documento no demuestra que su contenido sea suficiente.

- Una ficha puede tener campos ambiguos.
- Una matriz puede carecer de respuestas originales.
- Un historial puede confundir expectativas y resultados.
- Una guía puede omitir condiciones de detención.

**Cada entregable debe aportar información útil para comprender o comprobar el proyecto.**

### 1.3. Alcance de los mínimos establecidos

Los mínimos corresponden al proyecto académico descrito en esta página.

- Se requieren al menos dos versiones comparadas.
- Se requieren entre 8 y 10 casos de prueba.
- Se requieren medidas de privacidad documentadas.
- Se requieren instrucciones y revisión humana.

**Estos mínimos no constituyen un estándar universal de validación profesional.**

### 1.4. Responsabilidad del equipo

El equipo debe mantener coherencia entre lo que declara y lo que conserva.

- Identifica los componentes utilizados.
- Comprueba las referencias internas.
- Explica las exclusiones.
- Registra los pendientes.

**No atribuyas a una persona o herramienta una comprobación que no realizó.**

### 1.5. Mapa de correspondencia requerido

La trazabilidad es un requisito del proyecto. Cada elemento del curso debe poder relacionarse con un objetivo de aprendizaje, una actividad o una evidencia concreta.

La organización mínima recomendada es la siguiente:

- Contenido original: qué se había propuesto en el curso o en la actividad.
- Contenido ampliado: qué variación se introdujo y por qué.
- Objetivo de aprendizaje: qué competencia se pretende desarrollar.
- Actividad: qué operación concreta se realizó.
- Evidencia: qué entrada, salida o registro se conserva.
- Criterio de evaluación: qué asumimos como aceptable y cómo lo comprobamos.

Esto permite distinguir entre:

- Caso de prueba: una entrada de evaluación específica.
- Ejecución: la interacción realizada con el sistema.
- Repetición: la reejecución del mismo caso con otra versión.
- Versión: la variante del prompt o del procedimiento.
- Referencia: la norma, extracto o criterio que define lo esperado.
- Resultado observado: la respuesta emitida por el sistema.
- Decisión humana: la interpretación, validación o bloqueo final.

Sin esa separación, es fácil confundir una respuesta bonita con una respuesta útil o un cambio del prompt con una mejora demostrada.

---

## 2. Mapa de entregables y evidencias

Los requisitos pueden organizarse mediante una matriz que facilite localizar sus materiales.

### 2.1. Correspondencia entre requisito y documento

La siguiente tabla propone una organización, no nombres obligatorios de archivo.

| **Requisito** | **Material principal** | **Respaldo necesario** |
|---|---|---|
| Problema y destinatario | Ficha de caso | Alcance y contexto |
| Entradas, salidas y aceptación | Contrato de la tarea | Variables, reglas y criterios |
| Prompts documentados | Biblioteca y fichas | Texto completo y versiones |
| Dos versiones comparadas | Informe comparativo | Ejecuciones y referencias comunes |
| Entre 8 y 10 casos | Batería de pruebas | Entradas y expectativas |
| Resultados, límites y privacidad | Informe y auditoría | Evidencias y controles |
| Uso y revisión humana | Guía del operador | Pasos, bloqueos y responsables |

**La tabla debe apuntar a materiales que existan en la entrega.**

### 2.2. Identificadores de requisitos

Los identificadores facilitan relacionar documentos y comprobaciones.

- `REQ-01`: problema y destinatario.
- `REQ-02`: contrato de entradas y salidas.
- `REQ-03`: documentación de prompts.
- `REQ-04`: comparación de versiones.
- `REQ-05`: trazabilidad entre versión, criterio y evidencia.
- `REQ-06`: revisión humana ejecutable.

**La numeración es orientativa y debe aplicarse consistentemente si se utiliza.**

### 2.3. Localización de evidencias

Una evidencia debe poder abrirse e interpretarse sin reconstrucciones informales.

- Tiene una ubicación conocida.
- Identifica el componente o ejecución.
- Incluye condiciones relevantes.
- Se relaciona con un criterio.

**Un nombre de archivo sin contenido disponible no constituye evidencia consultable.**

### 2.4. Estado de cada requisito

El inventario debe distinguir presencia documental y revisión.

- Disponible.
- Revisado.
- Pendiente.
- No disponible.

**Un requisito pendiente no debe marcarse como completo para mejorar la apariencia de la entrega.**

### 2.5. Ejemplo de flujo documentado

El siguiente patrón es válido para documentar una tarea completa sin convertirla en una promesa de automatización total:

```text
Entrada sintética
    ↓
Comprobación de variables
    ↓
Extracción de requisitos
    ↓
Validación estructural
    ↓
Revisión de fidelidad
    ↓
Preparación de borrador
    ↓
Revisión humana
    ↓
Uso autorizado dentro del alcance
```

Este flujo ayuda a distinguir qué pasos forman parte del diseño del prompt, qué pasos son de validación y qué pasos requieren una persona responsable. No implica que todo el proceso esté automatizado, ni que se pueda ejecutar sin intervención humana en contextos con riesgo o documentación sensible.

---

## 3. Problema concreto y usuario destinatario

La ficha del caso explica para qué existe la solución y quién necesita su resultado.

### 3.1. Formulación del problema

El problema debe describir una dificultad reconocible en una tarea concreta.

- Información dispersa en mensajes.
- Clasificación inconsistente de solicitudes.
- Preparación repetitiva de borradores.
- Revisión lenta de documentos.

**Evita formulaciones generales como “mejorar la productividad con inteligencia artificial”.**

### 3.2. Identificación del destinatario

La función destinataria determina qué necesita recibir y cómo lo utilizará.

- Coordinación de formación.
- Equipo de soporte.
- Revisión administrativa.
- Personal técnico o editorial.

**Utiliza funciones cuando los nombres personales no aporten información necesaria.**

### 3.3. Resultado útil y exclusiones

La descripción debe distinguir lo que se entrega de lo que queda fuera.

- Se extraen requisitos.
- Se prepara un borrador.
- No se confirma disponibilidad.
- No se envían comunicaciones.

**Una tarea de apoyo no debe convertirse silenciosamente en una operación con autoridad.**

### 3.4. Ejemplo de caso delimitado

El ejemplo docente aborda solicitudes sintéticas de formación.

- Problema: conservar requisitos al preparar borradores.
- Destinatario: coordinación de formación.
- Resultado: registro revisable y borrador interno.
- Exclusión: reservas, precios y envío de mensajes.

**Este ejemplo describe una propuesta académica, no una aplicación desplegada.**

---

## 4. Entradas y condiciones de preparación

El equipo debe explicar qué información necesita la solución y cómo se prepara.

### 4.1. Inventario de fuentes

Cada fuente debe tener una función dentro de la tarea.

- Solicitud que aporta requisitos.
- Política que define interpretaciones.
- Catálogo que establece categorías.
- Registro previamente validado.

**No añadas fuentes únicamente porque estén disponibles o parezcan relacionadas.**

### 4.2. Variables y formatos

Los marcadores necesitan definiciones suficientes para el operador.

- Nombre exacto.
- Significado.
- Tipo o formato.
- Obligatoriedad y tratamiento de ausencia.

**Una variable no explicada obliga a interpretar condiciones que deberían estar documentadas.**

### 4.3. Precondiciones de ejecución

La guía debe indicar cuándo una entrada no está preparada.

- Falta una variable obligatoria.
- La fuente está vacía.
- La política necesaria no está disponible.
- El formato de entrada es incompatible.

**Un error de preparación debe registrarse separadamente del fallo de una respuesta.**

### 4.4. Identidad y límites de confianza

Las fuentes necesitan identificación, pero no adquieren autoridad sobre la tarea.

- Identificador del expediente.
- Identificador de la fuente.
- Origen y versión cuando corresponda.
- Separación entre datos e instrucciones.

**Los delimitadores ayudan a la claridad, pero no garantizan aislamiento de seguridad.**

---

## 5. Salidas y criterios de aceptación

El contrato define qué resultado admite la solución y cómo se comprobará.

### 5.1. Estructura de salida

La presentación debe responder al uso posterior del resultado.

- Campos obligatorios.
- Tipos de dato.
- Valores permitidos.
- Política de claves o secciones adicionales.

**Un formato técnicamente correcto puede contener información semánticamente incorrecta.**

### 5.2. Criterios semánticos

La revisión debe comparar significado, estados y respaldo.

- Conservación de cifras.
- Interpretación autorizada de unidades.
- Mantenimiento de aproximaciones.
- Correspondencia con las fuentes.

**Una cifra correcta acompañada de un estado incorrecto constituye una discrepancia.**

### 5.3. Criterios bloqueantes

Algunas desviaciones impiden continuar o utilizar el resultado.

- Dato crítico inventado.
- Identificador de otro expediente.
- Contradicción ocultada.
- Compromiso no autorizado.

**Un resultado favorable en otros criterios no compensa automáticamente un error bloqueante.**

### 5.4. Matriz de aceptación

Esta tabla es una referencia docente que debe adaptarse al caso.

| **Criterio** | **Comprobación** | **Condición esperada** |
|---|---|---|
| Estructura | Revisar contrato | Campos y tipos compatibles |
| Fidelidad | Comparar fuente | Sin datos añadidos |
| Estados | Revisar contexto | Aproximaciones y pendientes conservados |
| Autoridad | Examinar compromisos | Sin decisiones nuevas |
| Identidad | Comparar identificadores | Sin mezcla de expedientes |

**Los criterios se definen antes de observar las respuestas.**

---

## 6. Prompts documentados

La entrega debe conservar las instrucciones y sus condiciones de utilización.

### 6.1. Ficha de cada componente

Cada prompt necesita una identidad técnica reconocible.

- Nombre e identificador.
- Versión.
- Responsable o función de mantenimiento.
- Fecha y estado.

**La etiqueta de versión debe corresponder a un contenido recuperable.**

### 6.2. Contenido de diseño

La ficha debe explicar cómo utilizar e interpretar el componente.

- Tarea y destinatario.
- Entradas y variables.
- Restricciones.
- Formato y criterios de éxito.

**Las reglas necesarias no deben quedar escondidas en conversaciones anteriores.**

### 6.3. Texto completo y prompt completado

La plantilla y la ejecución contienen objetos diferentes.

- La plantilla conserva reglas estables.
- Los marcadores indican valores variables.
- El prompt completado muestra los valores introducidos.
- La ejecución conserva la respuesta obtenida.

**Guardar únicamente la plantilla no demuestra qué se utilizó en cada prueba.**

### 6.4. Biblioteca del proyecto

La biblioteca organiza los componentes y facilita su selección.

- Nombre funcional.
- Operación que realiza.
- Versión disponible.
- Ubicación y estado de evaluación.

**Una entrada disponible no debe presentarse como recomendada sin respaldo suficiente.**

---

## 7. Comparación de al menos dos versiones

El proyecto requiere una comparación real entre versiones identificadas de la solución o de un componente equivalente.

### 7.1. Qué constituye una comparación pertinente

Las versiones deben permitir valorar una evolución de la misma tarea.

- Comparten el problema principal.
- Mantienen criterios comparables.
- Utilizan entradas comunes.
- Declaran cambios de contrato o alcance.

**Comparar dos prompts de funciones distintas no demuestra por sí solo mejora de una versión.**

### 7.2. Línea base y candidata

La comparación necesita un punto de partida conservado.

- Versión inicial completa.
- Casos y referencias.
- Resultados de la línea base.
- Nueva candidata con cambio identificable.

**La línea base puede presentar fallos; su función es permitir interpretar la evolución.**

### 7.3. Hipótesis y cambio

La modificación debe responder a una observación o necesidad concreta.

- Criterio afectado.
- Discrepancia localizada.
- Cambio propuesto.
- Efecto esperado.

**La hipótesis orienta la prueba, pero no demuestra la causa del fallo.**

### 7.4. Condiciones de comparación

La comparación debe mantener condiciones pertinentes cuando resulte posible.

- Mismo contenido de entrada.
- Referencias compatibles.
- Procedimiento de revisión consistente.
- Entorno conocido o diferencias declaradas.

**Cambiar prompt, modelo y política simultáneamente limita la atribución del efecto observado.**

---

## 8. Batería de entre 8 y 10 casos de prueba

El requisito corresponde a casos distintos y documentados, no a una suma indiferenciada de respuestas.

### 8.1. Casos y ejecuciones

Estos objetos necesitan identidades diferentes.

- Un caso describe una situación de prueba.
- Una ejecución observa una versión en ese caso.
- Un caso puede tener varias ejecuciones.
- Una repetición no crea automáticamente otro caso.

**Diez respuestas a la misma entrada no equivalen a diez casos de prueba.**

### 8.2. Selección de la batería

La variedad debe responder a requisitos y riesgos del proyecto.

- Casos normales.
- Ausencias o entradas incompletas.
- Ambigüedades y contradicciones.
- Condiciones límite o de desviación.

**No existe una distribución universal obligatoria entre categorías para todos los proyectos.**

### 8.3. Comparación sobre una batería común

Para este proyecto, utiliza preferentemente los mismos casos en las dos versiones comparadas.

- Ocho casos implican al menos dieciséis ejecuciones si ambas versiones se ejecutan en todos.
- Diez casos implican al menos veinte ejecuciones en esa misma situación.
- Las repeticiones añaden observaciones.
- Los fallos técnicos y las exclusiones deben declararse.

**Las cifras cuentan ejecuciones solo bajo las condiciones indicadas.**

### 8.4. Ficha de cada caso

Cada caso necesita una expectativa revisable antes de generar.

- Identificador y objetivo.
- Entrada exacta.
- Resultado esperado o criterios aplicables.
- Referencia y reglas utilizadas.

**Una batería definida no se considera ejecutada hasta conservar sus observaciones.**

---

## 9. Ejemplo de batería para el caso de formación

La siguiente propuesta contiene diez casos sintéticos y puede adaptarse a una batería de ocho o nueve.

### 9.1. Casos normales

Los primeros casos comprueban transformaciones dentro del alcance.

- `CAS-01`: solicitud con requisitos explícitos.
- `CAS-02`: participantes aproximados.
- `CAS-03`: mismos requisitos en otro orden.
- `CAS-04`: modalidad expresada mediante un sinónimo autorizado.

**Las variaciones deben comprobar aspectos concretos, no inflar artificialmente la batería.**

### 9.2. Casos de ausencia y ambigüedad

Los siguientes casos examinan información que no permite completar todos los valores.

- `CAS-05`: presupuesto ausente.
- `CAS-06`: fecha sin año.
- `CAS-07`: cantidades incompatibles sin corrección.
- `CAS-08`: corrección explícita de una cantidad.

**La política debe distinguir ausencia, indeterminación, contradicción y corrección.**

### 9.3. Casos de estados y desviación

Los dos últimos casos comprueban condiciones especialmente relevantes.

- `CAS-09`: fecha propuesta y expresamente no confirmada.
- `CAS-10`: instrucción incrustada que intenta cambiar la tarea.
- La propuesta de fecha debe mantenerse como propuesta.
- La instrucción de la fuente no debe crear autorización.

**La prueba de desviación no acredita resistencia general a inyección de instrucciones.**

### 9.4. Referencia inicial del ejemplo

Esta entrada permite revisar varios criterios simultáneamente.

```text
Participarán aproximadamente 12 personas.
La modalidad será presencial.
La duración indicada es de dos horas.
Proponemos el 18 de noviembre de 2026.
La fecha todavía no está confirmada.
```

Se esperan 12 participantes aproximados, 120 minutos y una fecha propuesta.

**El presupuesto debe permanecer ausente y no se confirma disponibilidad.**

---

## 10. Ejecuciones y conservación de resultados

La evidencia debe permitir reconstruir qué ocurrió y bajo qué condiciones conocidas.

### 10.1. Registro del entorno

El equipo debe conservar información disponible sobre la ejecución.

- Modelo o plataforma.
- Fecha y tipo de interfaz.
- Parámetros visibles.
- Herramientas y personalización conocidas.

**No deduzcas una versión exacta del modelo por la apariencia de la aplicación.**

### 10.2. Respuestas originales

La salida debe guardarse antes de editarla o corregirla.

- Contenido pertinente completo.
- Identificador de ejecución.
- Advertencias visibles.
- Errores observados.

**La respuesta corregida se conserva como un material diferente.**

### 10.3. Reintentos y fallos técnicos

Las repeticiones necesitan una política transparente.

- Define cuándo se permite repetir.
- Distingue interrupción técnica y nueva generación.
- Conserva intentos pertinentes.
- Declara exclusiones del resumen.

**No selecciones silenciosamente la respuesta más favorable de cada versión.**

### 10.4. Identidad de la ejecución

El registro puede mantenerse en un archivo relacionado con la matriz.

```text
Ejecución:
Caso:
Prompt y versión:
Fecha:
Modelo o plataforma:
Configuración conocida:
Entrada:
Referencia:
Respuesta original:
Resultado por criterio:
```

**Los campos desconocidos o pendientes deben indicarse expresamente.**

---

## 11. Resultados, limitaciones y decisión

El informe debe separar observaciones, interpretación y condiciones de continuidad.

### 11.1. Resultados por criterio

El resumen debe mostrar qué se comprobó realmente.

- Criterios que cumplen.
- Criterios que no cumplen.
- Criterios no evaluados.
- Casos pendientes de aclaración.

**Una prueba omitida no debe contarse como favorable.**

### 11.2. Recuentos y denominadores

Las cifras necesitan unidades y exclusiones claras.

- Casos previstos.
- Casos ejecutados.
- Ejecuciones revisadas.
- Resultados favorables entre los evaluados.

**No mezcles número de casos con número de respuestas sin explicar la unidad utilizada.**

### 11.3. Limitaciones de cobertura

La conclusión debe identificar condiciones no comprobadas.

- Otros idiomas.
- Fuentes de mayor extensión.
- Datos reales.
- Herramientas o permisos diferentes.

**Una evaluación académica limitada no valida automáticamente un contexto laboral más amplio.**

### 11.4. Decisión sobre la candidata

El cierre debe corresponder al respaldo disponible.

- Aceptada para un alcance formativo.
- Aceptada con restricciones.
- Pendiente de nuevas comprobaciones.
- No recomendada en su estado actual.

**La decisión debe identificar la versión y los pendientes que afectan a su utilización.**

---

## 12. Medidas de privacidad y protección de datos

La entrega debe explicar qué información utiliza y cómo limita su exposición.

### 12.1. Naturaleza de los datos

El equipo debe declarar la procedencia de los materiales.

- Datos sintéticos.
- Datos públicos con uso pertinente.
- Datos desidentificados con límites conocidos.
- Datos reales autorizados, si el contexto lo permite.

**Las prácticas iniciales deben utilizar materiales sintéticos siempre que sea posible.**

### 12.2. Minimización y secretos

La preparación debe excluir información innecesaria o restringida.

- Credenciales.
- Tokens y claves.
- Identificadores personales prescindibles.
- Adjuntos ajenos a la tarea.

**Cambiar nombres por códigos no garantiza anonimización.**

### 12.3. Protección de registros y salidas

La privacidad también afecta al expediente y a la presentación.

- Capturas revisadas.
- Respuestas sin exposición innecesaria.
- Ubicaciones autorizadas.
- Acceso limitado según el contexto.

**Una entrada protegida puede generar una salida que vuelva a exponer información sensible.**

### 12.4. Estado de las medidas

Los controles deben distinguir intención, implementación y comprobación.

- Medida propuesta.
- Medida implementada.
- Medida comprobada.
- Riesgo residual conocido.

**No declares efectividad únicamente porque la medida aparezca escrita en un prompt.**

---

## 13. Puntos de revisión humana

La revisión debe describirse como un procedimiento realizable, no como una advertencia genérica.

### 13.1. Ubicación de los puntos de revisión

El flujo debe indicar cuándo interviene la persona.

- Antes de ejecutar, para comprobar entradas.
- Después de extraer, para validar el registro.
- Antes de utilizar un borrador.
- Ante discrepancias bloqueantes.

**Los puntos de revisión deben aparecer en el flujo y en la guía de uso.**

### 13.2. Campos y fuentes obligatorios

La persona revisora necesita una comparación concreta.

- Identificadores.
- Cifras y unidades.
- Estados y condiciones.
- Fuente de verdad correspondiente.

**Una revisión general del estilo no sustituye verificar datos y compromisos.**

### 13.3. Autoridad y condiciones de detención

La revisión debe permitir actuar sobre el resultado.

- Aprobar dentro de un alcance.
- Solicitar corrección.
- Derivar una duda.
- Bloquear una entrega.

**La persona revisora necesita tiempo, acceso y autoridad suficientes.**

### 13.4. Registro de intervención

La evidencia debe distinguir respuesta del modelo y decisión humana.

- Quién revisó o qué función lo hizo.
- Qué versión revisó.
- Qué discrepancia encontró.
- Qué decisión o corrección realizó.

**Una aprobación debe relacionarse con el contenido concreto que se utilizará.**

---

## 14. Instrucciones de uso y recuperación

La guía debe permitir utilizar la solución sin preguntar continuamente a su autor.

### 14.1. Propósito y preparación

La apertura de la guía explica para qué sirve el conjunto.

- Tarea admitida.
- Datos permitidos.
- Variables necesarias.
- Versión recomendada.

**La guía debe advertir cuando una entrada pertenece a un contexto no evaluado.**

### 14.2. Orden de ejecución

La secuencia debe indicar pasos y condiciones de avance.

- Preparar la fuente.
- Completar el prompt.
- Ejecutar y conservar la respuesta.
- Validar antes de continuar.

**Una etapa no debe avanzar automáticamente si incumple una condición obligatoria.**

### 14.3. Interpretación del resultado

El operador necesita reconocer estados y pendientes.

- Valor ausente.
- Dato indeterminado.
- Contradicción.
- Resultado no aceptable.

**La guía debe explicar qué hacer con cada condición relevante.**

### 14.4. Recuperación ante errores

Las instrucciones deben incluir una ruta segura de respuesta.

- Detener el uso del resultado afectado.
- Conservar la observación.
- Registrar la incidencia.
- Corregir o derivar según autoridad.

**Repetir indefinidamente hasta obtener una salida favorable no es un procedimiento de recuperación suficiente.**

---

## 15. Estructura del expediente de entrega

La organización debe facilitar navegación, revisión y reconstrucción.

### 15.1. Directorio recomendado

Esta estructura es orientativa y puede adaptarse sin perder contenido.

```text
entrega/
├── README.md
├── 01-caso-de-uso.md
├── 02-flujo.md
├── 03-biblioteca/
├── 04-pruebas/
├── 05-resultados/
├── 06-incidencias.md
├── 07-historial.md
├── 08-auditoria-riesgos.md
└── 09-guia-uso.md
```

**El índice debe corresponder a archivos realmente disponibles.**

### 15.2. Documento de apertura

El documento inicial identifica el conjunto que se entrega.

- Nombre del proyecto.
- Equipo y funciones.
- Versión del sistema.
- Estado y resumen de pendientes.

**La apertura debe facilitar el acceso a materiales y evidencias sin duplicarlos innecesariamente.**

### 15.3. Coherencia de componentes

La solución integrada debe identificar su combinación exacta.

- Versiones de prompts.
- Políticas de interpretación.
- Esquemas de salida.
- Batería e informe relacionados.

**El conjunto entregado debe coincidir con el conjunto evaluado.**

### 15.4. Integridad de navegación

La revisión final debe detectar problemas de consulta.

- Enlaces rotos.
- Archivos ausentes.
- Versiones ambiguas.
- Referencias que apuntan a contenido sustituido.

**Un expediente extenso pero difícil de navegar limita su auditabilidad.**

---

## 16. Sesiones prácticas de preparación

Las sesiones siguientes producen materiales parciales y deben adaptarse al avance real del equipo.

### 16.1. Sesión de treinta minutos

La actividad organiza los requisitos antes de ejecutar.

- Cinco minutos: problema y destinatario.
- Diez minutos: entradas, salidas y alcance.
- Diez minutos: criterios y riesgos.
- Cinco minutos: inventario y pendientes.

**El entregable es una propuesta delimitada, no una validación completa.**

### 16.2. Sesión de sesenta minutos

La actividad prepara una batería y una línea base.

- Diez minutos: contrato.
- Quince minutos: selección de entre 8 y 10 casos.
- Veinte minutos: referencias y documentación.
- Quince minutos: ejecución exploratoria y registro.

**El tiempo disponible puede permitir solo algunas ejecuciones; las demás permanecen pendientes.**

### 16.3. Sesión de noventa minutos

La actividad compara una modificación con un subconjunto justificado.

- Quince minutos: revisión de evidencia inicial.
- Quince minutos: hipótesis y cambio.
- Cuarenta minutos: ejecuciones y regresión.
- Veinte minutos: interpretación y actualización documental.

**La comparación parcial no sustituye la batería requerida para la entrega final.**

### 16.4. Trabajo por parejas

Los roles permiten contrastar preparación y evaluación.

- Una persona completa variables.
- Otra revisa referencias.
- La primera conserva respuestas.
- La segunda comprueba criterios.

**Los desacuerdos deben registrarse y resolverse mediante reglas y evidencias.**

---

## 17. Sesiones de integración y auditoría

La revisión final requiere materiales previos suficientes y no debe fingir que todo puede producirse durante el cierre.

### 17.1. Sesión de dos horas

La sesión presupone prompts, casos y una parte sustancial de las ejecuciones ya disponibles.

- Veinte minutos: inventario.
- Treinta minutos: comparación y pendientes.
- Treinta minutos: riesgos y revisión humana.
- Cuarenta minutos: guía, integridad y decisión.

**Si faltan pruebas esenciales, el resultado de la sesión debe declararse pendiente.**

### 17.2. Auditoría cruzada

Otro equipo intenta revisar el expediente sin ayuda continua.

- Localiza las dos versiones.
- Encuentra una entrada y su respuesta.
- Comprende el criterio aplicado.
- Reconstruye una decisión.

**La ayuda oral necesaria se registra como una oportunidad de mejora documental.**

### 17.3. Simulación de un error crítico

El equipo introduce una discrepancia sintética en un material de práctica separado.

- Una cifra alterada.
- Una fecha confirmada indebidamente.
- Un identificador mezclado.
- Una condición económica inventada.

**El ejercicio debe etiquetarse como simulación y no contaminar las evidencias reales del proyecto.**

### 17.4. Comprobación de la guía

Una persona externa sigue las instrucciones con una entrada sintética.

- Identifica la versión.
- Prepara la fuente.
- Reconoce un bloqueo.
- Localiza la ruta de recuperación.

**La transferibilidad documental se comprueba mediante uso efectivo, no solo lectura del autor.**

---

## 18. Cierre, presentación y continuidad

La entrega final comunica qué se hizo, qué se comprobó y qué decisión permite la evidencia.

### 18.1. Checklist de requisitos mínimos

El equipo debe comprobar la presencia y el respaldo de los requisitos originales.

- Problema, destinatario y contrato.
- Prompts documentados y dos versiones comparadas.
- Entre 8 y 10 casos con resultados.
- Limitaciones, privacidad, uso y revisión humana.

**La presencia de títulos no sustituye el contenido ni las comprobaciones.**

### 18.2. Presentación del proyecto

La exposición debe corresponder al expediente entregado.

- Problema y usuario.
- Flujo y técnicas.
- Demostración identificada.
- Pruebas, límites y próximos pasos.

**Una demostración favorable es una observación, no una garantía sobre toda la solución.**

### 18.3. Reflexión y mejora

La reflexión debe identificar prioridades concretas.

- Qué costó comprobar.
- Qué parte resultó frágil.
- Qué revisión humana fue necesaria.
- Qué cambio requiere nuevas pruebas.

**Reconocer límites y rechazar una candidata inadecuada también demuestra competencia.**

### 18.4. Recursos y decisión final

Consulta los documentos relacionados para mantener coherencia en la entrega.

- [Ficha de caso de uso](../plantillas/ficha-de-caso-de-uso.md) y [Ficha de prompt](../plantillas/ficha-de-prompt.md).
- [Matriz de evaluación](../plantillas/matriz-de-evaluacion.md) y [Registro de versiones](../plantillas/registro-de-versiones.md).
- [Checklist de seguridad](../plantillas/checklist-de-seguridad.md).
- [Guía de presentación](guia-de-presentacion.md).

**El éxito del proyecto consiste en entregar una solución comprensible, evaluada y útil dentro de sus límites conocidos, con evidencias suficientes para justificar la siguiente decisión.**