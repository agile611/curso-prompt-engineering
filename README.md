# Curso de Prompt Engineering

Sitio web educativo construido con MkDocs y Material for MkDocs.

## Preparar el entorno

```bash
python -m venv .venv
```

Linux o macOS:

```bash
source .venv/bin/activate
```

Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

Instalar dependencias:

```bash
python -m pip install -r requirements.txt
```

## Previsualizar

```bash
mkdocs serve
```

Abre `http://127.0.0.1:8000`.

## Compilar y validar

```bash
mkdocs build --strict
```

La web generada queda en `site/`.

## Publicar en GitHub Pages

Con el repositorio y el remoto configurados:

```bash
mkdocs gh-deploy
```

## Organización

- `mkdocs.yml`: configuración y navegación.
- `docs/`: documentación fuente.
- `docs/assets/`: imágenes y datos de práctica.
- `site/`: web compilada; no se versiona.

## Estado inicial

La portada, la configuración, los índices de jornadas y la unidad
de anatomía del prompt tienen contenido inicial.

Las demás unidades incluyen una estructura editorial pendiente de completar.
Los datos de ejemplo son sintéticos.
