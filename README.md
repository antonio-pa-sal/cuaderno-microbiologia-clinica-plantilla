# Cuadernos de prácticas

Repositorio MkDocs Material para organizar cuadernos digitales por módulo profesional y publicarlos en GitHub Pages.

## Estructura por módulo

```text
docs/
├── index.md
└── modulos/
    └── microbiologia-clinica/
        ├── fuentes-canonicas/       # registro y procedencia de las fuentes
        ├── practicas-generadas/     # Markdown que alimenta el sitio
        ├── assets/                  # guía y evidencias visuales del módulo
        └── index.md                 # portada del cuaderno del módulo
```

Cada módulo utiliza un slug estable y mantiene separadas sus fuentes canónicas, fichas generadas y evidencias. El registro de las fuentes canónicas de Microbiología Clínica está en `docs/modulos/microbiologia-clinica/fuentes-canonicas/README.md`; los documentos fuente se mantienen en el proyecto que los produjo y no se duplican aquí.

El proceso reutilizable y las instrucciones de Codex se mantienen en el repositorio separado [cuadernos-practicas-workflow](https://github.com/antonio-pa-sal/cuadernos-practicas-workflow). Para incorporar otro módulo, sigue ambos documentos y crea su propia carpeta dentro de `docs/modulos/`.

## Puesta en marcha

1. Configura GitHub Pages con **GitHub Actions** como origen.
2. Revisa la navegación del módulo en `mkdocs.yml`.
3. Instala las versiones fijadas en `requirements.txt`.
4. Compila con `python -m mkdocs build --strict`.
5. Publica los cambios en `main` según la autorización del responsable del repositorio.

La acción de GitHub instala las mismas dependencias fijadas en `requirements.txt`, compila el sitio y publica el resultado. Un build correcto comprueba la construcción del sitio; no sustituye la validación curricular, docente ni de seguridad.

## Evidencias visuales y privacidad

Cada módulo almacena sus imágenes en `docs/modulos/<slug>/assets/<codigo-practica>/`. Las subcarpetas se crean cuando se incorpore la primera imagen; no es necesario crear carpetas vacías por adelantado.

Usa nombres breves y descriptivos, por ejemplo:

```text
docs/modulos/microbiologia-clinica/assets/P04/gram_01.jpg
```

Desde un Markdown situado en `practicas-generadas/`, enlaza la imagen con una ruta relativa y añade texto alternativo y pie de figura:

```markdown
![Resultado de la tinción de Gram](../assets/P04/gram_01.jpg)
*Figura 1. Resultado de la tinción de Gram observado durante la práctica.*
```

Consulta la guía del módulo en `docs/modulos/microbiologia-clinica/assets/README.md`. No publiques rostros, nombres, etiquetas identificativas, datos personales o clínicos, documentación sensible ni imágenes cuya realización o publicación no esté autorizada.
