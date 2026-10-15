# Herramientas

El entorno de trabajo del curso debe permitir diseñar prompts, ejecutar pruebas, conservar resultados y documentar decisiones.

No necesita ser complejo para resultar útil.

Una interfaz de modelo de lenguaje, un editor de texto y una hoja de cálculo son suficientes para completar el recorrido básico.

El acceso a una API, Python y Git constituye una ampliación opcional.

La elección depende de la tarea, los conocimientos del participante y las condiciones autorizadas de utilización.

Esta página explica cómo organizar ambos entornos y cómo registrar sus capacidades reales.

Incluye procedimientos de preparación, ejemplos originales y sesiones prácticas con datos sintéticos.

**El objetivo es trabajar con un entorno comprensible, controlado y documentado, no acumular herramientas.**

Los ejemplos técnicos no representan integraciones ejecutadas.

Las salidas de referencia indican expectativas docentes, no resultados observados.

Cada equipo debe conservar sus propias pruebas y declarar las condiciones desconocidas.

Las funciones de los servicios pueden cambiar.

Por eso, la documentación debe describir lo que estaba disponible durante la ejecución.

!!! info "Entorno mínimo"
    Una interfaz de LLM.
    Un editor de texto.
    Una hoja de cálculo para registrar pruebas.
    Una ubicación autorizada para conservar los materiales.

!!! info "Entorno técnico opcional"
    Acceso autorizado a una API.
    Python y un entorno virtual.
    Git para versionar materiales.
    Controles adecuados para credenciales, datos y operaciones.

!!! warning "Condición de utilización"
    La disponibilidad de una herramienta no equivale a autorización.
    No introduzcas información restringida en servicios no aprobados.
    No conectes capacidades innecesarias.
    La aceptación académica no autoriza un despliegue profesional.

---

## 1. Función del entorno de trabajo

Las herramientas deben apoyar una tarea definida y permitir revisar cómo se obtuvo cada resultado.

### 1.1. Diseñar y conservar instrucciones

El entorno necesita un lugar estable para redactar componentes.

- El editor conserva el texto completo.
- Los archivos identifican las versiones.
- Las variables se documentan antes de utilizarse.

Una conversación puede ayudar a explorar, pero no debe ser el único archivo del proyecto.

**La instrucción recomendada debe poder recuperarse sin reconstruir el historial de mensajes.**

### 1.2. Ejecutar y observar

La interfaz o la API permite producir respuestas en condiciones determinadas.

- Cada ejecución utiliza una entrada concreta.
- El resultado debe conservarse antes de editarlo.
- Las condiciones conocidas deben registrarse.

La ejecución y la evaluación son operaciones distintas.

**Obtener una respuesta no demuestra que cumpla los criterios.**

### 1.3. Comparar y decidir

La hoja de cálculo o los registros estructurados organizan las comprobaciones.

- Relacionan casos y versiones.
- Separan expectativas y observaciones.
- Hacen visibles discrepancias y pendientes.

La comparación debe utilizar referencias compatibles.

**Las herramientas facilitan el registro; la conclusión necesita criterios y evidencia.**

### 1.4. Mantener límites operativos

La configuración debe corresponder al alcance de la tarea.

- Lectura cuando no se necesita escritura.
- Datos sintéticos durante las prácticas iniciales.
- Sin envío ni modificación externa innecesarios.

Los límites deben comprobarse en la aplicación.

**Pedir al modelo que no actúe no equivale a retirar una capacidad.**

---

## 2. Elección entre entorno mínimo y técnico

La elección debe considerar utilidad, esfuerzo, riesgos y posibilidad de evaluación.

### 2.1. Cuándo basta el entorno mínimo

El entorno mínimo resulta adecuado para proyectos breves y revisables manualmente.

- Pocas versiones de prompts.
- Entradas de tamaño manejable.
- Baterías que pueden ejecutarse sin automatización.

No requiere conocimientos de programación.

**El recorrido básico debe permitir demostrar diseño, evaluación y documentación completos.**

### 2.2. Cuándo aporta valor el entorno técnico

La ampliación técnica puede reducir tareas repetitivas.

- Ejecutar varias entradas con el mismo procedimiento.
- Validar formatos de salida.
- Conservar registros estructurados.

La automatización añade configuración y mantenimiento.

**Su utilidad debe compararse con el esfuerzo total, no solo con la velocidad de generación.**

### 2.3. Comparación de alternativas

La siguiente tabla resume funciones, no recomendaciones comerciales.

| **Necesidad** | **Entorno mínimo** | **Ampliación opcional** |
|---|---|---|
| Redactar prompts | Editor de texto | Editor con validación |
| Ejecutar casos | Interfaz conversacional | API |
| Registrar pruebas | Hoja de cálculo | CSV o JSONL |
| Validar estructura | Revisión manual | Script |
| Conservar versiones | Archivos identificados | Git |

**Ambos entornos necesitan criterios, referencias y revisión proporcional al riesgo.**

### 2.4. Evitar complejidad innecesaria

Una herramienta nueva debe resolver una necesidad identificada.

- No automatizar antes de definir el contrato.
- No conectar servicios sin una función concreta.
- No adoptar Git sin comprender qué conserva.

La complejidad puede introducir nuevos errores.

**Una solución sencilla y auditable puede ser preferible a una integración difícil de revisar.**

---

## 3. Interfaz de modelo de lenguaje

La interfaz permite interactuar con el modelo, pero puede añadir condiciones que no son visibles en el prompt.

### 3.1. Identificar el servicio utilizado

Registra la información que realmente muestra la aplicación.

- Nombre de la plataforma.
- Modelo visible.
- Tipo de cuenta o espacio, cuando sea pertinente.

No incluyas identificadores personales innecesarios.

**Si el modelo no aparece, registra `no visible` en lugar de deducirlo.**

### 3.2. Preparar una conversación

El procedimiento debe reducir diferencias evitables entre pruebas.

- Utilizar una conversación nueva cuando corresponda.
- Comprobar instrucciones personalizadas conocidas.
- Revisar herramientas activas.

Una conversación nueva puede conservar otras influencias.

**El historial visible no representa necesariamente todo el contexto efectivo.**

### 3.3. Introducir la entrada

La preparación debe comprobar la plantilla antes de enviarla.

- Sustituir marcadores obligatorios.
- Incluir la política necesaria.
- Identificar la fuente de prueba.

Un marcador vacío puede invalidar la ejecución.

**Los errores de preparación deben registrarse separadamente de los errores de contenido.**

### 3.4. Conservar la respuesta

La respuesta original debe guardarse antes de corregirla.

- Mantener el contenido pertinente completo.
- Identificar caso y ejecución.
- Conservar advertencias o interrupciones visibles.

Una captura puede complementar el archivo de texto.

**No reemplaces la salida original por una versión editada.**

---

## 4. Editor de texto y documentos del proyecto

El editor conserva instrucciones, contratos y explicaciones fuera de la conversación.

### 4.1. Seleccionar un editor adecuado

El editor debe facilitar lectura y almacenamiento consistente.

- Archivos de texto o Markdown.
- Codificación compatible con acentos.
- Búsqueda y revisión del contenido.

No se necesita un editor especializado.

**La herramienta debe permitir recuperar exactamente la versión documentada.**

### 4.2. Separar materiales

Los documentos deben distinguir funciones dentro del expediente.

- Plantillas y prompts.
- Casos y referencias.
- Ejecuciones e informes.

La separación evita confundir expectativas con resultados.

**Una respuesta docente de referencia no debe guardarse como si fuera una ejecución.**

### 4.3. Utilizar nombres claros

Los nombres deben identificar contenido y versión.

- `P-01-v0.1.md`.
- `CAS-01-entrada.txt`.
- `EJ-001-respuesta.txt`.

Evita nombres como `final-ultimo-definitivo`.

**La convención debe aplicarse consistentemente en enlaces y registros.**

### 4.4. Revisar cambios de formato

El editor puede alterar la presentación del contenido.

- Comillas sustituidas automáticamente.
- Saltos de línea modificados.
- Caracteres invisibles o espacios adicionales.

Estos cambios pueden afectar formatos estructurados.

**Comprueba el contenido efectivo, no solo su apariencia visual.**

---

## 5. Hoja de cálculo para registrar pruebas

La hoja de cálculo organiza observaciones y facilita comparar versiones.

### 5.1. Función de la matriz

La matriz debe relacionar una prueba con su resultado.

- Caso e identificador de ejecución.
- Versión del prompt.
- Resultado esperado y observado.

Las respuestas extensas pueden conservarse en archivos relacionados.

**La hoja no necesita contener todo el expediente dentro de sus celdas.**

### 5.2. Columnas recomendadas

Una estructura separada permite registrar condiciones sin perder legibilidad.

| **Campo** | **Contenido** | **Condición** |
|---|---|---|
| Caso | Identificador de entrada | Obligatorio |
| Ejecución | Observación concreta | Obligatorio |
| Versión | Prompt utilizado | Obligatorio |
| Estado | Resultado de revisión | Obligatorio |
| Evidencia | Ruta del material | Debe ser consultable |

**Añade modelo, fecha y criterios en columnas o registros relacionados.**

### 5.3. Estados de evaluación

Utiliza un catálogo que distinga resultado y pendiente.

- `cumple` y `no_cumple`.
- `no_evaluado` y `pendiente_de_aclaracion`.
- `no_aplica`, con justificación.

Los colores pueden complementar las etiquetas.

**Una celda vacía no debe interpretarse automáticamente como favorable.**

### 5.4. Riesgos de transformación automática

La hoja puede modificar datos sin que resulte evidente.

- Convertir identificadores en números.
- Interpretar fechas según configuración regional.
- Eliminar ceros iniciales.

Importa como texto los campos que deban conservarse literalmente.

**Comprueba que el registro mantiene los valores originales.**

---

## 6. Registro del modelo y sus funciones

La documentación debe describir las capacidades disponibles durante la ejecución.

### 6.1. Inventario de capacidades

Registra únicamente funciones observadas o confirmadas.

- Entrada de texto.
- Archivos o imágenes.
- Herramientas conectadas.

La disponibilidad puede depender de cuenta, configuración y modalidad.

**No atribuyas funciones porque aparezcan en otra versión del producto.**

### 6.2. Límites visibles

Los límites deben documentarse cuando puedan afectar la tarea.

- Tamaño de entrada permitido.
- Tipos de archivo admitidos.
- Límites de salida conocidos.

La aplicación puede procesar solo parte de un archivo.

**Aceptar una carga no demuestra utilización íntegra del contenido.**

### 6.3. Funciones activas y utilizadas

Disponibilidad y utilización son condiciones diferentes.

- Una función puede estar disponible y desactivada.
- Puede estar activa y no utilizarse.
- Puede utilizarse con alcance limitado.

La ejecución debe indicar lo relevante.

**No declares navegación o ejecución de código si no ocurrieron.**

### 6.4. Ficha del entorno

Este bloque puede incorporarse al registro de cada prueba.

```text
Fecha:
Plataforma:
Modelo visible:
Interfaz:
Funciones disponibles:
Funciones activas:
Funciones utilizadas:
Configuración conocida:
Condiciones desconocidas:
```

**La ficha debe describir el entorno real, no una configuración ideal.**

---

## 7. Archivos, imágenes y fuentes externas

Las capacidades de entrada requieren comprobar qué contenido puede interpretarse.

### 7.1. Carga de documentos

La carga debe tener una finalidad concreta.

- Documento necesario para la tarea.
- Identificador de fuente.
- Formato compatible.

Los archivos extensos pueden requerir comprobaciones adicionales.

**No añadas documentos únicamente porque la interfaz permita subirlos.**

### 7.2. Imágenes y capturas

Las imágenes pueden aportar contenido visual o textual.

- Diagramas.
- Capturas de resultados.
- Documentos escaneados sintéticos.

La resolución y la disposición afectan a la lectura.

**Que el modelo acepte imágenes no demuestra precisión en todos sus detalles.**

### 7.3. OCR y extracción

El reconocimiento de texto puede introducir errores.

- Caracteres confundidos.
- Columnas mezcladas.
- Fragmentos omitidos.

Compara elementos críticos con la fuente visible.

**La extracción automática necesita revisión cuando afecta cifras, fechas o identificadores.**

### 7.4. Navegación y consulta externa

La consulta externa debe responder a una necesidad autorizada.

- Fuente pertinente.
- Fecha de consulta.
- Referencia conservada.

Una página recuperada puede contener información incorrecta o instrucciones de desviación.

**La pertinencia de una fuente no le concede autoridad sobre el objetivo.**

---

## 8. Configuración y comparabilidad

Las comparaciones necesitan condiciones conocidas y un procedimiento consistente.

### 8.1. Parámetros visibles

Algunos entornos permiten ajustar generación.

- Temperatura.
- Top-p.
- Límites de salida.

Otros servicios no muestran estas opciones.

**No inventes valores predeterminados para completar la documentación.**

### 8.2. Variación entre respuestas

Una entrada idéntica puede producir salidas diferentes.

- Puede existir muestreo.
- Puede cambiar el servicio.
- Puede influir contexto adicional.

La variación debe registrarse cuando afecta la conclusión.

**Una configuración conservadora no garantiza verdad ni determinismo completo.**

### 8.3. Procedimiento común

La comparación debe mantener condiciones pertinentes.

- Mismo contenido de entrada.
- Referencias compatibles.
- Método de revisión consistente.

Las diferencias inevitables deben declararse.

**Comparabilidad no significa control perfecto de todos los factores.**

### 8.4. Reintentos transparentes

Cada nueva generación constituye otra observación.

- Define la política previamente.
- Conserva intentos pertinentes.
- Distingue fallo técnico y repetición deliberada.

No selecciones silenciosamente la mejor salida.

**La selección de resultados puede exagerar el efecto de una versión.**

---

## 9. API como ampliación opcional

La API permite integrar generación mediante solicitudes programáticas.

### 9.1. Qué aporta una API

Una API facilita interacción estructurada entre una aplicación y un servicio.

- Envío de entradas.
- Recepción de respuestas.
- Acceso a metadatos disponibles.

Su uso requiere comprender el contrato del proveedor.

**Acceso programático no significa comportamiento idéntico al de la interfaz conversacional.**

### 9.2. Configuración autorizada

El proyecto necesita condiciones de acceso adecuadas.

- Cuenta permitida.
- Modelo habilitado.
- Límites y presupuesto conocidos.

No se necesitan credenciales compartidas para el recorrido básico.

**La configuración debe corresponder a las políticas del entorno.**

### 9.3. Contrato del proveedor

Las interfaces pueden utilizar estructuras diferentes.

- Nombres de campos.
- Tipos de mensajes.
- Gestión de herramientas.

Los ejemplos genéricos deben adaptarse a documentación vigente.

**No copies una solicitud de otro servicio suponiendo compatibilidad.**

### 9.4. Metadatos de respuesta

Conserva información disponible que ayude a interpretar la ejecución.

- Identificador de solicitud.
- Modelo declarado por el servicio.
- Uso reportado y estado.

Algunos datos pueden no estar presentes.

**Registra lo observado sin reconstruir metadatos inexistentes.**

---

## 10. Credenciales, costes y errores de API

La automatización requiere límites operativos antes de ejecutar lotes.

### 10.1. Protección de credenciales

Las credenciales no deben incorporarse a materiales compartidos.

- No pegarlas en prompts.
- No guardarlas en repositorios.
- No mostrarlas en capturas.

Utiliza mecanismos autorizados de configuración.

**Una variable de entorno evita algunas exposiciones, pero no garantiza protección absoluta.**

### 10.2. Límites de consumo

El equipo debe definir un alcance de ejecución.

- Número previsto de solicitudes.
- Límite de salida.
- Presupuesto permitido.

Los precios y cuotas dependen del servicio.

**No atribuyas costes actuales sin comprobar las condiciones aplicables.**

### 10.3. Manejo de errores

Los errores técnicos necesitan tratamiento separado.

- Autenticación.
- Cuota o límite de frecuencia.
- Interrupción o respuesta incompleta.

No todos los errores deben repetirse automáticamente.

**Una entrada rechazada no equivale a una respuesta semánticamente incorrecta.**

### 10.4. Reintentos de solicitudes

La repetición puede añadir costes o efectos.

- Limita el número de intentos.
- Registra el motivo.
- Comprueba si existen acciones externas.

Los mecanismos de idempotencia dependen del servicio.

**No repitas operaciones con consecuencias sin revisar cómo evita duplicados la aplicación.**

---

## 11. Python y entorno virtual

Python puede apoyar validación y registro sin ser necesario para completar el curso.

### 11.1. Función de Python

Un script puede reducir tareas repetitivas y comprobar formatos.

- Leer casos de archivos.
- Validar salidas.
- Generar registros.

La interpretación semántica sigue necesitando criterios.

**Automatizar una comprobación incorrecta multiplica el error con rapidez.**

### 11.2. Entorno virtual

Un entorno virtual separa dependencias de un proyecto.

- Facilita una instalación controlada.
- Reduce conflictos entre bibliotecas.
- Permite documentar paquetes utilizados.

No es una barrera de seguridad para ejecutar código no confiable.

**Aislamiento de dependencias no equivale a aislamiento de ejecución.**

### 11.3. Creación y activación

Estos comandos son ilustrativos para un entorno local autorizado.

```bash
python -m venv .venv

# macOS o Linux
source .venv/bin/activate

# Windows PowerShell
.venv\Scripts\Activate.ps1
```

**La activación depende de la consola y de las políticas del sistema.**

### 11.4. Dependencias documentadas

Registra las bibliotecas realmente utilizadas.

- Nombre y versión.
- Finalidad.
- Procedencia autorizada.

Un archivo de dependencias puede facilitar reconstrucción.

**No instales paquetes desconocidos únicamente porque aparezcan en una respuesta generada.**

---

## 12. Validación estructural con Python

El ejemplo siguiente revisa un contrato pequeño sin utilizar una API.

### 12.1. Contrato docente

La salida representa una clasificación sintética.

- `expediente_id`: texto no vacío.
- `categoria`: valor del catálogo.
- `evidencia`: lista de textos no vacíos.

No se admiten claves adicionales.

**La correspondencia de la evidencia con la fuente requiere una comprobación aparte.**

### 12.2. Función de validación

Este código utiliza únicamente la biblioteca estándar de Python.

```python
def validar_registro(registro):
    if not isinstance(registro, dict):
        return False
    claves = {"expediente_id", "categoria", "evidencia"}
    if set(registro) != claves:
        return False
    if not isinstance(registro["expediente_id"], str):
        return False
    if not registro["expediente_id"].strip():
        return False
    categorias = {"informacion", "cambio", "revision"}
    if registro["categoria"] not in categorias:
        return False
    evidencia = registro["evidencia"]
    if not isinstance(evidencia, list):
        return False
    return all(isinstance(x, str) and x.strip() for x in evidencia)
```

### 12.3. Alcance del ejemplo

La función comprueba condiciones estructurales concretas.

- Tipos básicos.
- Claves exactas.
- Categorías admitidas.

La lista vacía es válida porque el contrato no exige elementos.

**Si la política exige evidencia para ciertas categorías, añade esa regla explícitamente.**

### 12.4. Pruebas de la función

La validación también necesita casos de comprobación.

- Registro compatible.
- Campo ausente.
- Categoría no admitida.

La salida esperada debe definirse antes de ejecutar.

**Que el script se ejecute sin error no demuestra que todas sus reglas sean correctas.**

---

## 13. Formatos de registro y automatización

Los archivos estructurados pueden complementar la hoja de cálculo.

### 13.1. CSV

CSV representa registros mediante filas y campos.

- Puede importarse en hojas de cálculo.
- Necesita una convención de delimitador.
- Requiere comillas para ciertos contenidos.

Los saltos de línea y caracteres especiales deben conservarse correctamente.

**La exportación debe comprobarse, no asumirse equivalente al documento original.**

### 13.2. JSONL

JSONL conserva un objeto JSON por línea.

- Facilita añadir observaciones.
- Puede procesarse secuencialmente.
- Mantiene registros independientes.

Los saltos internos de texto deben representarse dentro del valor JSON.

**Un archivo JSONL no es una lista JSON convencional.**

### 13.3. Registro docente

Este objeto ilustra metadatos sin afirmar una ejecución real.

```json
{
  "ejecucion_id": "EJ-DEMO-001",
  "caso_id": "CAS-01",
  "prompt_version": "P-01-v0.1",
  "tipo": "ejemplo_docente",
  "estado": "no_evaluado",
  "respuesta_archivo": null
}
```

**El identificador y el estado distinguen la ilustración de una observación.**

### 13.4. Ejecución por lotes

La automatización debe definirse después del contrato.

- Leer entradas identificadas.
- Limitar solicitudes.
- Guardar respuestas y errores.

Cada caso mantiene su identidad aunque el lote falle parcialmente.

**Un lote iniciado no debe declararse completo si quedan solicitudes sin respuesta.**

---

## 14. Git y conservación de versiones

Git puede conservar cambios de archivos y facilitar colaboración técnica.

### 14.1. Qué conserva Git

Git registra instantáneas de contenido dentro de un repositorio.

- Prompts.
- Contratos.
- Documentación.

No es necesario incluir todas las respuestas originales en el mismo repositorio.

**El contenido sensible necesita una política de almacenamiento específica.**

### 14.2. Commit

Un commit identifica un estado del contenido versionado.

- Relaciona archivos y cambios.
- Puede incluir un mensaje explicativo.
- Permite recuperar estados anteriores.

El mensaje debe describir una modificación concreta.

**Un commit no demuestra que el contenido haya sido probado.**

### 14.3. Flujo inicial ilustrativo

Estos comandos crean un repositorio y guardan archivos seleccionados.

```bash
git init
git add README.md prompts/ pruebas/ referencias/
git status
git commit -m "Registra linea base y casos iniciales"
```

**Revisa los archivos preparados antes de confirmar el commit.**

### 14.4. Ramas y etiquetas

Las ramas y etiquetas pueden organizar candidatas y referencias.

- Una rama permite desarrollar cambios.
- Una etiqueta identifica un punto concreto.
- La recomendación necesita evidencia adicional.

No todas las etiquetas comerciales o técnicas significan aceptación.

**La convención del proyecto debe explicar qué representa cada estado.**

---

## 15. Seguridad del repositorio y colaboración

La conservación de versiones requiere revisar qué información se comparte.

### 15.1. Archivos excluidos

Un archivo `.gitignore` puede evitar incorporaciones accidentales futuras.

```gitignore
.venv/
__pycache__/
.env
.env.*
!.env.example
resultados-restringidos/
```

**La exclusión no elimina archivos que ya estén registrados en Git.**

### 15.2. Revisión antes de compartir

El repositorio debe inspeccionarse antes de publicarse o transferirse.

- Credenciales.
- Capturas.
- Datos personales.

Los archivos históricos también pueden contener información eliminada de la vista actual.

**Borrar un secreto del último archivo no garantiza su retirada del historial.**

### 15.3. Incidente con una credencial

Una exposición necesita respuesta según las políticas aplicables.

- Detener su utilización.
- Revocar o rotar la credencial.
- Revisar alcance de exposición.

La limpieza del repositorio es una medida adicional.

**Reescribir el historial no invalida una clave que siga activa.**

### 15.4. Colaboración controlada

Los equipos deben coordinar cambios y revisiones.

- Responsables de archivos.
- Convención de mensajes.
- Procedimiento para conflictos.

No combines versiones incompatibles sin comprobar contratos.

**La integración documental también puede introducir errores funcionales.**

---

## 16. Organización del entorno del proyecto

Una estructura consultable relaciona materiales sin imponer una herramienta concreta.

### 16.1. Directorio orientativo

El proyecto puede organizarse de la siguiente manera.

```text
proyecto/
├── README.md
├── prompts/
├── casos/
├── referencias/
├── ejecuciones/
├── informes/
├── scripts/
└── guia-uso.md
```

**Las carpetas opcionales solo deben existir si cumplen una función real.**

### 16.2. Documento de apertura

El archivo inicial debe explicar cómo interpretar el conjunto.

- Propósito y alcance.
- Entorno utilizado.
- Versiones relevantes.

Añade ubicación de resultados y pendientes.

**La apertura debe orientar la consulta, no duplicar todo el expediente.**

### 16.3. Identidad integrada

Una solución con varios componentes necesita identificar su combinación.

- Versiones de prompts.
- Políticas y esquemas.
- Batería e informe.

Los materiales entregados deben coincidir con los evaluados.

**Una modificación posterior requiere actualizar la identidad o declarar la diferencia.**

### 16.4. Recuperación y copias

El equipo debe prever pérdida de acceso o archivos.

- Copias autorizadas.
- Exportaciones comprobadas.
- Material de demostración conservado.

No se necesita copiar información restringida a ubicaciones personales.

**Una copia útil debe ser recuperable y respetar las condiciones de acceso.**

---

## 17. Sesiones prácticas con el entorno mínimo

Estas propuestas permiten practicar sin API, Python ni Git.

### 17.1. Sesión de treinta minutos

La actividad organiza una primera ejecución documentada.

- Cinco minutos: inventario del entorno.
- Diez minutos: prompt e identificación de entrada.
- Diez minutos: ejecución y conservación.

Los cinco minutos finales cubren comparación y pendientes.

**El resultado es una observación revisada, no una batería completa.**

### 17.2. Sesión de sesenta minutos

La actividad relaciona editor, interfaz y matriz.

- Diez minutos: contrato y variables.
- Quince minutos: tres casos y referencias.
- Veinte minutos: ejecuciones.

Los quince minutos finales cubren revisión y documentación.

**Selecciona casos normales, ausentes y ambiguos compatibles con el alcance.**

### 17.3. Entrada de práctica

El caso utiliza una solicitud sintética de formación.

```text
Participarán aproximadamente 12 personas.
La modalidad será presencial.
La duración será de dos horas.
Proponemos el 18 de noviembre de 2026.
La fecha todavía no está confirmada.
```

**La referencia conserva aproximación, 120 minutos y fecha propuesta.**

### 17.4. Entregable de la sesión

Los materiales deben permitir reconstruir el trabajo.

- Prompt completado.
- Entrada y referencia.
- Respuesta original y matriz.

Añade modelo visible, fecha y funciones utilizadas.

**El presupuesto ausente no debe convertirse en una cantidad inventada.**

---

## 18. Sesiones técnicas opcionales

Las actividades técnicas amplían registro y validación sin modificar los requisitos de calidad.

### 18.1. Sesión de sesenta minutos con Python

La actividad no requiere conexión a un servicio externo.

- Diez minutos: entorno y contrato.
- Quince minutos: función de validación.
- Veinte minutos: casos de prueba.

Los quince minutos finales cubren resultados y límites.

**La sesión comprueba estructura, no verdad de los hechos.**

### 18.2. Sesión de noventa minutos con Git

La actividad registra una línea base y una modificación.

- Quince minutos: estructura y exclusiones.
- Veinte minutos: commit inicial.
- Veinte minutos: cambio y comparación.

Los treinta y cinco minutos finales cubren revisión, recuperación y documentación.

**Utiliza exclusivamente archivos sintéticos y revisados.**

### 18.3. Sesión autorizada con API

La actividad presupone acceso configurado y documentación vigente del proveedor.

- Comprobar límites y presupuesto.
- Ejecutar una entrada identificada.
- Conservar respuesta y metadatos.

El docente asignará tiempo según el entorno real.

**No dediques la sesión a compartir credenciales o eludir restricciones de acceso.**

### 18.4. Entregable técnico

La ampliación debe conservar tanto código como evidencia.

- Script y dependencias.
- Contrato de entrada.
- Registros de ejecución.

Añade errores, exclusiones y condiciones desconocidas.

**La automatización no convierte una prueba parcial en una evaluación completa.**

---

## 19. Auditoría y resolución de incidencias

La revisión del entorno permite distinguir fallos de preparación, servicio y contenido.

### 19.1. Clasificación de incidencias

El diagnóstico debe partir de hechos observables.

- Variable sin completar.
- Solicitud rechazada.
- Respuesta incompatible.

Una misma ejecución puede presentar varios problemas.

**No atribuyas todos los fallos al modelo sin revisar el procedimiento.**

### 19.2. Simulación de interrupción

La práctica introduce un fallo controlado de disponibilidad.

- Declarar que no hubo respuesta completa.
- Conservar el estado conocido.
- Utilizar evidencia previa como respaldo.

La modalidad de respaldo debe identificarse.

**Una captura anterior no debe presentarse como ejecución del momento.**

### 19.3. Auditoría cruzada

Otro equipo intenta reconstruir una prueba.

- Localizar el prompt.
- Encontrar la entrada.
- Abrir la respuesta original.

Debe comprender el criterio y el entorno registrado.

**La ayuda oral necesaria señala una oportunidad de mejora documental.**

### 19.4. Recuperación documentada

La recuperación debe tener límites y una decisión clara.

- Corregir preparación.
- Repetir según política.
- Derivar o detener.

Registra si cambió alguna condición relevante.

**Recuperar funcionamiento no demuestra que el resultado cumpla el contrato.**

---

## 20. Checklist final y continuidad

El cierre debe relacionar herramientas, evidencias y condiciones de utilización.

### 20.1. Checklist del entorno mínimo

Comprueba que el equipo puede trabajar y conservar sus materiales.

- [ ] Interfaz autorizada.
- [ ] Editor y ubicación de archivos.
- [ ] Matriz con identificadores.

Añade procedimiento de copia y recuperación.

**La disponibilidad debe comprobarse antes de depender de ella en una presentación.**

### 20.2. Checklist del entorno técnico

Comprueba los elementos opcionales realmente utilizados.

- [ ] API y límites autorizados.
- [ ] Entorno y dependencias documentados.
- [ ] Repositorio revisado.

Añade validación, errores y protección de credenciales.

**No marques una capacidad como implementada si únicamente está propuesta.**

### 20.3. Checklist de evidencia

Comprueba el respaldo de las conclusiones.

- [ ] Modelo y funciones registrados.
- [ ] Entradas y respuestas originales.
- [ ] Referencias y criterios disponibles.

Las repeticiones y pendientes deben permanecer visibles.

**Una herramienta sofisticada no sustituye evidencia suficiente.**

### 20.4. Recursos y síntesis

Consulta los materiales relacionados para mantener coherencia.

- [Plantillas](../plantillas/index.md).
- [Glosario](glosario.md).
- [Proyecto final](../proyecto-final/index.md).

Relaciona la elección del entorno con la tarea y sus riesgos.

**Un buen entorno permite saber qué se ejecutó, cómo se revisó y bajo qué condiciones puede reutilizarse el resultado.**
