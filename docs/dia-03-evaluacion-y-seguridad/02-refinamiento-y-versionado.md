# Refinamiento y versionado

Refinar un prompt consiste en modificar su diseño para resolver un problema observado o incorporar un requisito justificado.

Versionar consiste en identificar y conservar esos diseños para saber qué se utilizó, qué cambió y por qué.

Ambas prácticas permiten mejorar una instrucción sin perder la relación entre requisitos, pruebas y resultados.

No basta con añadir frases hasta obtener una respuesta satisfactoria.

Necesitamos formular una hipótesis, comprobar sus efectos y revisar si aparecen nuevos fallos.

También necesitamos distinguir entre corregir una respuesta y corregir el proceso que la produjo.

Esta unidad continúa el trabajo iniciado en diseño de pruebas.

Utilizarás un fallo documentado como punto de partida para preparar una nueva versión.

Después comprobarás el caso afectado y ejecutarás pruebas de regresión.

El objetivo no es encontrar una instrucción definitiva.

El objetivo es **mantener una evolución trazable, evaluada y proporcionada al uso previsto**.

!!! info "Duración y alcance"
    La sesión lectiva dura una hora.
    Esta página incluye documentación ampliada y prácticas opcionales.
    Durante la sesión se realiza un ciclo breve de refinamiento.
    No se exige validar un sistema para producción ni completar todas las ampliaciones.

## 1. Fundamentos: mejorar sin perder la trazabilidad

Esta sección establece qué significa refinar y cómo documentar una evolución que pueda revisarse.

La calidad del cambio depende de su justificación y de la evidencia que lo acompaña.

### 1.1. Ficha de la unidad

La unidad pertenece al tercer del curso.

| Elemento | Descripción |
|---|---|
| Jornada | 3 · Evaluación y seguridad |
| Unidad | Refinamiento y versionado |
| Duración lectiva | 1 hora |
| Modalidad | Explicación, demostración y práctica |
| Resultado | Nueva versión evaluada y registro de decisión |

Se requiere un prompt documentado y una batería inicial de pruebas.

Puede utilizarse el trabajo de la unidad anterior.

No se requiere programación.

Los ejemplos utilizan datos ficticios.

**La evaluación considera tanto la modificación como su comprobación.**

### 1.2. Objetivos de aprendizaje

Los objetivos describen acciones observables.

Al finalizar podrás:

- Identificar un problema respaldado por una ejecución.
- Separar observación e hipótesis.
- Proponer un cambio relacionado con un requisito.
- Conservar una versión inicial.
- Registrar diferencias entre versiones.
- Comprobar el fallo que motivó el cambio.
- Ejecutar pruebas de regresión.
- Reconocer mejoras locales y deterioros.
- Decidir si conservar, revisar o descartar la modificación.
- Actualizar una entrada de biblioteca.

No se exige demostrar una mejora en todos los casos.

**Un cambio descartado con evidencia también representa aprendizaje.**

### 1.3. Qué significa refinar

Refinar es revisar un diseño para mejorar su adecuación a la tarea.

Puede implicar añadir, eliminar, reorganizar o precisar instrucciones.

El punto de partida debe ser un problema o una necesidad identificada.

Ejemplos de refinamiento:

- Aclarar una regla de prioridad.
- Definir un estado que faltaba.
- Eliminar requisitos incompatibles.
- Corregir una demostración.
- Precisar un esquema.
- Reducir contexto irrelevante.
- Separar operaciones difíciles de revisar.

Una instrucción más larga no es necesariamente mejor.

Una instrucción más breve tampoco lo es.

**La mejora depende del cumplimiento y del uso, no de la longitud.**

### 1.4. Qué significa versionar

Versionar es identificar diseños distintos y conservar su relación.

Una versión debe permitir recuperar el contenido exacto utilizado.

También debe relacionarse con las pruebas correspondientes.

El registro responde a preguntas concretas:

- ¿Qué instrucciones se enviaron?
- ¿Qué políticas estaban vigentes?
- ¿Qué ejemplos se incluyeron?
- ¿Qué esquema se solicitó?
- ¿Qué resultados se obtuvieron?
- ¿Qué cambió después?

Un nombre como `final-definitivo` no responde suficientemente.

La numeración necesita una convención.

**La versión identifica un diseño; no certifica su calidad.**

### 1.5. Corrección de salida y refinamiento de prompt

Corregir una salida resuelve un resultado concreto.

Refinar el prompt modifica las condiciones de futuras ejecuciones.

Son acciones diferentes.

```text
Corrección de salida:
Cambiar manualmente "confirmada" por "propuesta".

Refinamiento:
Precisar la política para que las fechas tentativas
se representen como propuestas.
```

Ambas acciones pueden ser necesarias.

La corrección manual debe quedar identificada.

No debe presentarse como una respuesta generada correctamente.

**Reparar una respuesta no demuestra que el fallo haya dejado de producirse.**

### 1.6. Cambio de diseño y cambio de requisito

Un refinamiento puede mantener la tarea original.

También puede aparecer porque la tarea ha cambiado.

Conviene distinguir ambas situaciones.

Ejemplo de refinamiento:

```text
La política ya exigía conservar aproximaciones.
Se aclara cómo representarlas.
```

Ejemplo de cambio de requisito:

```text
La aplicación ahora necesita distinguir
participantes mínimos y máximos.
```

El segundo caso puede requerir un esquema nuevo.

No debe evaluarse como si la tarea fuera idéntica.

**Una nueva necesidad puede justificar una evolución más amplia.**

### 1.7. Observación, hipótesis y conclusión

Estos elementos deben registrarse por separado.

La observación describe lo que ocurrió.

La hipótesis propone una explicación o una intervención.

La conclusión resume lo comprobado.

```text
Observación:
Una corrección explícita fue marcada como contradicción.

Hipótesis:
La regla de prioridad no distingue correcciones autorizadas.

Conclusión posible:
La nueva regla resolvió este caso y mantuvo
el cumplimiento en los casos de regresión ejecutados.
```

La conclusión no debe anticiparse a las pruebas.

**Describir el comportamiento evita inventar causas internas del modelo.**

### 1.8. Diagnóstico antes de modificar

Un fallo puede proceder de distintos elementos.

No asumas automáticamente que falta una frase en el prompt.

Revisa:

- La fuente.
- La referencia de evaluación.
- El requisito.
- La plantilla completada.
- El contexto de conversación.
- El esquema.
- Las herramientas.
- El procedimiento de copia.
- La propia interpretación del revisor.

Una referencia equivocada puede producir un falso fallo.

Una entrada incompleta puede impedir la respuesta solicitada.

**El diagnóstico debe incluir el proceso completo.**

### 1.9. Evidencia mínima para iniciar un cambio

Un cambio necesita una razón revisable.

La evidencia mínima incluye:

- Caso.
- Entrada.
- Prompt completo.
- Versión.
- Respuesta original.
- Requisito incumplido.
- Referencia.
- Consecuencia prevista.

No basta con escribir “a veces falla”.

Tampoco basta con decir “suena poco profesional”.

Si el problema es expresivo, define el rasgo que incumple.

**La evidencia convierte una preferencia difusa en una intervención justificable.**

### 1.10. Mejora local y mejora general

Resolver un caso es una mejora local.

No demuestra que todas las entradas similares funcionen.

Una nueva versión puede:

- Resolver el caso original.
- Fallar en una variante.
- Introducir una regresión.
- Aumentar el coste.
- Dificultar el mantenimiento.

La evaluación debe explorar estos efectos.

No necesitamos probar todo el mundo posible.

Sí necesitamos declarar el alcance de lo observado.

La siguiente prueba debe responder a una incertidumbre concreta.

**La generalización requiere evidencia adicional.**

### 1.11. Regresión

Una regresión es un deterioro respecto a un comportamiento anterior.

Puede aparecer después de un cambio aparentemente beneficioso.

Ejemplo:

```text
Antes:
Los conflictos no resueltos se marcaban como contradictorios.

Después:
La regla nueva elige siempre la última cifra.
```

El cambio podría resolver correcciones explícitas y romper conflictos reales.

Por eso necesitamos casos de regresión.

Estos casos comprueban comportamientos que deben conservarse.

No son necesariamente una evaluación reservada independiente.

**Corregir un fallo no debe ocultar los nuevos.**

### 1.12. Repetición y estabilidad

Repetir un caso ayuda a observar variabilidad.

No amplía por sí sola la cobertura de situaciones.

Un caso ejecutado tres veces sigue siendo un caso.

Las repeticiones pueden mostrar:

- Consistencia.
- Fallos intermitentes.
- Cambios de formato.
- Variación de estados.
- Sensibilidad al entorno.

Conserva todas las ejecuciones.

No selecciones únicamente la mejor.

La estabilidad observada sigue limitada a esas condiciones.

**Distingue diversidad de casos y consistencia entre repeticiones.**

### 1.13. Costes y complejidad

Un refinamiento puede mejorar calidad y aumentar trabajo.

Considera:

- Longitud de instrucciones.
- Cantidad de ejemplos.
- Número de etapas.
- Tiempo de revisión.
- Dependencias.
- Coste de ejecución.
- Facilidad de actualización.

No inventes precios ni mediciones.

Distingue observaciones y estimaciones.

Una mejora pequeña puede no justificar una arquitectura complicada.

**La decisión debe valorar el proceso completo.**

### 1.14. Principio de cambio proporcionado

Empieza con una intervención relacionada con el fallo.

Evita añadir todas las técnicas disponibles.

Un cambio proporcionado puede ser:

- Una definición.
- Una excepción explícita.
- Una demostración revisada.
- Una corrección del esquema.
- Una separación de etapas.

Si varios elementos deben cambiar conjuntamente, documéntalo.

No atribuyas después todo el efecto a una sola frase.

El objetivo es mejorar con control suficiente.

**Refinar significa tomar decisiones, no acumular instrucciones.**

---

## 2. Método: preparar versiones, pruebas y decisiones

Esta sección organiza un ciclo de refinamiento reproducible.

El método puede realizarse con archivos de texto y una tabla de registro.

### 2.1. Definir la unidad versionada

Antes de numerar, decide qué constituye una versión.

Puede ser:

- Una plantilla.
- Un conjunto de instrucciones y ejemplos.
- Un esquema.
- Un flujo.
- Una configuración de aplicación.

En esta unidad versionaremos una plantilla con sus políticas.

El esquema permanecerá constante durante el cambio principal.

Los casos y las referencias tendrán identificadores propios.

La evaluación relacionará esos elementos.

No mezcles versiones de prompt y casos sin explicarlo.

**La unidad versionada debe ser reconocible.**

### 2.2. Conservar una línea base

La línea base es el diseño anterior al cambio.

Debe guardarse sin sobrescribir.

Conserva:

- Contenido exacto.
- Identificador.
- Versión.
- Fecha.
- Estado.
- Dependencias.
- Evidencias disponibles.

Si no puedes recuperar lo utilizado, registra esa limitación.

No reconstruyas una supuesta versión inicial de memoria.

Puedes crear una nueva línea base documentada.

Pero debe identificarse como tal.

**La comparación necesita saber de dónde parte.**

### 2.3. Elegir una convención de versiones

Una convención sencilla es suficiente para el curso.

Utilizaremos números incrementales.

```text
0.1:
Primera versión documentada.

0.2:
Primera modificación evaluada.

0.3:
Nueva revisión posterior.
```

La numeración no representa un porcentaje de madurez.

El número `1.0` no implica aprobación profesional.

Puedes utilizar otra convención si está definida.

Mantén consistencia dentro de la biblioteca.

**El significado debe estar documentado, no supuesto.**

### 2.4. Identificadores estables

El identificador de la entrada permanece aunque cambie la versión.

Ejemplo:

```text
Entrada: P-002
Nombre: Extraer requisitos de formación
Versión: 0.1

Entrada: P-002
Nombre: Extraer requisitos de formación
Versión: 0.2
```

No reutilices el identificador para otra tarea.

Si el propósito cambia sustancialmente, considera una entrada nueva.

Relaciona la procedencia de esa entrada.

El nombre puede evolucionar si sigue siendo descriptivo.

**La estabilidad facilita seguir el historial.**

### 2.5. Registrar una solicitud de cambio

La solicitud describe qué se pretende resolver.

No necesita un sistema complejo.

```text
ID del cambio:
Entrada:
Versión de origen:
Problema:
Caso y evidencia:
Requisito afectado:
Impacto:
Hipótesis:
Intervención propuesta:
Comprobaciones:
```

No escribas la solución antes de entender el problema.

**La solicitud conecta necesidad, modificación y evaluación.**

### 2.6. Formular una hipótesis comprobable

La hipótesis debe anticipar un comportamiento observable.

Ejemplo:

```text
Si distinguimos correcciones explícitas de notas posteriores,
el sistema debería aceptar una cifra corregida
sin elegir arbitrariamente en conflictos no resueltos.
```

La hipótesis incluye una mejora y una condición de conservación.

Puede resultar falsa.

También puede ser parcialmente correcta.

Define qué evidencia la apoyaría.

Define qué evidencia justificaría descartarla.

No atribuyas motivaciones internas al modelo.

**La hipótesis orienta pruebas, no determina resultados.**

### 2.7. Diseñar el cambio mínimo

El cambio mínimo es la intervención suficiente para explorar la hipótesis.

No necesariamente es una única palabra.

Puede ser una regla y su aclaración.

Antes de editar, identifica:

- Sección afectada.
- Texto anterior.
- Texto propuesto.
- Elementos que permanecen iguales.
- Riesgos de la modificación.

Evita cambiar simultáneamente rol, formato y ejemplos sin necesidad.

Si lo haces, registra la intervención combinada.

La atribución causal será más limitada.

**La comparación gana claridad cuando las diferencias son explícitas.**

### 2.8. Mostrar diferencias

Una comparación textual facilita revisar el cambio.

Puedes utilizar una tabla o un bloque `diff`.

```diff
- Si aparecen varias cifras, utiliza la última.
+ Utiliza una cifra posterior solo si la fuente
+ identifica explícitamente que corrige o sustituye la anterior.
+ Si no hay prioridad válida, conserva la contradicción.
```

Este ejemplo muestra una política modificada.

No supone que la versión inicial fuera adecuada.

El historial debe explicar el motivo.

No es necesario utilizar Git para mostrar diferencias.

**Una diferencia visible reduce cambios inadvertidos.**

### 2.9. Mantener constantes las condiciones

Para comparar versiones, conserva lo que puedas controlar.

Mantén:

- Caso.
- Referencia.
- Esquema.
- Formato.
- Modelo visible.
- Herramientas.
- Condiciones conocidas.
- Método de revisión.

Una conversación nueva puede seguir incluyendo personalización.

No afirmes aislamiento completo sin evidencia.

Si cambia el entorno, registra el cambio.

La comparación sigue siendo informativa, pero más limitada.

**Las condiciones desconocidas deben aparecer en la conclusión.**

### 2.10. Seleccionar pruebas de regresión

Elige casos que representen comportamientos relevantes.

No necesitas repetir todos los casos disponibles en la sesión.

Prioriza:

- El campo afectado.
- Una situación que antes cumplía.
- Una excepción cercana.
- Un conflicto no resuelto.
- Un requisito crítico.

La selección debe justificarse antes de observar resultados.

No elijas solo pruebas fáciles.

No cambies referencias para favorecer la nueva versión.

Los casos anteriores conservan su función de regresión.

**La batería debe buscar también deterioros.**

### 2.11. Reservar una prueba nueva

Una prueba nueva puede explorar transferencia.

Debe definirse antes de ejecutar la versión candidata.

Idealmente, otra persona mantiene su referencia.

Si el diseñador ya ha estudiado todo el material, documenta esa exposición.

No llames independiente a una prueba utilizada para ajustar.

Una variante nueva ofrece evidencia adicional.

No demuestra generalización amplia.

Su dificultad debe relacionarse con el cambio.

Evita una entrada artificialmente favorable.

**La reserva protege la interpretación, no garantiza representatividad.**

### 2.12. Definir condiciones de aceptación

La aceptación debe acordarse antes de evaluar.

Para una práctica breve puede requerir:

- Resolver el fallo observado.
- Mantener los casos de regresión ejecutados.
- No introducir desviaciones críticas.
- Conservar el esquema.
- Documentar límites.

Cumplir esas condiciones permite conservar una candidata.

No autoriza automáticamente producción.

Si falta evidencia, puede mantenerse en revisión.

La aceptación debe corresponder al uso previsto.

No conviertas una media en permiso automático.

**Una mejora local puede merecer conservación provisional.**

### 2.13. Decidir: conservar, revisar o descartar

La decisión debe describir el resultado del cambio.

Posibles decisiones:

| Decisión | Situación |
|---|---|
| Conservar como candidata | Mejora observada sin regresiones en lo ejecutado |
| Revisar | Resultado parcial o evidencia insuficiente |
| Descartar | No aporta mejora o introduce fallos inaceptables |
| Escalar | Requiere modificar datos, esquema o flujo |
| Revertir | Una versión adoptada presenta deterioro relevante |

La decisión no necesita un ganador obligatorio.

Puede concluir que el prompt no es la solución adecuada.

Registra qué versión queda recomendada.

Conserva también la alternativa descartada cuando aporta evidencia.

**La decisión debe poder revisarse después.**

### 2.14. Historial, responsables y dependencias

Cada cambio debe relacionarse con quien lo documentó.

Incluye:

- Fecha.
- Autor.
- Revisor, si existe.
- Motivo.
- Diferencia.
- Pruebas.
- Resultado.
- Estado.
- Dependencias afectadas.

No inventes una aprobación inexistente.

En una práctica individual, indica que no hubo revisión externa.

Si cambia el esquema receptor, registra su versión.

**La trazabilidad incluye personas, documentos y condiciones.**

---

## 3. Laboratorio: corregir una regla sin romper los conflictos

La práctica principal trabaja con una tarea de extracción de participantes.

El cambio busca distinguir una corrección explícita de una contradicción no resuelta.

### 3.1. Agenda de la hora

La sesión combina diagnóstico, modificación y comprobación.

Las ampliaciones quedan fuera del recorrido obligatorio.

| Minutos | Actividad | Evidencia |
|---|---|---|
| 00–10 | Fundamentos y preparación | Línea base |
| 10–20 | Fallo y diagnóstico | Solicitud de cambio |
| 20–30 | Versión candidata | Diferencia registrada |
| 30–45 | Reejecución y regresión | Respuestas y matriz |
| 45–55 | Revisión por parejas | Incidencias |
| 55–60 | Decisión y entrega | Historial actualizado |

Se recomiendan cinco ejecuciones básicas.

Puede añadirse una prueba nueva si el tiempo lo permite.

No elimines la revisión para ejecutar más.

**El resultado principal es un ciclo completo documentado.**

### 3.2. Situación de trabajo

Un equipo ficticio organiza solicitudes de formación.

Necesita recuperar el número de participantes.

Algunas solicitudes contienen cifras anteriores y correcciones posteriores.

Otras contienen cifras incompatibles sin resolución.

El sistema debe distinguir esas situaciones.

No debe elegir siempre la última cifra.

Tampoco debe marcar como conflicto una corrección explícita válida.

La salida se utilizará como ficha interna.

No aprobará condiciones comerciales.

No enviará comunicaciones.

**El propósito es conservar información y certeza.**

### 3.3. Esquema del laboratorio

Utilizaremos un objeto JSON pequeño.

Debe contener únicamente estas claves.

```text
participantes:
  entero no negativo o null

estado:
  exacto | aproximado | no_indicado | contradictorio

evidencia:
  fragmento literal breve de la fuente

alertas:
  lista que puede contener participantes_contradictorios
```

La lista estará vacía si no hay contradicción pendiente.

No se permiten alertas duplicadas.

El esquema se mantendrá entre versiones.

**La comparación modifica una política, no la estructura.**

### 3.4. Política objetivo

La política correcta se define antes de ejecutar.

Sus reglas son:

- Número inequívoco: conservarlo.
- Aproximación explícita: marcar `aproximado`.
- Número ausente: utilizar `null` y `no_indicado`.
- Cifras incompatibles sin prioridad: utilizar `null` y `contradictorio`.
- Corrección explícita: utilizar el valor que sustituye al anterior.
- Posición posterior sin corrección: no concede prioridad por sí sola.

La evidencia debe permitir revisar la decisión.

Si hay conflicto, debe incluir ambos valores.

Si hay corrección, debe incluir su formulación.

**La referencia representa esta política, no el comportamiento inicial.**

### 3.5. Versión inicial 0.1

Esta versión contiene una regla incompleta.

Se utiliza deliberadamente como material de diagnóstico.

```text
Extrae el número de participantes de la solicitud.

Devuelve únicamente JSON con:
participantes, estado, evidencia y alertas.

Utiliza únicamente la fuente.
Conserva aproximaciones.
Si no hay número, utiliza null y "no_indicado".

Si aparecen cifras diferentes, utiliza null y "contradictorio".
Añade "participantes_contradictorios" a alertas.
En los demás casos, utiliza una lista vacía.

SOLICITUD
{{SOLICITUD}}
```

### 3.6. Identificar la limitación de 0.1

La versión inicial trata todas las cifras diferentes del mismo modo.

No distingue una corrección explícita.

Su regla puede entrar en conflicto con la política objetivo.

Esa limitación es observable en el texto.

No necesitamos atribuir una causa interna al modelo.

El prompt puede producir una respuesta aceptable pese a la omisión.

También puede seguir literalmente la regla incompleta.

Por eso ejecutaremos el caso afectado.

Si no aparece el fallo, no debemos inventarlo.

La omisión sigue siendo una cuestión de diseño.

**Una deficiencia documental y un fallo de ejecución son evidencias distintas.**

### 3.7. Caso F-01: corrección explícita

Este caso motiva el refinamiento.

Sustituye el marcador con el texto completo.

```text
El primer mensaje indicaba 12 participantes.

Corrección confirmada:
Serán 15 participantes.
La cifra de 15 sustituye a la anterior.
```

Resultado esperado:

- Participantes: 15.
- Estado: `exacto`.
- Evidencia: corrección y sustitución explícitas.
- Alertas: lista vacía.

No debe conservar una contradicción pendiente.

**La prioridad está respaldada por la fuente.**

### 3.8. Ejecutar y registrar F-01

Ejecuta F-01 con la versión 0.1.

Guarda la respuesta original.

Utiliza esta ficha:

```text
Caso: F-01
Versión: 0.1
Prompt completo:
Respuesta original:
Referencia:
Cumple:
Incidencias:
Condiciones conocidas:
```

Si el resultado cumple, registra cumplimiento.

No lo sustituyas por una salida simulada.

**La práctica debe conservar lo realmente observado.**

### 3.9. Salida simulada para diagnóstico

El docente puede utilizar esta salida si necesita mostrar el fallo.

Debe identificarse como simulada.

```json
{
  "participantes": null,
  "estado": "contradictorio",
  "evidencia": "12 participantes; serán 15 participantes",
  "alertas": ["participantes_contradictorios"]
}
```

Esta salida no aplica la política objetivo.

Omite que la fuente resuelve el conflicto.

No demuestra que todos los modelos produzcan ese error.

Sirve para practicar el diagnóstico.

**Una simulación enseña el método, pero no cuenta como ejecución real.**

### 3.10. Solicitud de cambio CH-01

Documenta la intervención propuesta.

Ejemplo de referencia:

```text
ID: CH-01
Entrada: P-EXTRACCION-PARTICIPANTES
Origen: versión 0.1

Problema:
La regla trata cualquier diferencia como conflicto pendiente.

Requisito:
Aplicar correcciones explícitas autorizadas por la fuente.

Hipótesis:
Una distinción entre corrección y mera aparición posterior
resolverá F-01 sin elegir arbitrariamente en conflictos reales.
```

Añade la evidencia real o identifica la simulación.

### 3.11. Diferencia propuesta

El cambio precisa la regla de prioridad.

No modifica el esquema.

```diff
- Si aparecen cifras diferentes, utiliza null y "contradictorio".
+ Si aparecen cifras diferentes:
+ - Aplica una corrección cuando la fuente identifica explícitamente
+   que un valor sustituye o corrige al anterior.
+ - No concedas prioridad solo porque una cifra aparezca después.
+ - Si no existe una prioridad explícita válida,
+   utiliza null y "contradictorio".
```

La intervención contiene varias frases relacionadas.

Su función es expresar una misma distinción.

Registra que no se añadieron demostraciones.

**La comparación sigue siendo una modificación de política.**

### 3.12. Versión candidata 0.2

Guarda la nueva versión sin sobrescribir 0.1.

Completa las reglas estructurales comunes en ambas si faltaban.

```text
Extrae el número de participantes de la solicitud.

Devuelve únicamente JSON con:
participantes, estado, evidencia y alertas.

Utiliza únicamente la fuente.
Conserva aproximaciones.
Si no hay número, utiliza null y "no_indicado".

Si hay cifras diferentes, aplica una corrección
solo cuando la fuente identifica que sustituye al valor anterior.
No elijas una cifra únicamente por aparecer después.
Si no hay prioridad explícita, utiliza null y "contradictorio"
y añade "participantes_contradictorios".

En los demás casos, alertas será una lista vacía.

SOLICITUD
{{SOLICITUD}}
```

### 3.13. Casos de regresión

Comprueba comportamientos que deben mantenerse.

Utiliza estos tres casos.

```text
R-01:
Participarán aproximadamente 20 personas.

R-02:
Una ficha indica 8 participantes y otra indica 11.
No se sabe qué cifra es correcta.

R-03:
Una nota indica 14 participantes.
Una nota posterior indica 17 participantes.
No se explica si la segunda corrige la primera.
```

R-01 evalúa aproximación.

R-02 y R-03 evalúan conflictos no resueltos.

**R-03 busca detectar una prioridad temporal indebida.**

### 3.14. Referencias, ejecución y decisión

Las referencias de regresión son:

- R-01: 20, `aproximado`, sin alertas.
- R-02: `null`, `contradictorio`, con alerta.
- R-03: `null`, `contradictorio`, con alerta.

Ejecuta F-01 y los tres casos con 0.2.

Si hay evidencias previas de 0.1, enlázalas.

Si no las hay, no afirmes comparación empírica de regresión entre versiones.

Puedes comprobar que 0.2 cumple las referencias.

Registra el alcance de esa comprobación.

Decide conservar, revisar o descartar la candidata.

No declares producción.

**Una decisión válida explica la mejora y las pruebas pendientes.**

---

## 4. Evaluación, mantenimiento y ampliaciones

Esta sección permite ampliar el ciclo y mantener la biblioteca de forma responsable.

Las actividades adicionales no se añaden automáticamente a la hora lectiva.

### 4.1. Matriz de resultados

Resume las ejecuciones sin ocultar las incidencias.

Utiliza una matriz sencilla.

| Caso | Versión | Contenido | Estructura | Incidencias |
|---|---|---|---|---|
| F-01 | 0.1 | Registrar | Registrar | Registrar |
| F-01 | 0.2 | Registrar | Registrar | Registrar |
| R-01 | 0.2 | Registrar | Registrar | Registrar |
| R-02 | 0.2 | Registrar | Registrar | Registrar |
| R-03 | 0.2 | Registrar | Registrar | Registrar |

Añade otras ejecuciones si existen.

Utiliza `No evaluado` cuando falte una comprobación.

No confíes únicamente en el resumen.

Conserva las respuestas originales.

**La matriz facilita consulta; el registro permite verificar.**

### 4.2. Prueba nueva opcional

Otra persona puede preparar una variante antes de la ejecución.

Ejemplo didáctico:

```text
En el borrador aparecen unas 30 personas.

Actualización confirmada:
La cifra corregida es aproximadamente 24.
Esta actualización sustituye la estimación anterior.
```

La referencia será 24 y `aproximado`.

No debe convertirse en exacto por aparecer “confirmada”.

Se confirma la actualización, no la precisión absoluta.

Si el diseñador ya estudió este ejemplo, no es reservado para él.

**La exposición previa debe quedar documentada.**

### 4.3. Interpretar mejoras parciales

Una versión puede resolver F-01 y fallar R-03.

Eso representa una mejora parcial con deterioro relevante.

No debe resumirse únicamente como “mejoró”.

Describe:

- Qué requisito mejoró.
- Qué requisito falló.
- Qué casos lo muestran.
- Qué consecuencias tendría.
- Qué cambio revisarías.

Una candidata puede permanecer en revisión.

También puede descartarse.

No necesitas una nueva modificación inmediata si falta tiempo.

**La interpretación debe conservar el balance de efectos.**

### 4.4. Evitar ajustes interminables

El refinamiento necesita límites.

No repitas hasta obtener una respuesta favorable y ocultes las anteriores.

Define:

- Número de ciclos previsto.
- Tiempo disponible.
- Casos mínimos.
- Condiciones de detención.
- Acción si persiste el fallo.

Puede ser necesario cambiar el esquema.

También puede ser mejor utilizar una regla programática.

O solicitar información humana.

El prompt no tiene que resolver toda la arquitectura.

**Detener el ajuste puede ser una decisión de diseño responsable.**

### 4.5. Ampliación: eliminar instrucciones redundantes

Refinar también puede significar reducir.

Selecciona una instrucción repetida o irrelevante.

Formula una hipótesis:

```text
Eliminar tres repeticiones de la misma regla
mantendrá el cumplimiento en los casos seleccionados
y facilitará el mantenimiento.
```

Conserva la versión anterior.

Ejecuta casos pertinentes.

No midas ahorro de tokens si no tienes medición.

Puedes registrar reducción de caracteres como dato distinto.

**La simplificación necesita comprobación igual que la ampliación.**

### 4.6. Ampliación: añadir una demostración

Una demostración puede comunicar una excepción difícil.

Debe ser coherente con la regla.

No utilices el caso reservado como ejemplo y mantengas su puntuación como independiente.

Crea una demostración distinta.

Revisa:

- Entrada.
- Salida.
- Estado.
- Evidencia.
- Formato.

Documenta que cambia el conjunto de ejemplos.

Mantén constantes las demás condiciones cuando sea posible.

**Añadir few-shot es una intervención que debe identificarse.**

### 4.7. Ampliación: cambiar el esquema

Algunas tareas no pueden representarse adecuadamente con el esquema actual.

Por ejemplo, un rango de participantes.

Una evolución podría añadir:

- Mínimo.
- Máximo.
- Estado de rango.
- Motivo de incertidumbre.

Eso cambia la salida y puede afectar al consumidor.

Versiona esquema y prompt.

Revisa compatibilidad.

No compares ambos objetos mediante una igualdad literal.

Define nuevos criterios.

**Un cambio estructural requiere evaluar la integración afectada.**

### 4.8. Herramientas y registro técnico

Git puede ayudar a conservar diferencias y recuperar versiones.

No es obligatorio.

Un sistema de archivos también puede funcionar.

Ejemplo de organización:

```text
P-EXTRACCION/
├── index.md
├── versiones/
│   ├── prompt-0.1.txt
│   └── prompt-0.2.txt
├── casos/
├── ejecuciones/
└── historial.md
```

No guardes credenciales en el repositorio.

**La herramienta facilita trazabilidad, pero no crea una evaluación válida.**

### 4.9. Reversión

Revertir significa volver a una versión anterior identificada.

Puede ser necesario si aparece un deterioro.

Antes de revertir, registra:

- Incidencia.
- Versión afectada.
- Versión de retorno.
- Motivo.
- Dependencias.
- Comprobaciones necesarias.

Una versión anterior también puede tener fallos.

La reversión reduce un problema concreto, no garantiza seguridad total.

No borres la versión fallida si sostiene evidencia útil.

Actualiza el índice y el estado.

**Revertir debe ser trazable y verificable.**

### 4.10. Privacidad y revisión de cambios

Los cambios pueden introducir datos sensibles.

Revisa especialmente:

- Demostraciones nuevas.
- Fragmentos de evidencia.
- Nombres.
- Direcciones.
- Rutas.
- Identificadores personales.
- Documentos adjuntos.
- Respuestas guardadas.

No uses secretos reales para probar fugas.

Utiliza marcadores sintéticos.

La seguridad no se limita al texto principal.

**El historial también debe respetar privacidad y permisos.**

### 4.11. Actualización de la biblioteca

La entrada de biblioteca debe reflejar la decisión.

Actualiza:

- Versión recomendada.
- Estado.
- Fecha.
- Motivo.
- Pruebas.
- Limitaciones.
- Pendientes.
- Alternativa anterior.

“Probado en casos documentados” es más preciso que “funciona siempre”.

Enlaza las versiones.

No elimines la relación con los resultados previos.

Una candidata puede seguir en revisión.

**La biblioteca debe mostrar qué se conoce realmente.**

### 4.12. Entregable de la unidad

Entrega un ciclo completo de refinamiento.

Debe incluir:

1. Línea base.
2. Caso o necesidad que motiva el cambio.
3. Observación e hipótesis.
4. Diferencia registrada.
5. Versión candidata.
6. Casos de comprobación.
7. Referencias.
8. Respuestas originales.
9. Matriz e incidencias.
10. Decisión.
11. Limitaciones.
12. Historial actualizado.

### 4.13. Checklist y rúbrica formativa

Revisa antes de entregar.

Marca únicamente lo demostrable.

- [ ] La versión inicial está conservada.
- [ ] El problema tiene evidencia.
- [ ] La hipótesis es comprobable.
- [ ] Las diferencias son explícitas.
- [ ] Las referencias no se adaptaron para favorecer resultados.
- [ ] El fallo original se comprobó.
- [ ] Se ejecutaron casos de regresión.
- [ ] Los originales están guardados.
- [ ] La decisión reconoce límites.
- [ ] La biblioteca está actualizada.

La rúbrica valora diagnóstico, trazabilidad, comprobación y transparencia.

**No exige una mejora obligatoria ni certifica producción.**

### 4.14. Recursos y continuidad

Continúa con las plantillas del curso.

Relaciona versiones, casos y resultados.

- [Plantillas](../plantillas/index.md)
- [Ficha de prompt](../plantillas/ficha-de-prompt.md)
- [Registro de versiones](../plantillas/registro-de-versiones.md)
- [Matriz de evaluación](../plantillas/matriz-de-evaluacion.md)
- [Checklist de seguridad](../plantillas/checklist-de-seguridad.md)
- [Proyecto final](../proyecto-final/index.md)

Refinar requiere un motivo.

Versionar requiere conservar el diseño exacto.

Verificar requiere una referencia adecuada.

Una mejora local necesita límites.

**La evolución profesional de un prompt consiste en cambiar con criterio, comprobar los efectos y conservar evidencia suficiente para explicar la decisión.**