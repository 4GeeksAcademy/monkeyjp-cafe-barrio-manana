# Especificación: página de Menú

## Objetivo

Crear la página de menú (`menu.html`) para Café Barrio, mostrando los productos disponibles organizados por categorías (Café, Té y Comida), con filtros visuales y datos estructurados Schema.org.

## Alcance

La página incluye la navbar y el footer compartidos del sitio, una presentación del menú, una barra de filtros visuales (sin funcionalidad JavaScript) y una cuadrícula de al menos 8 productos con imagen, nombre y precio. No incluye funcionalidad de pedido ni carrito.

## Requisitos

### Estructura del documento

- Debe ser un documento HTML5 válido en español.
- Debe cargar Tailwind CSS v4 por CDN mediante `<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>`.
- No debe depender de React, JavaScript propio, backend, base de datos ni hojas de estilo adicionales.
- Debe usar la misma navbar y footer que `docs/reference/base.html`, sin modificaciones en la estructura compartida.

### Navbar y footer

- La navbar debe incluir el logo "Café Barrio" enlazado a `index.html`, y enlaces a `index.html` (Inicio), `menu.html` (Menú) y `order.html` (Pedido).
- El footer debe incluir dirección, horario y un enlace a `order.html`.
- Ambos deben ser visualmente idénticos a los de `docs/reference/base.html`.

### Contenido del menú

- Un título principal (`h1`) con el texto "Nuestro Menú".
- Una breve presentación descriptiva del menú.
- Una barra de filtros visuales con tres botones o enlaces: Café, Té y Comida.
- Los filtros deben ser solo visuales (sin JavaScript), sin funcionalidad de filtrado real.

### Cuadrícula de productos

- Mínimo 8 productos variados distribuidos entre Café, Té y Comida.
- Cada producto debe incluir:
  - Una imagen placeholder relacionada con el producto (usando `https://placehold.co/` u otro servicio de placeholders).
  - Nombre del producto.
  - Precio en euros (€).
- La cuadrícula debe ser responsive:
  - 1 columna en móvil.
  - 2 columnas en tablet (`sm:`).
  - 4 columnas en escritorio (`lg:`).
- Las imágenes deben ser de tamaño uniforme y las tarjetas coherentes con el diseño existente en `DESIGN.md`.
- Usar el mismo estilo de tarjeta (fondo blanco, `rounded-xl`, borde suave) definido en `DESIGN.md`.

### Datos estructurados Schema.org

- La página debe incluir datos estructurados JSON-LD para `CafeOrCoffeeShop`.
- Cada producto debe incluir microdatos HTML de Schema.org usando `itemscope`, `itemtype`, `itemprop`:
  - `MenuItem` para cada elemento del menú.
  - Propiedades: `name`, `image`, `price`, `priceCurrency` (EUR).
- El precio debe marcarse con las propiedades `price` y `priceCurrency` dentro del marcado `MenuItem`.

### Accesibilidad

- Debe incluir un enlace de salto al contenido principal (`Saltar al contenido principal`).
- La navegación debe tener `aria-label="Navegación principal"`.
- Las imágenes deben tener atributos `alt` descriptivos.
- Los elementos interactivos deben ser accesibles por teclado.

## Fuera de alcance

- Funcionalidad de filtrado real con JavaScript.
- Carrito de compras o sistema de pedido en la página de menú.
- Procesamiento de formularios.
- Página de pedido (`order.html`).

## Criterios de aceptación

- `menu.html` existe en la raíz del proyecto y es un documento HTML5 válido.
- La página tiene navbar y footer idénticos a los de `base.html`.
- Hay al menos 8 productos con imagen, nombre y precio.
- La cuadrícula es responsive (1 columna móvil, 2 tablet, 4 escritorio).
- Los productos tienen microdatos `MenuItem` con `name`, `image`, `price` y `priceCurrency`.
- Los filtros visuales (Café, Té, Comida) están presentes sin funcionalidad JavaScript.
- Las imágenes son de tamaño uniforme y las tarjetas siguen el diseño de `DESIGN.md`.
- No hay enlaces rotos entre páginas.
