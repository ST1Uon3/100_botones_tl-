# Catálogo de Botones CSS

Página web que reúne **99 botones** diseñados con CSS, organizados en **10 secciones** que avanzan de lo básico a lo avanzado. El objetivo es practicar y documentar las técnicas de estilo más usadas en botones: colores, bordes, tipografía, degradados, estados, transformaciones, iconos, pseudoelementos, animaciones y diseños de tendencia.

---

## Tabla de contenido

1. [Descripción del proyecto](#descripción-del-proyecto)
2. [Tecnologías utilizadas](#tecnologías-utilizadas)
3. [Estructura del proyecto](#estructura-del-proyecto)
4. [Cómo ejecutarlo](#cómo-ejecutarlo)
5. [Estructura de la página](#estructura-de-la-página)
6. [Detalle de las 10 secciones](#detalle-de-las-10-secciones)
7. [Técnicas de CSS practicadas](#técnicas-de-css-practicadas)
8. [Accesibilidad](#accesibilidad)
9. [Convenciones de nombres](#convenciones-de-nombres)
10. [Observaciones y mejoras pendientes](#observaciones-y-mejoras-pendientes)

---

## Descripción del proyecto

Es una página de una sola vista titulada **«Catálogo de Botones CSS»**. Cada sección es una tarjeta que agrupa botones de una misma familia de técnicas, con su nivel de dificultad indicado en el título (básico, intermedio, avanzado o desafío final).

Los botones **no usan las clases de botón de Bootstrap** (`.btn`, `.btn-primary`, etc.) para su apariencia: todo el diseño de cada botón está escrito en una hoja de estilos propia (`styles.css`). Bootstrap se usa únicamente para la **maquetación** (cuadrícula, espaciados y utilidades flex).

## Tecnologías utilizadas

| Tecnología | Uso |
|---|---|
| **HTML5** | Estructura semántica de la página (`main`, `section`, `button`, `h1`, `h3`). |
| **CSS3** | Estilo de todos los botones en `styles.css` (degradados, transiciones, transformaciones, animaciones, pseudoelementos). |
| **Bootstrap 5.3.3** (CDN) | Solo maquetación: `container`, `row`, `col-md-6`, `g-4`, `d-flex`, `flex-wrap`, `gap-3`, `py-5`, `mb-5`, `text-center`, `fw-bold`, `p-2`, `rounded`, `h-100`. |
| **SVG en línea** | Icono de estrella dentro del botón circular. |
| **Caracteres Unicode** | Iconos simples como `←`, `→`, `↓`, `↻`, `★`, `✦` y el emoji `🔍`. |

## Estructura del proyecto

```
proyecto/
├── index.html        # Página con los 99 botones
├── styles.css        # Estilos de todos los botones y de las tarjetas
├── img/
│   └── flor.jpg      # Imagen usada en los botones de la sección 7 y en el botón cinematográfico
└── README.md
```

> El archivo HTML hace referencia a `styles.css` e `img/flor.jpg`. Ambos deben estar en las rutas indicadas para que la página se vea completa.

## Cómo ejecutarlo

1. Descarga o clona el proyecto y comprueba que existan `styles.css` y la carpeta `img/` con `flor.jpg`.
2. Abre `index.html` con doble clic en cualquier navegador moderno (Chrome, Edge, Firefox o Safari).
3. Se necesita conexión a internet, porque Bootstrap se carga desde el CDN de jsDelivr.

No requiere instalación, compilación ni servidor.

## Estructura de la página

- Un contenedor principal (`<main class="py-5">` con `.container`) centra todo el contenido.
- El título `h1` está centrado y en negrita.
- Las 10 secciones están en una cuadrícula de Bootstrap (`.row.g-4`), con **dos tarjetas por fila** en pantallas medianas o grandes (`.col-md-6`) y **una por fila** en pantallas pequeñas.
- Cada tarjeta es un `<section class="section-card h-100">`: `h-100` hace que las tarjetas de una misma fila tengan la misma altura.
- Dentro de cada tarjeta, los botones van en un contenedor flexible (`d-flex flex-wrap align-items-center gap-3`) que los acomoda en varias líneas con separación uniforme.

## Detalle de las 10 secciones

### 1. Fundamentos y colores (básico)
Paleta base de botones, con una clase por cada color o rol.

| Clase | Botón |
|---|---|
| `btn-primary` | Primario |
| `btn-secondary` | Secundario |
| `btn-success` | Éxito |
| `btn-danger` | Peligro |
| `btn-warning` | Advertencia |
| `btn-info` | Información |
| `btn-dark` | Oscuro |
| `btn-light` | Claro |
| `btn-text` | Texto (sin relleno) |
| `btn-custom` | Personalizado |

### 2. Bordes, tamaños y formas (básico)
Variaciones de contorno, radio de esquinas y dimensiones.

| Clase | Botón |
|---|---|
| `btn-outline` | Contorno |
| `btn-border-thick` | Borde grueso |
| `btn-border-dashed` | Borde discontinuo |
| `btn-border-dotted` | Borde punteado |
| `btn-rounded` | Esquinas redondeadas |
| `btn-pill` | Forma de píldora |
| `btn-circle` | Circular, con icono de estrella en SVG |
| `btn-small` | Tamaño pequeño |
| `btn-large` | Tamaño grande |
| `btn-full` | Ancho completo |

### 3. Tipografía y sombras (básico a intermedio)
Efectos sobre el texto y sobre la caja del botón.

| Clase | Botón |
|---|---|
| `btn-uppercase` | Mayúsculas |
| `btn-spaced` | Espaciado entre letras |
| `btn-bold` | Negrita |
| `btn-elegant` | Tipografía elegante |
| `btn-underline` | Subrayado |
| `btn-shadow-soft` | Sombra suave |
| `btn-shadow-strong` | Sombra pronunciada |
| `btn-shadow-color` | Sombra de color |
| `btn-relief` | Relieve |
| `btn-text-glow` | Texto brillante |

### 4. Degradados (intermedio)
Uso de `linear-gradient` y `radial-gradient` en distintas direcciones y combinaciones.

| Clase | Botón |
|---|---|
| `btn-gradient-horizontal` | Degradado horizontal |
| `btn-gradient-vertical` | Degradado vertical |
| `btn-gradient-diagonal` | Degradado diagonal |
| `btn-gradient-three` | Degradado de tres colores |
| `btn-gradient-radial` | Degradado radial |
| `btn-gradient-sunset` | Paleta «atardecer» |
| `btn-gradient-ocean` | Paleta «océano» |
| `btn-gradient-pastel` | Paleta pastel |
| `btn-gradient-border` | Borde degradado |
| `btn-gradient-hover` | Degradado que cambia al interactuar |

### 5. Estados e interacción (intermedio)
Respuesta del botón al mouse, al clic y al teclado.

| Clase | Botón |
|---|---|
| `btn-hover-background` | Cambio de fondo al pasar el mouse |
| `btn-hover-text` | Cambio de color del texto |
| `btn-hover-border` | Cambio de borde |
| `btn-hover-shadow` | Sombra al interactuar |
| `btn-hover-underline` | Subrayado interactivo |
| `btn-active` | Estado presionado (`:active`) |
| `btn-focus` | Foco destacado (`:focus`) |
| *(atributo `disabled`)* | Botón deshabilitado |
| `btn-transition-slow` | Transición lenta |
| `btn-transition-stagger` | Transición escalonada |

### 6. Transformaciones (intermedio)
Uso de `transform` y `transition` para dar movimiento al botón.

| Clase | Botón |
|---|---|
| `btn-grow` | Crece |
| `btn-shrink` | Se reduce |
| `btn-lift` | Se eleva |
| `btn-move-right` | Se desplaza a la derecha |
| `btn-rotate` | Rota |
| `btn-skew` | Se inclina |
| `btn-press` | Efecto de presión |
| `btn-perspective` | Perspectiva 3D |
| `btn-icon-move` | Icono `→` que se mueve |
| `btn-transform-combined` | Varias transformaciones a la vez |

### 7. Iconos e imágenes (intermedio a avanzado)
Combinación de texto con iconos o con la imagen `img/flor.jpg`.

| Clase | Botón |
|---|---|
| `btn-icon-left` | Icono a la izquierda (`←`) |
| `btn-icon-right` | Icono a la derecha (`→`) |
| `btn-icon-only` | Solo icono (`🔍`), con `aria-label="Buscar"` |
| `btn-download` | Icono de descarga (`↓`) |
| `btn-image-background` | Imagen como fondo |
| `btn-image-overlay` | Imagen con capa superpuesta |
| `btn-avatar` | Imagen tipo avatar junto al texto |
| `btn-icon-separated` | Icono en una zona separada del texto |
| `btn-image-hover` | Imagen que reacciona al interactuar |
| `btn-icon-reveal` | Icono que aparece al interactuar |

### 8. Efectos con pseudoelementos (avanzado)
Efectos creados con `::before` y `::after`, normalmente con el texto envuelto en un `<span>` para controlar la capa de contenido.

| Clase | Botón |
|---|---|
| `btn-fill-left` | Relleno que entra desde un lado |
| `btn-fill-bottom` | Relleno desde abajo |
| `btn-fill-center` | Relleno desde el centro |
| `btn-shine` | Brillo que se desliza |
| `btn-underline-expand` | Línea inferior que se expande |
| `btn-corners` | Esquinas destacadas |
| `btn-double-layer` | Doble capa |
| `btn-circle-expand` | Círculo que se expande |
| `btn-border-reveal` | Borde que se dibuja al interactuar |
| `btn-diagonal-sweep` | Barrido con corte diagonal |

### 9. Animaciones CSS (avanzado)
Animaciones con `@keyframes` que se ejecutan por sí solas, sin necesidad de interacción.

| Clase | Botón |
|---|---|
| `btn-pulse` | Pulso |
| `btn-heartbeat` | Latido |
| `btn-float` | Flotante |
| `btn-shake` | Sacudida |
| `btn-bounce` | Rebote |
| `btn-glow-pulse` | Brillo pulsante |
| `btn-gradient-motion` | Degradado en movimiento |
| `btn-icon-spin` | Icono `↻` giratorio |
| `btn-loading` | Estado de carga con `.spinner` |
| `btn-sequence` | Secuencia de animaciones |

### 10. Botones de diseño avanzado (desafío final)
Estilos de tendencia que combinan varias de las técnicas anteriores. Tres de ellos necesitan un contenedor propio que crea el entorno visual donde se aprecia el efecto.

| Clase | Botón | Contenedor |
|---|---|---|
| `btn-neon` | Neón | — |
| `btn-glass` | Cristal (*glassmorphism*) | `.glass-env` |
| `btn-neumorphic` | Neumórfico | `.neumorphic-env` |
| `btn-retro-3d` | Retro 3D | — |
| `btn-metallic` | Metálico | — |
| `btn-rainbow-border` | Borde arcoíris | — |
| `btn-double-text` | Doble texto (texto inicial y texto revelado) | — |
| `btn-cinematic` | Imagen cinematográfica | — |
| `btn-premium` | Acción premium con icono `✦` | — |

> Esta sección tiene **9 botones** en lugar de 10. Con las demás suman 99 en total.

## Técnicas de CSS practicadas

- **Modelo de caja:** `padding`, `border`, `border-radius`, `width`, tamaños y formas.
- **Color y fondo:** colores sólidos, `linear-gradient`, `radial-gradient`, `background-clip` y fondos con imagen.
- **Tipografía:** `text-transform`, `letter-spacing`, `font-weight`, `text-decoration` y `text-shadow`.
- **Sombras:** `box-shadow` y `text-shadow` (suaves, fuertes, de color, en relieve y de brillo).
- **Pseudoclases:** `:hover`, `:active`, `:focus` y `:disabled`.
- **Transiciones:** `transition` con distintas duraciones y retardos.
- **Transformaciones:** `scale`, `translate`, `rotate`, `skew` y `perspective`.
- **Pseudoelementos:** `::before` y `::after` para rellenos, brillos, líneas y capas decorativas.
- **Animaciones:** `@keyframes` y `animation` para pulsos, latidos, rebotes y rotaciones.
- **Diseños modernos:** neón, cristal, neumorfismo, relieve retro 3D, metal y bordes de colores.
- **Maquetación con Bootstrap:** cuadrícula de 12 columnas, utilidades flex y espaciados.

## Accesibilidad

- Los botones que contienen solo un icono incluyen `aria-label` (`btn-icon-only` y `btn-circle`).
- El icono `🔍` lleva `aria-hidden="true"` para que los lectores de pantalla no lo lean dos veces.
- En `btn-double-text`, el botón tiene un `aria-label` único y los dos textos están marcados con `aria-hidden="true"`, para que se anuncie una sola vez.
- Las imágenes de los botones tienen el atributo `alt`.
- Se incluye un botón con el atributo `disabled` nativo.
- El documento declara el idioma con `lang="es"`.
- Todos los elementos interactivos son `<button>`, que ya son navegables con teclado y anunciados correctamente.

## Convenciones de nombres

Las clases siguen el patrón `btn-<categoría>-<variante>`, escrito en inglés y con guiones:

- `btn-gradient-sunset` → botón, degradado, atardecer.
- `btn-hover-shadow` → botón, efecto al interactuar, sombra.
- `btn-fill-left` → botón, relleno, lado izquierdo.

Esto permite ubicar rápido el efecto de cada botón en `styles.css` y evita choques entre estilos.

## Observaciones y mejoras pendientes

- **Falta una etiqueta de cierre.** La sección 7 («Iconos e imágenes») no cierra su `<section>`: después de `</div>` de los botones hay otro `</div>` sin `</section>` de por medio. Conviene agregarla para que el HTML sea válido y no afecte la estructura de la cuadrícula.
- **Dependencia de la imagen.** Cuatro botones (`btn-image-background`, `btn-image-overlay`, `btn-avatar`, `btn-image-hover`) y el botón `btn-cinematic` usan `img/flor.jpg`. Si la ruta cambia, esos botones se verán rotos.
- **Dependencia del CDN.** Sin internet, Bootstrap no carga y se pierde la maquetación en cuadrícula.
- **Nombres que se parecen a Bootstrap.** Clases como `btn-primary` o `btn-danger` coinciden con nombres de Bootstrap. Funciona porque no se usa `.btn` junto a ellas, pero puede generar confusión. Se podría usar un prefijo propio (por ejemplo `my-btn-primary`).
- **Animación y movimiento reducido.** La sección 9 tiene animaciones continuas. Se recomienda agregar `@media (prefers-reduced-motion: reduce)` en `styles.css` para quienes prefieren menos movimiento.
- **Contraste.** Algunos estilos (pasteles, botón claro, neumórfico y cristal) deben revisarse con una herramienta de contraste para cumplir WCAG AA.
- **Posibles mejoras futuras:** mostrar el código CSS de cada botón al hacer clic, agregar un botón «copiar» y un modo oscuro para la página.


# 100 Botones
## Diseño Original

Usé:
Dos `@keyframes` (`glow-pulse` y `heartbeat`) con la primera repitiendose infinitamente cada 2s y la segunda cada 1.5s, de fondo le puse una imagen con la clase `transition-transform` y un hover para que cuando le pases el mouse se acerque la imagen, por ultimo agregué el cambio de borde de `pink` a `palevioletred` quedando así con 4 de las clases que mas me llamaron la atención

---

## Créditos

- Maquetación: [Bootstrap 5.3.3](https://getbootstrap.com/)
- Iconos: SVG de [Bootstrap Icons](https://icons.getbootstrap.com/) y caracteres Unicode.
