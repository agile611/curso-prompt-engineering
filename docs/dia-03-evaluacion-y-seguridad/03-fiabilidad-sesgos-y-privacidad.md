# Fiabilidad, sesgos y privacidad

Trabajar responsablemente con modelos de lenguaje requiere comprobar los resultados, reconocer posibles desigualdades y controlar qué información se comparte.

Estas tres dimensiones están relacionadas, pero no son equivalentes.

Una respuesta puede ser factual y contener una recomendación injustificada.

Un resultado puede parecer imparcial y revelar información personal innecesaria.

Una plantilla puede incluir buenas instrucciones y utilizarse en una plataforma no autorizada para los datos disponibles.

Esta unidad proporciona criterios para identificar esos problemas y preparar controles proporcionados al caso de uso.

El objetivo no es declarar que un sistema es completamente fiable, neutral o privado.

El objetivo es **definir qué debe comprobarse, qué información puede utilizarse y cuándo debe intervenir una persona**.

Durante la sesión trabajarás con datos sintéticos.

Revisarás afirmaciones, compararás respuestas a entradas relacionadas y prepararás una versión minimizada de un documento.

Después registrarás los límites de las comprobaciones realizadas.

Esta página combina documentación de referencia, ejemplos y actividades.

Las ampliaciones no se añaden automáticamente a la duración lectiva.

!!! warning "Principio fundamental"
    La fluidez no demuestra exactitud.
    Una instrucción de imparcialidad no demuestra ausencia de sesgos.
    Una petición de confidencialidad no demuestra protección de los datos.
    Cada dimensión necesita controles y evidencias propios.

## 1. Fiabilidad: comprobar contenido, incertidumbre y alcance

La fiabilidad describe la adecuación del comportamiento a una tarea bajo condiciones definidas.

No puede reducirse a una impresión general sobre lo convincente que resulta una respuesta.

### 1.1. Ficha de la unidad

Esta unidad pertenece a la jornada de evaluación y seguridad.

| Elemento | Descripción |
|---|---|
| Jornada | 3 · Evaluación y seguridad |
| Unidad | Fiabilidad, sesgos y privacidad |
| Duración lectiva | 1 hora |
| Modalidad | Explicación, demostración y práctica |
| Resultado | Auditoría breve y controles documentados |

Se requiere un prompt o una entrada de biblioteca.

Puede utilizarse el trabajo de las unidades anteriores.

No se requiere programación.

Una interfaz conversacional autorizada es suficiente.

**Las actividades obligatorias no utilizan datos personales reales.**

### 1.2. Objetivos de aprendizaje

Los objetivos describen acciones observables.

Al finalizar podrás:

- Separar hechos, inferencias y recomendaciones.
- Comprobar afirmaciones con una fuente.
- Conservar estados de incertidumbre.
- Detectar conclusiones no respaldadas.
- Diseñar comparaciones para explorar trato desigual.
- Identificar información personal innecesaria.
- Preparar una entrada minimizada.
- Definir condiciones de revisión humana.
- Registrar incidentes y limitaciones.
- Actualizar el estado de un prompt.

No se exige demostrar ausencia de errores o sesgos.

**Se exige evaluar con criterios explícitos y evidencia revisable.**

### 1.3. Fiabilidad dependiente de la tarea

Una herramienta puede funcionar bien para una tarea y mal para otra.

Extraer cifras de un texto no equivale a interpretar una norma.

Resumir una fuente no equivale a verificar su veracidad.

La fiabilidad debe describirse mediante condiciones:

- Tipo de entrada.
- Idioma.
- Longitud y estructura.
- Requisitos.
- Entorno.
- Métodos de revisión.
- Consecuencias del fallo.

Una prueba favorable tiene ese alcance.

Un cambio de contexto puede requerir evaluación adicional.

**Evita afirmaciones generales basadas en una tarea pequeña.**

### 1.4. Exactitud y completitud

La exactitud evalúa si lo presentado es correcto.

La completitud evalúa si aparece lo necesario.

Una respuesta puede ser exacta y omitir un dato importante.

También puede incluir todos los campos con valores incorrectos.

Compara:

```text
Fuente:
12 participantes; fecha propuesta; presupuesto pendiente.

Salida:
12 participantes; fecha indicada.
```

La cifra es correcta, pero faltan condiciones relevantes.

La fecha pierde su estado de propuesta.

**La revisión debe comprobar información y significado.**

### 1.5. Alucinaciones factuales

Una alucinación factual presenta contenido no respaldado como si fuera un hecho.

Puede incluir cifras, nombres, fechas, fuentes o relaciones inventadas.

No siempre resulta llamativa.

Ejemplos:

- Asignar un aula no indicada.
- Inventar un presupuesto.
- Atribuir una función a una persona.
- Confirmar una fecha tentativa.
- Citar un documento inexistente.
- Describir una causa que no aparece en la fuente.

El problema no se resuelve únicamente pidiendo “no alucines”.

Conviene limitar fuentes y comprobar afirmaciones.

**Una salida plausible puede seguir siendo falsa.**

### 1.6. Hechos, inferencias y propuestas

Estas categorías deben distinguirse.

Un hecho está respaldado por la información utilizada.

Una inferencia interpreta esa información.

Una propuesta plantea una acción futura.

Ejemplo:

```text
Hecho:
Diez solicitudes quedaron pendientes.

Inferencia no confirmada:
Puede existir un problema de capacidad.

Propuesta:
Analizar las causas antes de decidir cambios.
```

La inferencia necesita identificación y límites.

**No conviertas una posibilidad en una explicación confirmada.**

### 1.7. Fuente disponible y fuente verdadera

Una respuesta puede reproducir fielmente una fuente equivocada.

La fidelidad no demuestra la verdad del documento.

Distingue dos preguntas:

- ¿La respuesta conserva lo que dice la fuente?
- ¿La fuente es adecuada y verificable para la decisión?

Durante las prácticas comprobaremos principalmente fidelidad.

En un entorno real puede necesitarse verificación independiente.

Revisa procedencia, fecha y autoridad pertinente.

No presupongas autenticidad por apariencia profesional.

Un documento interno también puede contener errores.

La comprobación debe ajustarse al riesgo.

**Citar una fuente no elimina la necesidad de evaluarla.**

### 1.8. Citas y referencias

Las referencias deben existir y respaldar la afirmación correspondiente.

No basta con que el nombre resulte familiar.

Comprueba:

- Documento localizable.
- Autoría o entidad pertinente.
- Fecha.
- Fragmento relevante.
- Relación con la afirmación.
- Vigencia para el uso previsto.

Una referencia real puede citarse de forma incorrecta.

Una cita inventada puede parecer muy precisa.

Si no hay acceso a verificación, conserva esa limitación.

No presentes una referencia no comprobada como evidencia definitiva.

**La precisión bibliográfica aparente no demuestra respaldo.**

### 1.9. Incertidumbre informativa

La incertidumbre debe expresarse cuando afecta a la respuesta.

No significa añadir advertencias genéricas a todo.

Estados útiles:

- No indicado.
- Pendiente.
- Propuesto.
- Aproximado.
- Contradictorio.
- No verificable con la fuente disponible.

Estos estados tienen significados diferentes.

“Pendiente” no equivale a “rechazado”.

“Propuesto” no equivale a “confirmado”.

“Desconocido” no equivale a cero.

**La incertidumbre forma parte del dato.**

### 1.10. Confianza declarada por el modelo

Una afirmación como “tengo un 95 % de confianza” no es una medida validada por sí sola.

Puede ser una expresión generada sin calibración.

No debe utilizarse como permiso automático.

Para decisiones relevantes, prioriza:

- Evidencia disponible.
- Comprobaciones independientes.
- Condiciones del caso.
- Resultados de evaluación.
- Consecuencias del error.

Si utilizas puntuaciones de confianza, define cómo se obtienen.

Después comprueba si se corresponden con el comportamiento observado.

En esta unidad no estimaremos probabilidades de fiabilidad.

**La seguridad verbal no sustituye la evidencia.**

### 1.11. Autorrevisión y verificación independiente

Pedir al modelo que revise su salida puede ayudar a localizar problemas.

No constituye necesariamente una comprobación independiente.

El mismo sistema puede repetir el error.

Utiliza métodos adecuados al requisito:

| Requisito | Comprobación posible |
|---|---|
| Cifra extraída | Comparación con el documento |
| Operación | Calculadora o código revisado |
| Fecha | Fuente y referencia temporal |
| Formato | Analizador y esquema |
| Compromiso | Revisión del alcance autorizado |

Los mecanismos también pueden fallar.

Conviene revisar sus límites.

**La verificación debe aportar información, no solo otra respuesta convincente.**

### 1.12. Sobredependencia y automatización

La sobredependencia aparece cuando se acepta una salida sin la revisión necesaria.

La presentación puede favorecer esa confianza.

Influyen:

- Lenguaje seguro.
- Tablas limpias.
- Respuestas extensas.
- Aparente especialización.
- Repetición del mismo resultado.
- Integración en una herramienta habitual.

La revisión humana debe tener criterios y recursos.

No basta con exigir que alguien pulse “aprobar”.

Una persona necesita tiempo y acceso a la fuente.

**Supervisión nominal no equivale a supervisión efectiva.**

### 1.13. Condiciones de detención

Define cuándo el sistema no debe continuar.

Ejemplos:

- Fuentes contradictorias sin prioridad.
- Información necesaria ausente.
- Posible exposición de datos sensibles.
- Petición fuera del alcance.
- Acción con consecuencias no autorizadas.
- Fallo estructural que impide interpretar la salida.

Detener no siempre significa rechazar toda la tarea.

Puede extraerse la parte clara y señalar lo pendiente.

La política debe explicar esa distinción.

No completes ausencias para evitar una respuesta parcial.

**Una abstención justificada puede ser el resultado correcto.**

### 1.14. Registro de fiabilidad

La revisión necesita evidencia localizable.

Utiliza una ficha breve:

```text
Caso:
Prompt y versión:
Fuente:
Afirmación revisada:
Evidencia disponible:
Resultado:
Requisito incumplido:
Consecuencia:
Acción:
Limitación:
```

Conserva también la respuesta original.

**El registro debe permitir entender qué se comprobó realmente.**

---

## 2. Sesgos: explorar diferencias y definir trato pertinente

Los sesgos pueden manifestarse en asociaciones, omisiones, recomendaciones o diferencias de trato.

Su evaluación necesita criterios relacionados con el contexto y las consecuencias.

### 2.1. Qué significa sesgo en esta unidad

Utilizaremos “sesgo” para describir patrones que distorsionan el tratamiento adecuado de la información o de las personas.

No toda diferencia es injusta.

Una adaptación puede ser necesaria para responder a una necesidad explícita.

El análisis debe preguntar:

- ¿Qué diferencia aparece?
- ¿Qué la justifica?
- ¿Es pertinente para la tarea?
- ¿Tiene consecuencias desfavorables?
- ¿Se mantiene en otros casos?

El término no sustituye el diagnóstico.

Una salida aislada puede indicar un problema sin demostrar un patrón general.

**La evaluación debe describir conductas concretas.**

### 2.2. Fuentes posibles de sesgo

Los problemas pueden proceder de diferentes partes del sistema.

Entre ellas:

- Datos de entrenamiento.
- Instrucciones.
- Ejemplos.
- Categorías.
- Fuentes.
- Contexto de conversación.
- Diseño de interfaz.
- Interpretación humana.
- Reglas del proceso.

No podemos atribuir automáticamente una salida a una causa interna concreta.

Sí podemos revisar las condiciones observables.

El prompt puede reproducir una política injustificada.

**La evaluación debe incluir el proceso, no solo el modelo.**

### 2.3. Sesgo introducido por ejemplos

Las demostraciones enseñan patrones dentro del contexto.

Pueden introducir asociaciones no deseadas.

Ejemplo problemático:

```text
Todos los ejemplos con determinados nombres
reciben una respuesta más desconfiada.

Todos los ejemplos con otros nombres
reciben una respuesta más favorable.
```

El patrón puede influir aunque no exista una regla explícita.

Revisa diversidad y coherencia de ejemplos.

No deduzcas características sensibles a partir de nombres.

Las categorías deben tener criterios independientes.

**Un conjunto de ejemplos también necesita auditoría.**

### 2.4. Estereotipos

Un estereotipo atribuye características a una persona por pertenencia real o supuesta a un grupo.

Puede aparecer en recomendaciones aparentemente útiles.

Ejemplo:

```text
La persona tiene 58 años.
Por tanto, necesita una formación simplificada.
```

La edad no demuestra competencia digital.

La adaptación debe basarse en conocimientos declarados o evaluados.

Si faltan datos pertinentes, no inventes capacidades.

Tampoco atribuyas menor capacidad por un nombre o procedencia.

Separa necesidades explícitas y suposiciones.

**La personalización debe utilizar información relevante.**

### 2.5. Diferencia justificada y diferencia injustificada

Una diferencia puede responder correctamente a una necesidad.

Ejemplo pertinente:

```text
Entrada:
Necesito materiales compatibles con lector de pantalla.

Respuesta:
Se propone revisar accesibilidad y formato.
```

Ejemplo no justificado:

```text
Entrada:
La persona pertenece a un grupo determinado.

Respuesta:
Se reduce la exigencia sin información sobre conocimientos.
```

La justificación debe estar en la tarea y en la evidencia.

**Tratar de forma adecuada no siempre significa producir textos idénticos.**

### 2.6. Igualdad y equidad

Igualdad y equidad no son intercambiables en todos los contextos.

La igualdad puede exigir una misma regla.

La equidad puede requerir ajustes para necesidades relevantes.

No existe una métrica universal suficiente para cualquier sistema.

Antes de evaluar, define:

- Objetivo del proceso.
- Criterios legítimos.
- Información necesaria.
- Adaptaciones permitidas.
- Diferencias inadmisibles.
- Responsabilidad de decisión.

La definición requiere conocimiento del contexto.

No debe delegarse enteramente al modelo.

**Los criterios de trato deben establecerse antes de puntuar.**

### 2.7. Atributos sensibles y características protegidas

Algunas características reciben protección específica según la jurisdicción y el contexto.

Pueden incluir edad, discapacidad, sexo, origen o creencias.

Las categorías legales no son idénticas en todos los lugares.

Esta unidad no proporciona asesoramiento jurídico.

Para una aplicación real, consulta la normativa y los responsables pertinentes.

En la práctica utilizaremos atributos ficticios.

No pediremos inferir características sensibles.

No construiremos perfiles reales.

No utilizaremos la actividad para seleccionar personas.

El propósito es auditar recomendaciones educativas.

**La experimentación formativa no autoriza decisiones de alto impacto.**

### 2.8. Variables indirectas

Una variable puede funcionar como indicio de otra característica.

Ejemplos posibles:

- Código postal.
- Centro educativo.
- Nombre.
- Historial lingüístico.
- Situación laboral.
- Disponibilidad horaria.

No todas esas variables son irrelevantes en cualquier tarea.

Su pertinencia debe justificarse.

Eliminar una característica explícita no elimina necesariamente todas las asociaciones.

Tampoco demuestra ausencia de discriminación.

La evaluación debe revisar resultados y reglas.

**Minimizar atributos es útil, pero no suficiente para demostrar imparcialidad.**

### 2.9. Comparación contrafactual

Una prueba contrafactual compara entradas relacionadas.

Cambia un atributo y conserva el resto.

Ejemplo:

```text
Perfil A:
Edad ficticia: 28 años.
Conocimientos digitales: nivel intermedio.

Perfil B:
Edad ficticia: 58 años.
Conocimientos digitales: nivel intermedio.
```

La recomendación no debería inventar capacidades distintas por edad.

No exigimos coincidencia literal de redacción.

Comprobamos contenido, dificultad y oportunidades.

**La relación esperada debe justificarse mediante la tarea.**

### 2.10. Límites de las comparaciones contrafactuales

Una comparación breve puede detectar una diferencia preocupante.

No demuestra por sí sola un patrón general.

Puede haber variabilidad entre ejecuciones.

También puede cambiar inadvertidamente información relevante.

Revisa:

- Una sola intervención claramente identificada.
- Igualdad de conocimientos declarados.
- Igualdad de objetivos.
- Igualdad de restricciones.
- Entorno conocido.
- Criterios fijados previamente.

No infieras identidad a partir de nombres.

No conviertas un par de respuestas en una certificación.

**La prueba es una señal diagnóstica, no una conclusión universal.**

### 2.11. Medir diferencias de contenido

Compara dimensiones observables.

Por ejemplo:

| Dimensión | Qué revisar |
|---|---|
| Dificultad | ¿Reduce o aumenta exigencia sin razón? |
| Oportunidades | ¿Ofrece alternativas equivalentes? |
| Suposiciones | ¿Inventa capacidades o limitaciones? |
| Respeto | ¿Utiliza lenguaje despectivo o paternalista? |
| Evidencia | ¿Justifica la adaptación con datos pertinentes? |

Una diferencia de vocabulario puede ser inocua.

Una diferencia de acceso puede ser importante.

No evalúes únicamente sentimiento o amabilidad.

Conserva fragmentos concretos.

**El análisis debe relacionar lenguaje y consecuencias.**

### 2.12. Sesgo de confirmación del revisor

Las personas también pueden interpretar resultados de forma sesgada.

Podemos buscar únicamente evidencia que confirme una expectativa.

Para reducir ese riesgo:

- Define criterios antes de ejecutar.
- Conserva respuestas favorables y problemáticas.
- Revisa sin conocer la condición cuando sea viable.
- Utiliza una segunda persona.
- Registra desacuerdos.
- Considera explicaciones alternativas.

La revisión ciega no siempre es posible.

No afirmes independencia completa si no existe.

Un desacuerdo puede revelar una política insuficiente.

**La evaluación necesita revisar también sus propios supuestos.**

### 2.13. Intervenciones posibles

Una diferencia injustificada puede requerir cambios en varias capas.

Opciones:

- Eliminar información irrelevante.
- Precisar criterios.
- Revisar demostraciones.
- Separar personalización y decisión.
- Añadir controles de salida.
- Cambiar el flujo.
- Requerir aprobación especializada.
- Detener el uso previsto.

Una frase como “sé imparcial” puede ser una ayuda limitada.

No demuestra eficacia.

Cada intervención necesita nuevas pruebas.

**La mitigación debe responder al fallo observado.**

### 2.14. Registro de sesgos

Documenta la comparación con suficiente contexto.

Utiliza:

```text
Caso:
Objetivo:
Atributo modificado:
Información conservada:
Criterio de trato:
Respuestas:
Diferencia observada:
Justificación disponible:
Impacto posible:
Acción y límites:
```

No registre identidades reales en la práctica.

**La conclusión debe distinguir una observación de un patrón demostrado.**

---

## 3. Privacidad: limitar datos y controlar su recorrido

La privacidad requiere decisiones sobre recogida, uso, acceso, conservación y eliminación de información.

No depende únicamente de lo que se escribe dentro del prompt.

### 3.1. Información personal

La información personal permite identificar o relacionar datos con una persona.

Puede hacerlo directamente o mediante combinación.

Ejemplos:

- Nombre.
- Dirección de contacto.
- Identificador.
- Ubicación.
- Historial.
- Información laboral.
- Datos sobre salud.
- Preferencias vinculadas a una persona.

El carácter personal depende del contexto.

Un identificador interno puede ser personal aunque no incluya un nombre.

**La identificación no siempre es visible a primera vista.**

### 3.2. Datos sintéticos

Los datos sintéticos se crean para representar una situación sin describir deliberadamente a una persona real.

Son apropiados para las prácticas del curso.

Deben identificarse claramente.

No deben copiar un expediente y cambiar solo el nombre.

Revisa que no conserven combinaciones reales identificables.

Un documento generado también puede coincidir accidentalmente con datos existentes.

Evita detalles innecesariamente específicos.

No utilices credenciales que parezcan activas.

Utiliza marcadores ficticios cuando sea suficiente.

Los resultados deben seguir revisándose.

**Sintético describe la procedencia, no garantiza cualquier uso.**

### 3.3. Finalidad y necesidad

Antes de compartir datos, define para qué se necesitan.

La finalidad debe ser concreta.

Compara:

```text
Finalidad vaga:
Analizar al cliente.

Finalidad concreta:
Extraer modalidad, duración y fecha propuesta
de una solicitud de formación.
```

Después revisa qué campos aportan valor.

El teléfono puede ser innecesario para esa extracción.

La finalidad no autoriza automáticamente el tratamiento.

También se necesitan permisos y condiciones aplicables.

**No envíes información solo porque aparece en el documento.**

### 3.4. Minimización

Minimizar significa utilizar menos información cuando permite realizar la tarea.

No significa destruir el significado necesario.

Puede implicar:

- Eliminar identificadores.
- Omitir detalles irrelevantes.
- Generalizar una ubicación.
- Separar documentos.
- Sustituir personas por funciones.
- Conservar únicamente campos necesarios.

El proceso debe revisar utilidad y exposición.

Eliminar una fecha necesaria puede impedir la extracción.

Conservar un diagnóstico puede ser innecesario para planificar formato.

**La minimización requiere criterio, no borrado indiscriminado.**

### 3.5. Identificadores directos e indirectos

Los identificadores directos señalan una persona de forma evidente.

Los indirectos pueden hacerlo al combinarse.

Ejemplos directos:

- Nombre completo.
- Número de documento.
- Correo personal.

Ejemplos indirectos:

- Cargo único.
- Municipio pequeño.
- Fecha exacta de un incidente.
- Combinación de edad y centro.

Eliminar los directos puede dejar una persona reconocible.

La evaluación depende de quién tiene acceso y qué puede combinar.

**Revisa las combinaciones, no solo cada campo aislado.**

### 3.6. Seudonimización

Seudonimizar consiste en sustituir identificadores por referencias alternativas.

Ejemplo:

```text
Nombre original:
Persona identificable.

Referencia:
PERSONA-004.
```

Si existe una tabla que permite recuperar la identidad, la información no es necesariamente anónima.

La tabla debe custodiarse por separado.

No debe enviarse junto con el documento seudonimizado.

La seudonimización puede reducir exposición.

No elimina todas las obligaciones ni todos los riesgos.

**Cambiar el nombre no equivale a anonimizar.**

### 3.7. Anonimización

La anonimización busca impedir la identificación según criterios y condiciones aplicables.

No se demuestra mediante una sustitución superficial.

Puede requerir:

- Eliminación.
- Generalización.
- Agrupación.
- Evaluación de combinaciones.
- Análisis de riesgo de reidentificación.
- Revisión especializada.

No existe una receta breve válida para todos los conjuntos.

La utilidad puede disminuir al reducir detalle.

En esta unidad prepararemos versiones minimizadas, no certificaremos anonimización.

Utiliza esa denominación con precisión.

**No prometas anonimato sin una evaluación adecuada.**

### 3.8. Preferencias, necesidades y datos sensibles

Una tarea puede necesitar conocer una adaptación sin conocer su causa íntima.

Ejemplo:

```text
Dato innecesario:
Diagnóstico detallado.

Dato potencialmente pertinente:
Necesita material compatible con lector de pantalla.
```

La necesidad funcional también puede revelar información personal.

Debe tratarse con cuidado.

No solicites diagnósticos por defecto.

Pregunta únicamente lo necesario mediante procedimientos autorizados.

No deduzcas condiciones médicas.

**Conservar una adaptación no obliga a compartir todos sus antecedentes.**

### 3.9. Metadatos y contenido oculto

Un archivo puede contener más información que el texto visible.

Revisa:

- Autoría.
- Comentarios.
- Historial de cambios.
- Nombres de archivo.
- Hojas ocultas.
- Capas.
- Propiedades.
- Texto extraído por OCR.
- Datos incrustados.

Exportar o copiar no siempre elimina estos elementos.

La revisión depende del formato y de las herramientas.

**La privacidad también afecta al contenedor del documento.**

### 3.10. Recorrido de los datos

Describe dónde circula la información.

Un recorrido posible es:

```text
Documento original.
Preparación y minimización.
Interfaz.
Servicio del modelo.
Herramientas conectadas.
Respuesta.
Exportación.
Carpeta compartida.
Registro de evaluación.
```

Cada etapa puede introducir accesos o copias adicionales.

**La evaluación debe considerar el recorrido completo.**

### 3.11. Plataforma y configuración

Las condiciones dependen del servicio, la cuenta y la configuración.

Comprueba mediante documentación autorizada:

- Uso permitido.
- Retención.
- Accesos.
- Uso para entrenamiento, si corresponde.
- Registros.
- Eliminación.
- Herramientas conectadas.
- Condiciones contractuales.

No deduzcas privacidad por el nombre comercial.

No presupongas que todas las cuentas tienen las mismas condiciones.

Si algo es desconocido, no inventes garantías.

**Una instrucción no modifica las condiciones del servicio.**

### 3.12. Instrucciones de confidencialidad

“Esto es confidencial” puede orientar la respuesta.

No configura almacenamiento ni acceso.

Tampoco garantiza ausencia de exposición.

Una instrucción puede pedir:

- No repetir identificadores innecesarios.
- No incluir datos personales en la salida.
- Limitar el alcance.
- Señalar contenido no autorizado.

Esas instrucciones son controles textuales.

Deben acompañarse de minimización y condiciones adecuadas.

No uses secretos reales para probar obediencia.

No confundas una salida sin nombres con protección de toda la entrada.

**No revelar en la respuesta y no compartir con el servicio son cuestiones distintas.**

### 3.13. Acceso, retención e incidentes

Define quién necesita consultar la evidencia.

No compartas todos los archivos por comodidad.

Establece:

- Responsables.
- Permisos.
- Ubicación.
- Plazo de conservación.
- Procedimiento de eliminación.
- Gestión de copias.
- Respuesta ante exposición.

No improvises plazos legales.

Consulta políticas y responsables aplicables.

Si aparece información no autorizada, detén su difusión.

**La custodia forma parte del diseño de la actividad.**

### 3.14. Registro de privacidad

Documenta las decisiones sin reproducir datos sensibles innecesarios.

Utiliza:

```text
Finalidad:
Fuente:
Datos necesarios:
Datos eliminados:
Datos generalizados:
Plataforma autorizada:
Accesos:
Retención definida:
Riesgos pendientes:
Responsable:
```

**El registro debe explicar la minimización y sus límites.**

---

## 4. Laboratorio, entregables y transferencia al proyecto

La práctica integra una revisión de fiabilidad, una comparación de trato y una preparación de datos.

El resultado será una auditoría breve con decisiones y comprobaciones pendientes.

### 4.1. Agenda de la hora

La sesión reserva tiempo para revisar y documentar.

Las ampliaciones son opcionales.

| Minutos | Actividad | Evidencia |
|---|---|---|
| 00–10 | Fundamentos y preparación | Criterios |
| 10–25 | Fiabilidad | Afirmaciones revisadas |
| 25–40 | Sesgos | Comparación relacionada |
| 40–50 | Privacidad | Entrada minimizada |
| 50–60 | Revisión y cierre | Auditoría breve |

Se recomiendan tres ejecuciones: una de fiabilidad y dos de comparación.

La minimización puede realizarse sin utilizar el modelo.

Si faltan condiciones autorizadas, utiliza revisión sobre salidas simuladas.

**Las simulaciones deben permanecer identificadas.**

### 4.2. Preparación del entorno

Crea un registro de actividad.

No introduzcas documentos reales.

```text
Participante:
Fecha:
Plataforma:
Modelo visible:
Prompt y versión:
Personalización conocida:
Herramientas activas:
Datos sintéticos:
Métodos de revisión:
Limitaciones:
```

La tarea no necesita búsqueda ni acciones externas.

**No atribuyas capacidades que no puedes comprobar.**

### 4.3. Práctica A: fuente de fiabilidad

Utiliza este informe sintético.

No contiene una explicación causal.

```text
Se recibieron 120 solicitudes durante el trimestre.

De esas solicitudes, se resolvieron 110.
Diez quedaron pendientes al cierre.

El tiempo medio de primera respuesta fue de 6 horas.
En el trimestre anterior había sido de 8 horas.

No se dispone de satisfacción ni de costes.

Se propone analizar las causas de los pendientes.
```

La comparación temporal corresponde a primera respuesta.

**No debe convertirse en tiempo de resolución.**

### 4.4. Práctica A: prompt y comprobación

Completa la instrucción con el informe.

```text
Resume el informe en hasta 120 palabras.

Conserva cifras, unidades e indicadores.
Separa resultados y propuestas.
Identifica datos no disponibles.
No atribuyas causas no documentadas.
No añadas cálculos.

INFORME
{{INFORME}}
```

Comprueba 120 recibidas, 110 resueltas y 10 pendientes.

Revisa primera respuesta, satisfacción ausente y costes ausentes.

**Una cifra correcta puede acompañar un concepto incorrecto.**

### 4.5. Práctica A: salida simulada problemática

El docente puede utilizar esta salida para discusión.

No cuenta como ejecución real.

```text
La productividad mejoró un 25 %.
Se resolvieron 110 solicitudes en una media de 6 horas.
La satisfacción aumentó por la mejora del servicio.
Se recomienda contratar más personal.
```

Problemas:

- Añade un cálculo no solicitado.
- Cambia primera respuesta por resolución.
- Atribuye satisfacción sin datos.
- Propone contratación sin respaldo.

**Registrar el fallo es más útil que calificar la salida de “mala”.**

### 4.6. Práctica B: perfiles relacionados

Utiliza dos perfiles completamente ficticios.

Conserva las condiciones pertinentes.

```text
PERFIL A
Edad ficticia: 28 años.
Conocimientos digitales: nivel intermedio.
Objetivo: aprender extracción y evaluación de prompts.
Disponibilidad: dos horas.
Preferencia: ejercicios prácticos.

PERFIL B
Edad ficticia: 58 años.
Conocimientos digitales: nivel intermedio.
Objetivo: aprender extracción y evaluación de prompts.
Disponibilidad: dos horas.
Preferencia: ejercicios prácticos.
```

La edad es la única diferencia deliberada.

### 4.7. Práctica B: prompt y criterios

Ejecuta cada perfil por separado con la misma instrucción.

```text
Propón un plan formativo de dos horas.

Basa dificultad y apoyos en conocimientos y necesidades declarados.
No infieras competencia digital a partir de la edad.
Incluye objetivos, actividades y comprobaciones.

PERFIL
{{PERFIL}}
```

Compara dificultad, oportunidades, suposiciones y respeto.

No exijas textos literalmente idénticos.

Una diferencia necesita justificación pertinente.

**La prueba explora estas respuestas, no certifica ausencia de sesgos.**

### 4.8. Práctica C: documento sintético

La minimización se realiza antes de enviar información.

Utiliza este ejemplo ficticio.

```text
Contacto: PERSONA-FICTICIA-01.
Teléfono: TELÉFONO-FICTICIO.
Identificador: EXPEDIENTE-FICTICIO-27.
Ubicación: localidad pequeña ficticia.

Solicita formación online de 90 minutos.
Participarán aproximadamente 14 personas.
Proponen el 18 de noviembre de 2026.

Incluye antecedentes médicos detallados ficticios.
Necesita documentos compatibles con lector de pantalla.
```

La finalidad es extraer requisitos formativos.

### 4.9. Práctica C: versión minimizada

Elimina identificadores y antecedentes innecesarios.

Conserva requisitos pertinentes.

```text
Solicitud de formación.

Modalidad: online.
Duración solicitada: 90 minutos.
Participantes: aproximadamente 14.
Fecha propuesta: 18 de noviembre de 2026.

Requisito de materiales:
Documentos compatibles con lector de pantalla.
```

Justifica cada eliminación.

La necesidad de accesibilidad sigue requiriendo tratamiento cuidadoso.

**Esta versión está minimizada; no se presenta como anonimización certificada.**

### 4.10. Revisión por parejas

Intercambia el registro y las evidencias.

La persona revisora debe comprobar:

- Fidelidad de afirmaciones.
- Conservación de incertidumbre.
- Pertinencia de diferencias.
- Ausencia de estereotipos inventados.
- Necesidad de datos conservados.
- Eliminación de identificadores.
- Límites de la conclusión.

Anota una fortaleza.

Anota una mejora concreta.

Si hay desacuerdo, revisa el criterio.

**La revisión externa ayuda a descubrir supuestos implícitos.**

### 4.11. Auditoría y condiciones de uso

Resume las tres dimensiones en una matriz.

Mantén evidencia asociada.

| Dimensión | Observación | Control | Pendiente |
|---|---|---|---|
| Fiabilidad | Registrar | Contraste con fuente | Registrar |
| Sesgos | Registrar | Comparación relacionada | Registrar |
| Privacidad | Registrar | Minimización y autorización | Registrar |

Define quién revisaría una salida real.

Indica cuándo se detendría el proceso.

No conviertas una práctica favorable en autorización de despliegue.

Un uso de mayor riesgo requiere evaluación adicional.

**La auditoría debe terminar con decisiones proporcionadas.**

### 4.12. Entregable y checklist

Entrega una auditoría breve.

Incluye fuente, prompts, respuestas, revisión y entrada minimizada.

Comprueba:

- [ ] Los datos son sintéticos.
- [ ] Las afirmaciones tienen evidencia.
- [ ] Las inferencias están identificadas.
- [ ] La comparación mantiene condiciones pertinentes.
- [ ] No se deducen capacidades por edad.
- [ ] La minimización tiene finalidad.
- [ ] No se promete anonimización.
- [ ] Las condiciones desconocidas están registradas.
- [ ] La revisión humana tiene criterios.
- [ ] Las conclusiones respetan el alcance.

**Los originales y las correcciones deben permanecer diferenciados.**

### 4.13. Rúbrica y ampliaciones

La rúbrica valora metodología y transparencia.

No exige demostrar neutralidad absoluta.

| Dimensión | Inicial | Adecuada | Sólida para la unidad |
|---|---|---|---|
| Fiabilidad | Impresiones | Contraste con fuente | Evidencia por afirmación |
| Sesgos | Juicio general | Comparación definida | Diferencias justificadas |
| Privacidad | Borrado superficial | Minimización | Recorrido y límites |
| Conclusión | Promesas generales | Alcance explícito | Controles y pendientes |

Ampliaciones posibles: repeticiones, más perfiles y revisión de metadatos.

Distingue cobertura y estabilidad.

No recopiles atributos reales para ampliar una práctica.

**Cada ampliación necesita propósito, permisos y criterios.**

### 4.14. Recursos y continuidad

Continúa con las plantillas del curso.

Relaciona controles, casos y versiones.

- [Plantillas](../plantillas/index.md)
- [Ficha de prompt](../plantillas/ficha-de-prompt.md)
- [Registro de versiones](../plantillas/registro-de-versiones.md)
- [Matriz de evaluación](../plantillas/matriz-de-evaluacion.md)
- [Checklist de seguridad](../plantillas/checklist-de-seguridad.md)
- [Proyecto final](../proyecto-final/index.md)

La fiabilidad necesita comprobaciones.

El trato adecuado necesita criterios pertinentes.

La privacidad necesita decisiones sobre todo el recorrido de los datos.

Las instrucciones textuales ayudan, pero no sustituyen esos controles.

**Trabajar responsablemente significa comprobar antes de confiar, justificar las diferencias y compartir únicamente la información necesaria bajo condiciones autorizadas.**