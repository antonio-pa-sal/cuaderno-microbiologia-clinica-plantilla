# Cuaderno de prácticas de Microbiología Clínica

Plantilla MkDocs + Material para publicar el cuaderno digital del alumnado en GitHub Pages.

## Estructura

- `docs/index.md`: portada con datos del alumno, centro, módulo y curso.
- `docs/practicas/`: P01–P26, con contenidos de referencia, procedimientos y campos rellenables por el alumnado.
- `docs/assets/`: evidencias visuales del alumnado, organizadas por práctica (P01, P02, etc.).
- `mkdocs.yml`: tema, navegación, buscador y orden de las páginas.
- `docs/stylesheets/extra.css`: diseño científico, limpio y adaptable.
- `.github/workflows/deploy.yml`: publicación automática en GitHub Pages tras cada cambio en `main`.

## Puesta en marcha

1. Sube este contenido a un repositorio de plantilla.
2. En **Settings → Pages**, selecciona **GitHub Actions** como origen.
3. Ejecuta el flujo o haz un primer commit en `main`.
4. Para cada alumno, crea una copia del repositorio o una asignación individual de GitHub Classroom.

El alumnado edita los `.md` desde **Edit** y **Preview** en GitHub, desde `github.dev` o mediante Codespaces. La página publicada se regenera automáticamente con cada cambio aceptado en `main`.

## Imágenes

Las evidencias visuales se almacenan en `docs/assets/` y se organizan en una subcarpeta por práctica. Las subcarpetas se crean cuando sea necesario incorporar la primera imagen; no es necesario crear carpetas vacías por adelantado.

```text
docs/assets/
├── P01/
├── P02/
└── P03/
```

Usa nombres breves y descriptivos, por ejemplo:

```text
docs/assets/P04/gram_01.jpg
```

Desde un archivo situado en `docs/practicas/`, enlaza la imagen con una ruta relativa e incluye un pie de figura:

```markdown
![Resultado de la tinción de Gram](../assets/P04/gram_01.jpg)
*Figura 1. Resultado de la tinción de Gram observada durante la práctica.*
```

Consulta [docs/assets/README.md](docs/assets/README.md) para las normas completas de organización, referencias y privacidad. No publiques rostros, nombres, etiquetas con datos personales, documentación sensible, datos identificables de pacientes ni imágenes cuya realización o publicación esté prohibida por el centro.
