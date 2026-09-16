# Evidencias visuales

`docs/assets/` es el directorio raíz de las evidencias visuales del cuaderno de prácticas.

Organiza las imágenes en una subcarpeta por práctica:

```text
docs/assets/P01/
docs/assets/P02/
...
docs/assets/P26/
```

No es necesario crear ahora las 26 carpetas vacías: Git no versiona carpetas sin archivos. Cada carpeta `Pxx` se creará cuando se incorpore su primera imagen.

Utiliza nombres breves y descriptivos, preferentemente en minúsculas y con guiones bajos:

```text
P04/gram_01.jpg
P04/gram_02.jpg
P18/antibiograma_01.jpg
```

Desde un archivo `docs/practicas/Pxx_*.md`, referencia la imagen con una ruta relativa a `docs/assets/` e incluye siempre un texto alternativo y un pie de figura técnico:

```markdown
![Resultado de la tinción de Gram](../assets/P04/gram_01.jpg)

*Figura 1. Resultado de la tinción de Gram observada durante la práctica.*
```

Antes de publicar una imagen, comprueba que no contiene:

- rostros ni nombres del alumnado;
- etiquetas, códigos u otros datos personales;
- documentación sensible;
- datos identificables de pacientes; ni
- imágenes cuya realización o publicación esté prohibida por el centro.

Si la imagen procede de una demostración, simulación, material docente o fuente externa autorizada, indícalo en el pie de figura o en el apartado de evidencias de la práctica. No presentes como ejecución propia una imagen que no lo sea.
