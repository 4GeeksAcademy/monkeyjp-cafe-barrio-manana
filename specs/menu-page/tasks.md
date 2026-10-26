# Tareas: página de Menú

## Preparación

- [x] Revisar `docs/reference/base.html`, `CONTEXT.md` y `DESIGN.md`.
- [x] Crear `specs/menu-page/spec.md` con la especificación de la página de menú.
- [x] Crear `specs/menu-page/plan.md` con el plan de implementación.

## Estructura compartida

- [x] Copiar navbar, footer y enlace de salto desde `docs/reference/base.html`.
- [x] Mantener Tailwind CSS v4 por CDN, sin CSS adicional ni JavaScript.
- [x] Verificar que los enlaces de navbar apuntan a `index.html`, `menu.html` y `order.html`.

## Contenido del menú

- [x] Añadir título `h1` "Nuestro Menú".
- [x] Añadir párrafo de presentación del menú.
- [x] Añadir barra de filtros visuales con Café, Té y Comida.

## Cuadrícula de productos

- [x] Añadir 4 productos de Café (imagen, nombre, precio).
- [x] Añadir 2 productos de Té (imagen, nombre, precio).
- [x] Añadir 2 productos de Comida (imagen, nombre, precio).
- [x] Imágenes placeholder uniformes (400×300).
- [x] Tarjetas con fondo blanco, `rounded-xl` y borde suave.
- [x] Cuadrícula responsive: `grid-cols-1 sm:grid-cols-2 lg:grid-cols-4`.

## Datos estructurados

- [x] Añadir JSON-LD `CafeOrCoffeeShop` en el `<head>`.
- [x] Añadir microdatos `MenuItem` a cada producto con `name`, `image`, `price` y `priceCurrency`.

## Verificación

- [x] Comprobar que la navbar y el footer son idénticos a `base.html`.
- [x] Verificar el diseño responsive en móvil, tablet y escritorio.
- [x] Confirmar que los enlaces entre `index.html` y `menu.html` funcionan.
- [x] Validar que no hay JavaScript funcional ni tecnologías no permitidas.
- [x] Revisar que no hay enlaces rotos.
