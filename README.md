# Inferencia Causal 2026

Este es el repositorio del curso de Inferencia Causal 2026 para estudiantes de la Licenciatura y Maestría en Economía del CIDE.

Sitio: <https://rojasirvin.github.io/inferencia-causal/>

## Publicación

El sitio se despliega solo: cada push a `main` dispara el workflow `Quarto Publish`,
que rinde el proyecto y lo publica en la rama `gh-pages`.

CI **solo instala Quarto, no R**, y los datos crudos pesados no se versionan. El sitio
se construye a partir de `_freeze/`, así que:

> Si editas un chunk de R, corre `quarto render` localmente y commitea `_freeze/`
> junto con el `.qmd`. Si no, CI intentará ejecutar R, no lo encontrará y fallará.

Las páginas sin código R (`cronograma`, `lecturas`, `programa`, `reglas`,
`presentaciones`, `tareas/index`) se pueden editar y subir directamente.

## Respuestas de las tareas

Los archivos `tareas/tarea-N-respuestas.qmd` se versionan pero **no se publican**:
están excluidos del render en `_quarto.yml`. Para liberar una, quita la exclusión.
