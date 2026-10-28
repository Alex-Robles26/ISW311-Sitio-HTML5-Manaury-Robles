# La Granja del Pollo · Sitio en HTML5

Tarea de ISW-311 Tecnologías de Internet I, Unidad I.
Sitio de tres páginas sobre La Granja del Pollo, un negocio de venta de huevos por cartón en Higüey, La Altagracia.

- **Sitio publicado:** https://alex-robles26.github.io/ISW311-Sitio-HTML5-Manaury-Robles/
- **Autor:** Manaury Robles · Matrícula 2023-3786

## Páginas

| Página | Qué tiene |
|---|---|
| `index.html` | Quiénes somos, qué ofrecemos, la noticia del galpón nuevo, preguntas frecuentes y un dato curioso |
| `servicios.html` | Productos, tabla de precios, los más vendidos, glosario, mapa de entregas y video |
| `contacto.html` | Medios de contacto, dirección y formulario de pedido |

## Mapa de etiquetas

| Familia | Página y sección | Etiquetas usadas | ¿Por qué esa etiqueta? |
|---|---|---|---|
| Cimientos | Las tres | `<!DOCTYPE html>`, `html lang="es"`, `head`, `body`, `meta charset`, `meta viewport`, `meta description`, `title` | El doctype y el `lang="es"` le dicen al navegador que es HTML5 y en español. El charset UTF-8 es para que las tildes y la ñ salgan bien, el viewport para que se vea bien en el celular, y cada página tiene su propio title y description porque cada una habla de algo distinto. |
| Encabezados y párrafos | Las tres, todas las secciones | `h1`, `h2`, `h3`, `p` | Un solo `h1` por página con el tema principal, cada sección arranca con su `h2` y en contacto puse un `h3` para "Dónde estamos" porque va dentro de la sección de medios. Así no hay saltos. Los textos van en `p` porque son párrafos. |
| Texto, citas y código | `index.html`, "Quiénes somos" y "Qué ofrecemos"; aside "Dato curioso" | `strong`, `em`, `mark`, `del`, `ins`, `abbr`, `small`, `sup`, `sub`, `q`, `blockquote`, `cite`, `kbd` | `strong` para lo importante (se vende por cartón de 30), `em` para recalcar que se recogen a mano. `del` e `ins` muestran el precio viejo y el nuevo de la oferta, que va resaltada con `mark`. `abbr` explica qué es RNC. `sup` para los m² y `sub` para el 3 del CaCO₃. `q` para el lema, que es corto y va dentro de la línea, y `blockquote` para el testimonio, que es más largo, con `cite` para el nombre de la repostería. `kbd` porque PEDIDO es lo que el cliente tiene que escribir. `small` en el pie para el copyright. |
| Listas | `servicios.html`, "Lo que vendemos", "Los más vendidos" y "Glosario" | `ul` anidada, `ol reversed`, `dl`, `dt`, `dd` | Los productos no tienen orden, por eso `ul`, y cada tipo de huevo tiene sus tamaños en una sublista dentro del `li`. Los más vendidos van en `ol reversed` porque es un top que cuenta del 3 al 1. El glosario es `dl` porque son palabras con su definición. |
| Enlaces | `contacto.html`, "Escríbenos o llámanos"; nav en las tres | `a` con `href` interno, `#pedido`, `mailto:`, `tel:`, `download`, `target="_blank"` con `rel="noopener"` | El nav enlaza las tres páginas. `#pedido` baja directo al formulario. `mailto:` abre el correo y `tel:` llama desde el celular. La lista de precios tiene `download` para que se baje en vez de abrirse. El enlace del Ministerio de Agricultura abre en otra pestaña con `rel="noopener"` para que esa página no tenga acceso a la nuestra. |
| Imágenes y multimedia | `servicios.html`, "Lo que vendemos", "Zona de entrega" y "Gallinas en el patio" | `figure`, `figcaption`, `img` con `alt`, `iframe` con `title`, `video` con `controls` y `source` | La foto de la canasta va en `figure` con su `figcaption` porque lleva su explicación y el crédito del autor. El `alt` dice lo que se ve para quien no puede ver la imagen. El mapa es un `iframe` de Google Maps y tiene `title` para que el lector de pantalla sepa qué es. El video lleva `controls` para que la persona lo ponga y lo pare, y `source` con su tipo. |
| Tablas | `servicios.html`, "Precios por cartón" | `table`, `caption`, `thead`, `tbody`, `tfoot`, `tr`, `th scope="col"`, `th scope="row"`, `td`, `rowspan`, `colspan` | Los precios son datos con filas y columnas, por eso tabla. El `caption` dice de qué es la tabla, `thead` tiene los títulos de columna con `scope="col"` y cada tipo de huevo es `th scope="row"`. Usé `rowspan` porque un mismo tipo de huevo tiene varios tamaños, y `colspan="4"` en el `tfoot` porque la nota aplica a toda la tabla. |
| Formularios | `contacto.html`, "Haz tu pedido" | `form`, `fieldset`, `legend`, `label for`, `input` (text, email, tel, number, date, time, file, radio, checkbox), `select` con `optgroup`, `textarea`, `button type="submit"` | Separé los datos de la persona y los del pedido en dos `fieldset`, y la forma de pago en otro porque los radios son un solo grupo. Cada campo tiene su `label` con `for` igual al `id`. El select agrupa los huevos blancos y marrones con `optgroup`. Para validar uso `required`, `minlength`, `maxlength`, `min`, `max` y `pattern` para el teléfono con guiones. |
| Semántica y div/span | Las tres; `index.html`, "Preguntas frecuentes"; `contacto.html` | `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`, `time`, `address`, `details`, `summary`, `div`, `span` | Cada parte tiene la etiqueta que dice lo que es: un solo `main` con el contenido, `section` para cada tema con su `h2`. La noticia del galpón es `article` porque se entiende sola, y el dato curioso es `aside` porque es algo aparte. `time` con `datetime` para la fecha de la noticia, `address` para la dirección de la granja y `details`/`summary` para que las preguntas se abran al tocarlas. Los `div` solo los usé en el formulario para agrupar cada label con su campo, que no tiene un significado especial, y un `span lang="en"` para marcar "delivery", que es inglés. |

## Créditos

- Foto de la canasta: George Chernilevsky, Wikimedia Commons, CC BY-SA 4.0.
- Video de la gallina: Nesnad, Wikimedia Commons, CC BY 4.0.
