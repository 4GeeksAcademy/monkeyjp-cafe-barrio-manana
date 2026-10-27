# Plan: página de Menú

Crear `menu.html` siguiendo [la especificación](spec.md), `CONTEXT.md`, `DESIGN.md` y la plantilla `docs/reference/base.html`.

## Pasos

1. Revisar `docs/reference/base.html` y copiar su estructura compartida (navbar, footer, enlaces de salto, Tailwind CDN).
2. Añadir título `h1` "Nuestro Menú" y una breve presentación del menú dentro de `main`.
3. Añadir barra de filtros visuales con tres botones/enlaces: Café, Té y Comida (sin JavaScript).
4. Crear cuadrícula responsive de productos con al menos 8 elementos:
   - 4 productos de Café.
   - 2 productos de Té.
   - 2 productos de Comida.
5. Cada producto incluir imagen placeholder (`https://placehold.co/400x300?text=...`), nombre y precio en euros.
6. Añadir microdatos Schema.org `MenuItem` a cada producto con `name`, `image`, `price` y `priceCurrency`.
7. Añadir datos estructurados JSON-LD para `CafeOrCoffeeShop` en el `head`.
8. Verificar enlaces entre `index.html` y `menu.html`.

## Límites

- No añadir JavaScript funcional para filtros.
- No modificar `docs/reference/base.html`.
- No alterar la navbar ni el footer compartidos.
- No crear páginas que no sean `menu.html`.

## Verificación

- Confirmar que `menu.html` tiene navbar y footer idénticos a `base.html`.
- Comprobar que la cuadrícula es responsive (1, 2 y 4 columnas).
- Verificar que los microdatos y JSON-LD son válidos.
- Probar enlaces entre `index.html` e `index.html` y `menu.html`.
