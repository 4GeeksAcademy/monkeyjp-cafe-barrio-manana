
# Contexto del proyecto — Café Barrio

## Negocio
Café Barrio es una cafetería local ficticia que ofrece café,
té y comida ligera.

Necesita una web informativa con un menú y un formulario
para solicitar pedidos anticipados.

## Objetivo
Construir un prototipo responsive de tres páginas,
trabajando en equipo con Git y desarrollo guiado por
especificaciones (SDD).

## Páginas

### Inicio — index.html
- Navbar con enlaces a Menú y Pedido.
- Hero con bienvenida y enlace al menú.
- Dos productos destacados con nombre, descripción y precio.
- Footer con dirección, horario y enlace a Pedido.

### Menú — menu.html
- Navbar y footer compartidos visualmente.
- Categorías: Café, Té y Comida.
- Filtros solo visuales, sin funcionamiento.
- Mínimo 8 productos con imagen placeholder, nombre y precio.

### Pedido — order.html
- Navbar y footer compartidos visualmente.
- Nombre del cliente.
- Hora de recogida: select con 3 o 4 opciones.
- Al menos 3 productos seleccionables mediante checkboxes.
- Instrucciones especiales.
- Botón submit. 

## Límites
- Solo HTML5 y Tailwind CSS v4 por CDN.
- Sin React, JavaScript propio, backend de pedidos ni base de datos.
- Formulario demostrativo: no procesa ni guarda pedidos.
- Diseño responsive mobile-first.
- HTML semántico y accesible.
- Datos estructurados Schema.org:
  CafeOrCoffeeShop y MenuItem en páginas pertinentes.

## Trabajo colaborativo
- Cada página se desarrolla en su propia rama.
- Cada funcionalidad tiene spec.md, plan.md y tasks.md.
- Todas las páginas siguen el mismo DESIGN.md.
- La integración se realiza mediante pull requests.
