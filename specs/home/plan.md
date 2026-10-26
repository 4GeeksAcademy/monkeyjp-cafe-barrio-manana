# Plan: página de Inicio

Crear `index.html` reutilizando `docs/reference/base.html` y siguiendo `spec.md`, `CONTEXT.md` y `DESIGN.md`.

## Pasos

1. Copiar la estructura de `docs/reference/base.html` a `index.html`, ajustar el título y conservar la navbar, el footer y Tailwind CSS por CDN.
2. Añadir dentro de `main` un hero de bienvenida con un enlace a `menu.html`.
3. Presentar exactamente dos productos destacados, cada uno con nombre, descripción y precio.
4. Incluir datos estructurados Schema.org para Café Barrio y los dos productos, coherentes con el contenido visible.

La implementación se limita a `index.html`: no rehacer la estructura compartida ni añadir JavaScript propio o CSS adicional.