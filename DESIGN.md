---
name: Soluway — Landing
description: Minimalismo tipográfico puro para la agencia de automatización e IA para PyMEs (soluway.com.ar).
colors:
  verde: "#2F7D6B"
  acento: "#3FA58E"
  tinta: "#0F1F1B"
  crema: "#F5FAF8"
  blanco-superficie: "#FFFFFF"
  gris-suave: "#DCE7E2"
  gris-texto: "#57685F"
  terracota: "#E76F51"
  terracota-texto: "#C14E31"
typography:
  display:
    fontFamily: "Space Grotesk, sans-serif"
    fontSize: "clamp(2.625rem, 7vw, 5.25rem)"
    fontWeight: 700
    lineHeight: 1.02
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "Space Grotesk, sans-serif"
    fontSize: "clamp(1.75rem, 3.5vw, 2.5rem)"
    fontWeight: 700
    lineHeight: 1.12
    letterSpacing: "-0.02em"
  title:
    fontFamily: "Space Grotesk, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 500
    letterSpacing: "-0.01em"
  cifra:
    fontFamily: "Space Grotesk, sans-serif"
    fontSize: "1.5rem"
    fontWeight: 700
    letterSpacing: "-0.01em"
  body-grande:
    fontFamily: "Inter, sans-serif"
    fontSize: "1.1875rem"
    fontWeight: 400
  body:
    fontFamily: "Inter, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.6
  button:
    fontFamily: "Inter, sans-serif"
    fontSize: "1rem"
    fontWeight: 600
  body-secundario:
    fontFamily: "Inter, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 400
  ui-label:
    fontFamily: "Inter, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 500
  label:
    fontFamily: "IBM Plex Mono, monospace"
    fontSize: "0.75rem"
    fontWeight: 500
    letterSpacing: "0.14em"
  metadata:
    fontFamily: "IBM Plex Mono, monospace"
    fontSize: "0.8125rem"
    fontWeight: 400
rounded:
  focus: "2px"
  sm: "6px"
  md: "8px"
spacing:
  gutter: "24px"
  fila: "26px 0"
  card: "36px"
  seccion-gap: "48px"
  seccion: "96px 0"
  hero: "120px 0 100px"
components:
  button-primary:
    backgroundColor: "{colors.verde}"
    textColor: "{colors.crema}"
    rounded: "{rounded.sm}"
    padding: "15px 30px"
  button-primary-hover:
    backgroundColor: "{colors.acento}"
    textColor: "{colors.crema}"
  button-nav:
    backgroundColor: "{colors.verde}"
    textColor: "{colors.crema}"
    rounded: "{rounded.sm}"
    padding: "9px 20px"
  input:
    backgroundColor: "{colors.crema}"
    textColor: "{colors.tinta}"
    rounded: "{rounded.sm}"
    padding: "12px 14px"
  card:
    backgroundColor: "{colors.blanco-superficie}"
    rounded: "{rounded.md}"
    padding: "{spacing.card}"
---

# Design System: Soluway — Landing

## Overview

**Creative North Star: "Minimalismo tipográfico puro"**

Es la traducción web del Manual de Marca Soluway v1.0: sin metáforas ni mundos conceptuales, la marca se demuestra en ejecución precisa. La tipografía grande hace todo el trabajo — Space Grotesk enorme y apretada para los titulares, Inter para el cuerpo, IBM Plex Mono para etiquetas y metadata — sobre un fondo crema casi blanco estructurado exclusivamente con reglas hairline. El aire es el lujo: paddings de sección de 96px, hero de 120px, y una sola tinta de acento (el verde Soluway) que aparece con moderación quirúrgica.

La densidad es baja y editorial: cada sección es una grilla de dos columnas (etiqueta mono a la izquierda, contenido a la derecha) que se lee como el índice de un documento. No hay cards con iconos, ni contadores animados, ni ilustraciones de hero, ni sombras decorativas — esas son refusas confirmadas del contrato de dirección. La única concesión al color fuera del verde es la terracota, reservada por manual a señalar problemas (la columna "antes" del caso real y los mensajes de error).

El listón de artesanía es Linear / Stripe / Vercel: micro-transiciones de 150–180ms, un único momento de motion autoral (la entrada escalonada del hero), y accesibilidad como parte del acabado (contraste AA derivado, `prefers-reduced-motion`, `:focus-visible` consistente).

**Key Characteristics:**
- Tipografía como único ornamento; jerarquía de tamaño y familia, no de decoración.
- Un solo acento (verde #2F7D6B); terracota solo para señalar problemas.
- Reglas hairline #DCE7E2 como toda la estructura visual — bordes, no sombras.
- Grilla de sección con columna de kicker mono de 220px.
- Aire generoso: el espacio en blanco es el lujo de la página.

## Colors

Paleta cerrada del manual de marca, casi monocroma en la práctica: crema, tinta y verde, con la terracota como voz disidente reservada.

### Primary
- **Verde Soluway** (#2F7D6B): el único acento del sistema. Kickers, énfasis del H1 (`em`), fondo de botones, flechas y signos `+`/`−`, links, focus ring, `::selection`, chip y cifras de la columna "después".
- **Verde Acento** (#3FA58E): exclusivamente estado hover — de botones y de links. Nunca aparece en reposo.

### Tertiary
- **Terracota** (#E76F51): color de problema. Solo en el chip y las cifras de la columna "antes" del caso real.
- **Terracota Texto** (#C14E31): terracota oscurecida derivada para texto chico (mensaje de error del formulario); pasa AA sobre crema.

### Neutral
- **Tinta** (#0F1F1B): texto principal, titulares, links de navegación.
- **Crema** (#F5FAF8): fondo de página y de inputs dentro de la card blanca. También color de texto sobre verde.
- **Blanco Superficie** (#FFFFFF): fondo de las cards estructurales (antes/después y formulario) — un paso más claro que la crema, sin sombra.
- **Gris Suave** (#DCE7E2): todas las reglas hairline y bordes. Nunca texto.
- **Gris Texto** (#57685F): texto secundario, subtítulos, metadata, placeholders. Derivado del gris UI del manual (#6B7C76), oscurecido en el mismo matiz para pasar AA 4.5:1 sobre crema y blanco.

### Named Rules
**La Regla del Único Acento.** El verde es la única voz de color de la página; el hover es siempre y solo el paso a #3FA58E. Todo lo demás es crema, tinta y grises del mismo matiz verdoso.

**La Regla de la Terracota.** La terracota nombra problemas y nada más: el "antes" del caso y el error del formulario. Nunca es decoración, nunca es acento alternativo.

**La Regla del Contraste Derivado.** Cuando un color del manual no alcanza AA para texto, se oscurece manteniendo el matiz (gris UI → #57685F; terracota → #C14E31 en texto chico). El manual manda el matiz; la legibilidad manda la luminosidad.

## Typography

**Display Font:** Space Grotesk (con sans-serif de fallback) — pesos 500 y 700
**Body Font:** Inter (con sans-serif) — pesos 400, 500 y 600
**Label/Mono Font:** IBM Plex Mono (con monospace) — pesos 400 y 500

**Character:** Geométrica y contemporánea en display, neutra y legible en cuerpo, técnica en las etiquetas. El tracking negativo crece con el tamaño (−0.01em → −0.03em); la mono siempre va con tracking abierto y mayúsculas cuando etiqueta.

### Hierarchy
- **Display** (700, clamp(2.625rem, 7vw, 5.25rem), line-height 1.02, −0.03em): solo el H1 del hero. Máximo 15ch, `text-wrap: balance`, alineado a la izquierda. El énfasis se marca con `em` en verde, sin itálica.
- **Headline** (700, clamp(1.75rem, 3.5vw, 2.5rem), line-height 1.12, −0.02em): H2 de sección, con `text-wrap: balance`.
- **Title** (500, 1.25rem, −0.01em): H3 de las filas del índice y de los pasos. Space Grotesk en peso medio, nunca bold.
- **Body** (400, 1.0625rem, line-height 1.6): cuerpo base en tinta. El subtítulo del hero sube a 1.1875rem en gris texto, máx. 58ch.
- **Body secundario** (400, 0.9375rem): descripciones de filas, datos, intros y notas — siempre en gris texto, máx. 60–62ch.
- **Label** (mono 500, 0.75rem, 0.14em, MAYÚSCULAS): kickers de sección, títulos de columna del caso, base del footer.
- **Metadata** (mono 400, 0.8125rem): nota del hero, meta del caso, email de contacto, numeración de pasos (0.875rem).

### Named Rules
**La Regla del Kicker.** Toda sección abre con su etiqueta mono en verde, mayúsculas y tracking 0.14em; fuera del hero lleva la flecha del manual (`→ Nombre`). Es el primer nivel de la jerarquía de marca, no un adorno.

**La Regla de la Mono Funcional.** IBM Plex Mono aparece solo donde hay dato, etiqueta o metadata (kickers, cifras de contexto, numeración `01/02/03`, legales del footer). Nunca en cuerpo de lectura.

## Layout

Contenedor único de 1120px (`--ancho`) centrado con gutter de 24px. El modelo espacial es una sucesión de secciones separadas por hairlines (`section { border-top: 1px solid #DCE7E2 }`) con padding vertical de 96px (72px bajo 860px); el hero es la excepción, sin borde superior y con 120px arriba / 100px abajo.

Dentro de cada sección rige la **grilla de sección**: `220px 1fr` con gap de 48px — kicker mono en la columna angosta (con 10px de padding-top para alinear a la baseline del H2), contenido en la ancha. Bajo 860px colapsa a una columna con gap de 28px, kicker arriba.

El contenido interno repite grillas de dos columnas más chicas: filas del índice `260px 1fr` (gap 24px), pasos `64px 1fr` (número mono a la izquierda), campos dobles del formulario `1fr 1fr`. Los anchos de lectura se limitan por `ch` (58–70ch según rol), nunca por columnas adicionales.

Breakpoints usados: 860px (grilla de sección), 780px (antes/después apila), 720px (filas del índice y nav), 600px (formulario). La nav es sticky de 64px con fondo crema al 88% y `backdrop-filter: blur(8px)`; en mobile solo sobrevive el logo y el botón "Hablemos".

## Elevation & Depth

Sistema plano por doctrina: la profundidad se expresa con hairlines y con el paso tonal crema → blanco, no con sombras. Las cards estructurales (antes/después, formulario) son blanco #fff con borde #DCE7E2 sobre el fondo crema — ese salto de un tono es toda la elevación. La única sombra del sistema es funcional, no de profundidad: el anillo de foco de los inputs (`box-shadow: 0 0 0 3px color-mix(in srgb, var(--verde) 15%, transparent)`).

### Named Rules
**La Regla Sin Sombras.** Ninguna superficie proyecta sombra en reposo ni en hover. Si algo necesita destacarse, se destaca con borde, con blanco sobre crema, o con tipografía.

## Shapes

Lenguaje de esquinas apenas redondeadas: 6px para elementos interactivos (botones, inputs, logo del footer), 8px para cards contenedoras, 2px para el radio del focus ring. Todos los bordes son de 1px en gris suave; no existen bordes de 2px+, ni bordes de color en reposo (el borde verde aparece solo en focus de inputs). Las esquinas de las cards recortan su contenido (`overflow: hidden` en antes/después para que el divisor interno llegue al borde). No hay círculos, pills ni formas decorativas; los únicos "chips" son cuadrados de 10×10px sin radio que titulan las columnas del caso.

## Components

### Buttons
- **Carácter:** sólidos, contenidos, sin sombra — el verde hace todo.
- **Shape:** esquinas suaves (6px).
- **Primary** (`.btn`): fondo verde, texto crema, Inter 600 de 1rem, padding 15px 30px.
- **Hover / Focus:** fondo pasa a #3FA58E y sube 1px (`translateY(-1px)`), transición de 180ms; focus con outline verde de 2px y offset 3px (patrón global).
- **Variante nav** (`.btn-nav`): mismo tratamiento en tamaño compacto, padding 9px 20px, sin lift.
- **Estado disabled:** opacidad .6 y `cursor: wait` durante el envío del formulario.
- **Link flecha** (`.link-arrow`): CTA secundario tipográfico — texto en tinta 600 con flecha verde pegada (`↓` hacia ancla); en hover todo el link pasa a verde.

### Cards / Containers
- **Corner Style:** 8px con `overflow: hidden` cuando hay divisores internos.
- **Background:** blanco #fff sobre el fondo crema.
- **Shadow Strategy:** ninguna (ver Elevation & Depth); el borde es la elevación.
- **Border:** 1px gris suave; divisor interno vertical del mismo color en antes/después.
- **Internal Padding:** 36px (24px el formulario bajo 600px).

### Inputs / Fields
- **Style:** fondo crema (un tono más oscuro que la card blanca que los contiene), borde 1px gris suave, 6px de radio, padding 12px 14px, Inter 0.9375rem, placeholder en gris texto.
- **Focus:** borde verde + anillo `0 0 0 3px` de verde al 15% vía `color-mix`; transición 150ms.
- **Labels:** Inter 500 de 0.875rem sobre el campo; lo opcional se marca en texto, no con asterisco.
- **Mensajes:** `.form-msg` de 0.9375rem — éxito en verde, error en #C14E31; el error siempre ofrece el email como vía alternativa.

### Navigation
- Sticky, 64px de alto, crema al 88% con blur de 8px y hairline inferior. Logo PNG de 30px a la izquierda; links Inter 500 de 0.9375rem en tinta con hover verde; el CTA "Hablemos" como `.btn-nav`. En mobile (<720px) desaparecen los links de texto, quedan logo y CTA — sin menú hamburguesa.

### Índice tipográfico (componente firma)
La sección Posibilidades es una lista sin viñetas donde cada `li.fila` es una grilla `260px 1fr` (título Space Grotesk 500 de 1.25rem / descripción 0.9375rem gris) entre hairlines. En hover, el título pasa a verde y una flecha `→` verde aparece deslizándose 4px (180ms). Es el patrón para cualquier enumeración de servicios o capacidades: tipografía y línea, nunca cards con iconos.

### Antes / Después (componente firma)
Card blanca de dos columnas divididas por hairline. Cada columna abre con un título mono en mayúsculas precedido por un chip cuadrado de 10px (terracota = antes, verde = después) y lista `.dato`s separados por hairlines: cifra o frase corta en Space Grotesk 700 de 1.5rem con `tabular-nums` (coloreada según columna) sobre descripción de 0.9375rem en gris. Bajo 780px apila con el "antes" arriba. Es el formato canónico de prueba: evidencia real tipográfica, sin gráficos ni testimonios.

### Grilla de herramientas
Variante a dos columnas del índice tipográfico para enumeraciones no accionables (herramientas construidas): entradas con hairline superior, título Space Grotesk 500 de 1.25rem y descripción 0.9375rem gris (máx. 48ch), `column-gap` de 48px, apila bajo 720px. Sin hover ni flecha porque no son links.

### Pasos numerados
Lista ordenada con contador CSS: número mono verde con cero inicial (`01`, `02`, `03`) en columna de 64px, título Space Grotesk 500 de 1.25rem y párrafo gris al lado, hairline superior por ítem.

### Legales del footer
Acordeones `<details>` nativos entre hairlines: summary en tinta 500 de 0.875rem con `+`/`−` mono verde a la derecha; contenido en gris texto, máx. 70ch. El footer cierra con la base mono de 0.75rem en mayúsculas.

### Motion
Un solo momento autoral: la entrada del hero. Los hijos directos arrancan en `opacity: .45` y `translateY(18px)` y suben con `cubic-bezier(0.16, 1, 0.3, 1)` en 800ms, escalonados de a 80ms — el arranque en .45 garantiza que una animación pausada nunca deje el hero en blanco. Todo el bloque vive dentro de `@media (prefers-reduced-motion: no-preference)`. El resto del motion son micro-transiciones de 150–180ms `ease` sobre color, fondo y transform. `scroll-behavior: smooth` para las anclas.

**La Regla del Único Momento.** Hay una sola animación de entrada en toda la página (el hero). Ninguna sección nueva agrega reveals on-scroll, parallax ni contadores.

## Do's and Don'ts

### Do:
- **Do** abrir cada sección con su kicker mono (`→ Nombre`, 0.75rem, 0.14em, mayúsculas, verde) en la columna de 220px de la grilla de sección.
- **Do** estructurar con hairlines #DCE7E2 de 1px: entre secciones, entre filas, entre datos, entre legales.
- **Do** usar la crema #F5FAF8 como fondo global y el blanco #fff solo como superficie de card con borde.
- **Do** limitar anchos de lectura con `ch` (58–62ch en cuerpo, 70ch en legales) y balancear titulares con `text-wrap: balance`.
- **Do** derivar tonos más oscuros del mismo matiz cuando un color de marca no pase AA en texto (#57685F, #C14E31).
- **Do** envolver toda animación en `@media (prefers-reduced-motion: no-preference)` y mantener el `:focus-visible` verde global.

### Don't:
- **Don't** usar cards con iconos, glifos decorativos ni ilustraciones — la enumeración canónica es el índice tipográfico.
- **Don't** agregar sombras a superficies ni en hover; la elevación es borde + paso tonal.
- **Don't** usar la terracota fuera de señalar problemas (columna "antes", mensajes de error).
- **Don't** inventar métricas, contadores animados ni testimonios; la única prueba publicable es el caso real antes/después.
- **Don't** introducir un segundo acento de color ni usar #3FA58E en reposo — es exclusivamente hover.
- **Don't** sumar animaciones de entrada más allá del hero, ni reveals on-scroll.
