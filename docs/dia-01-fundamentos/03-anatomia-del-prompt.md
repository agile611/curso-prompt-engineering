# Anatomía del prompt

Un prompt eficaz define la tarea y aporta la información necesaria
para que la respuesta pueda evaluarse.

## Ficha de la unidad

- **Duración:** 1,5 horas.
- **Modalidad:** explicación, demostración y práctica.
- **Resultado:** un prompt con requisitos verificables.

## Objetivos

- Distinguir instrucciones, contexto y datos de entrada.
- Especificar restricciones y formato de salida.
- Identificar ambigüedades antes de ejecutar un prompt.

## Conceptos clave

### Tarea

Describe qué debe hacer el modelo.

### Contexto

Explica para quién se realiza la tarea y con qué propósito.

### Datos de entrada

Incluye el material que el modelo debe utilizar.

### Restricciones y salida

Define límites, estructura y criterios de aceptación.

## Ejemplo

```text
TAREA
Resume el informe proporcionado.

CONTEXTO
El resumen está dirigido a una persona responsable de operaciones.

DATOS
[Inserta aquí el informe]

RESTRICCIONES
Utiliza únicamente información del informe.
Si falta algún dato, indica que no está disponible.

FORMATO
- Resumen ejecutivo de hasta 150 palabras.
- Tres hallazgos principales.
- Riesgos identificados.
- Datos pendientes de confirmar.
```

## Actividad práctica

1. Redacta una instrucción inicial para resumir un documento.
2. Ejecuta el prompt y conserva la respuesta.
3. Añade contexto, restricciones y formato.
4. Compara ambas respuestas.

## Criterios de comprobación

- [ ] La tarea está definida.
- [ ] La audiencia está identificada.
- [ ] Los datos están separados de las instrucciones.
- [ ] El formato de salida es explícito.
- [ ] Se indica cómo tratar la información ausente.

## Entregable

Guarda el prompt inicial, el prompt revisado y una explicación breve
de los cambios realizados.

## Recursos relacionados

- [Ficha de prompt](../plantillas/ficha-de-prompt.md)
- [Registro de versiones](../plantillas/registro-de-versiones.md)
