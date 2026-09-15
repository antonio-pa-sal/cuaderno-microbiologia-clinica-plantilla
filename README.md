# Cuaderno de prácticas de Microbiología Clínica

Plantilla MkDocs + Material para publicar el cuaderno digital del alumnado en GitHub Pages.

## Estructura

- `docs/index.md`: portada con datos del alumno, centro, módulo y curso.
- `docs/practicas/`: P01–P26, con bloques fijos del profesor y campos rellenables.
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

Guarda las imágenes en `docs/assets/` y enlázalas desde cada práctica, por ejemplo:

```markdown
![Preparación del portaobjetos](../assets/P02-portaobjetos.jpg)
*Figura 1. Portaobjetos preparado antes de la observación.*
```

No incluyas datos identificables de pacientes ni fotografías fuera de las normas del centro.
