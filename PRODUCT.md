# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

HTML/CSS/JS estático, una sola página (`index.html`), deploy en GitHub Pages con dominio propio `soluway.com.ar` (CNAME). Sin build step. La versión anterior usaba Tailwind por CDN y Font Awesome; nada obliga a mantenerlos.

## Users

Dueños y decisores de PyMEs argentinas (5+ empleados) que llegan desde LinkedIn, Instagram o referidos. Segmentos prioritarios: salud (clínicas), logística, retail, servicios profesionales (estudios contables y jurídicos). No son técnicos: evalúan si automatizar les ahorra tiempo y plata, desconfían del humo tecnológico y deciden por claridad y confianza, no por jerga.

## Product Purpose

Landing única de la agencia Soluway. Éxito = que un dueño de PyME entienda en una lectura qué le pueden automatizar, crea que es para negocios como el suyo, y mande el formulario de contacto.

## Positioning

"Tu socio tech": no son los más baratos, son los más claros. Construyen herramientas a medida (bots de WhatsApp con Claude API + FastAPI + Twilio, automatizaciones n8n/Make, OCR documental) y las explican sin tecnicismos. Anti-marca explícita: NO agencia genérica de "soluciones integrales", NO tech-bros, NO startup experimental.

## Operating Context

- El visitante típico llega desde contenido orgánico (LinkedIn/Instagram) o referido por otro cliente.
- Servicios reales: bots de WhatsApp (atención, turnos, recordatorios), automatizaciones entre sistemas (n8n self-hosted, Make.com legado), procesamiento documental (OCR de facturas/remitos), reportes automáticos, integraciones con Google Calendar/Sheets.
- Canal de contacto: formulario Formspree (`https://formspree.io/f/xbdzyqjd`) + email `soluway.group@gmail.com`. **Sin WhatsApp público por ahora** (decisión confirmada 2026-08).

## Capabilities and Constraints

- Sitio estático, sin backend propio: el formulario es Formspree, no cambiar el endpoint.
- Secciones legales (Términos, Privacidad, Cookies) deben conservarse — el texto actual es válido.
- Assets disponibles: `assets/logo.png` (logotipo), `assets/favicon_square.png` e `assets/fav_icon.png` (isologo). Solo PNG; versiones vectoriales pendientes.
- Idioma: español rioplatense, tuteo/voseo.

## Brand Commitments

Manual de Marca Soluway v1.0 (2026) es vinculante — resumen operativo en skill `soluway-brand`:

- Paleta cerrada: `#2F7D6B` primario, `#0F1F1B` casi negro, `#F5FAF8` crema, `#3FA58E` acento, `#DCE7E2` gris suave, `#6B7C76` gris UI, `#E76F51` terracota SOLO para señalar problemas/antes-después.
- Tipografías fijas: Space Grotesk (display), Inter (cuerpo), IBM Plex Mono (datos/tags/metadata). No sustituibles.
- Jerarquía de 6 niveles: etiqueta mono → kicker con flecha → título display → subtítulo → cuerpo → metadata.
- Voz: conversacional directo, argentino natural, cero emojis decorativos, lista negra de palabras ("innovador", "disruptivo", "soluciones integrales", "potenciar", "transformación digital", etc.).
- Frases firma (máx. una por pieza): "Tu socio tech" / "Con nosotros no gastás, invertís." / "Automatizá lo que te frena." / "Sin promesas raras. Sin vender humo."
- **Dirección visual elegida (2026-08, decisión de Tiziano tras 3 re-rolls)**: minimalismo tipográfico puro — sin metáforas ni mundos conceptuales; tipografía grande, grilla estricta, mucho aire, verde Soluway como único acento. Listón de artesanía: Linear / Stripe / Vercel. Preferencia estable para futuras superficies web de Soluway.

## Evidence on Hand

- **Un caso real publicable, anonimizado** (confirmado 2026-08): clínica de kinesiología en Buenos Aires, 4 personas. Antes: recepcionista dedicaba 4 hs/día a gestionar turnos por WhatsApp y teléfono, 30% de no-shows (~$180.000/mes en horas profesionales perdidas), doble booking frecuente. Solución: bot de WhatsApp que muestra turnos disponibles, confirma contra Google Calendar (3 profesionales) y manda recordatorio automático 24 hs antes. Publicar SIN nombre de la clínica.
- **No hay métricas agregadas publicables** (confirmado 2026-08): nada de contadores de "clientes activos" ni "personas alcanzadas". No fabricar.
- **No hay testimonios reales publicables**: las reseñas de la versión anterior eran placeholder — no reutilizarlas ni inventar otras.

## Product Principles

1. Claridad sobre impresión: si un dueño de PyME no lo entiende en una lectura, está mal.
2. Honestidad probatoria: solo evidencia real; ante la falta de prueba, mostrar concreción (qué hacemos y cómo), nunca inventar números.
3. Hablar de procesos del cliente (turnos, facturas, stock, emails), no de tecnología propia.
4. Cada sección empuja a una sola acción: mandar el formulario.
5. La marca se demuestra en ejecución precisa, no en decoración.
