# AGENTS.md — cuaderno de prácticas

Este repositorio contiene el producto web y las prácticas generadas. El proceso editorial reusable se mantiene en el repositorio separado [cuadernos-practicas-workflow](https://github.com/antonio-pa-sal/cuadernos-practicas-workflow).

Antes de crear o cambiar prácticas, consulta el `WORKFLOW.md` de ese repositorio y las fuentes canónicas vigentes del módulo. Cada procedimiento puede tener hasta **14 pasos numerados** y mantiene un máximo de **40 palabras por paso**. Mantén aquí únicamente el contenido del producto, su navegación y sus recursos. No copies fuentes internas ni archivos de gobierno completos al sitio publicado.

Para nuevas prácticas, sigue la plantilla simplificada de Fase 3 del `WORKFLOW.md`: **8.1 Verificación previa** con instrumental, equipos, reactivos/materiales y residuos previstos (urbanos o asimilables a los urbanos, punzocortantes, biológicos o infecciosos); **9.1 Registro de observaciones y cálculos** con cálculos, configuración de equipos y características del producto o resultado final, en tablas de dos columnas. No reintroduzcas 8.2, la antigua comprobación de calidad rellenable ni 9.2/9.3. Conserva los controles docentes y verifica numeración, referencias y renderizado.

En revisiones, limita la migración a las fichas autorizadas. P01/P02 de TAH y P01/P02/P03 de Microbiología Clínica son excepciones protegidas de la simplificación acordada; no las modifiques sin un nuevo encargo explícito ni uses sus tablas históricas como patrón para nuevas fichas.

Revisa `git status` y el diff antes de operar; no incluyas archivos ajenos al encargo. Commit, push y publicación requieren autorización expresa.

En el apartado de conclusión, pide una valoración razonada que conecte el objetivo con el resultado y/o el procedimiento. No solicites de nuevo cálculos, datos, registros o imágenes ya incluidos en la ficha.

## Rúbricas y ejemplos resueltos

En cada módulo, reserva `docs/modulos/<slug>/rubricas/<Pnn>/`, con una carpeta por cada práctica del programa vigente e identificada por su código estable (`P01`, `P02`, etc.). Estas carpetas se destinan a la futura rúbrica de evaluación y calificación de la práctica y a un ejemplo de práctica correctamente resuelto. La estructura de carpetas no autoriza a redactar ninguno de esos materiales: créalos únicamente ante una solicitud humana explícita y contrástalos con las fuentes canónicas del módulo, sus RA/CE y los criterios de evaluación aprobados. No añadas archivos de marcador dentro de las carpetas vacías.

Mantén `modulos/**/rubricas/**` excluido de la documentación generada por MkDocs para que los materiales docentes futuros no se publiquen automáticamente con el cuaderno del alumnado.
