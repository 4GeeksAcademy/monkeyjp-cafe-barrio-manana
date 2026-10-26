# Especificación: página de Inicio

## Objetivo

Definir los requisitos de `index.html`, la página de bienvenida de Café Barrio. La página debe presentar brevemente el café y dar acceso al menú.

## Alcance

La página de Inicio se construirá a partir de `docs/reference/base.html`. El contenido específico se añadirá dentro de `main`, conservando la estructura y la presentación compartidas de navegación y pie de página.

## Requisitos

### Estructura y navegación

- La página debe partir de `docs/reference/base.html` y mantener su navbar y footer compartidos.
- La navegación debe permitir acceder a Menú (`menu.html`) y Pedido (`order.html`), además de Inicio.
- El contenido específico de Inicio debe estar dentro de `main` y utilizar una jerarquía de encabezados semántica.

### Hero de bienvenida

- La página debe incluir un hero con un mensaje de bienvenida a Café Barrio.
- El hero debe incluir un enlace claro a `menu.html`.

### Productos destacados

- La página debe presentar exactamente dos productos destacados.
- Cada producto debe mostrar nombre, descripción y precio.
- Los productos deben estar identificados semánticamente como elementos de menú.

### Datos estructurados

- La página debe incluir datos estructurados Schema.org para la cafetería (`CafeOrCoffeeShop`).
- Debe incluir datos estructurados `MenuItem` para los dos productos destacados, coherentes con el contenido visible.

### Diseño y accesibilidad

- El diseño debe seguir `DESIGN.md`: estilo minimalista, cálido y acogedor; paleta, tipografías y espaciados establecidos; utilidades Tailwind.
- El contenido debe ser responsive con enfoque mobile-first y mantener legibilidad en móvil y escritorio.
- Los enlaces deben tener nombres claros, ser operables con teclado y mostrar un indicador de foco visible.
- La página debe usar HTML semántico y no añadir JavaScript propio ni CSS adicional.

## Fuera de alcance

- La lista completa de productos y filtros del menú.
- El formulario o el procesamiento de pedidos.
- Cambios al diseño de la navbar o el footer compartidos.
- Datos comerciales no definidos por el proyecto; no se deben inventar datos reales de dirección, horarios u otros datos del negocio.

## Criterios de aceptación

- `index.html` utiliza la plantilla `docs/reference/base.html` y conserva su navbar y footer compartidos.
- Se muestra un hero de bienvenida con un enlace a `menu.html`.
- Se muestran exactamente dos productos destacados y cada uno tiene nombre, descripción y precio.
- Los datos estructurados describen Café Barrio como `CafeOrCoffeeShop` y los dos destacados como `MenuItem`, coincidiendo con el contenido visible.
- La página sigue `DESIGN.md`, usa estructura semántica accesible y se adapta a móvil y escritorio sin CSS adicional ni JavaScript propio.