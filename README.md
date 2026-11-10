# Portafolio Personal – Piloni Bruno

Este proyecto es un portafolio web de una sola página, basado en la plantilla gratuita **Miniport** de [HTML5 UP](https://html5up.net). El presente documento describe, de forma sencilla, la función de cada sección del archivo `index.html`.

---

## 1. Estructura general del proyecto

```
/
├── index.html            → Página principal (contenido)
├── images/               → Imágenes del portafolio (pic00 a pic06)
└── assets/
    ├── css/main.css      → Estilos visuales
    └── js/               → Scripts de funcionamiento (jQuery, desplazamiento, etc.)
```

---

## 2. Encabezado del documento (`<head>`)

| Elemento | Función |
|---|---|
| `<!DOCTYPE HTML>` | Indica al navegador que el documento utiliza HTML5. |
| Comentario inicial | Reconoce la autoría de la plantilla (HTML5 UP) y su licencia CCA 3.0. |
| `<title>` | Define el título que aparece en la pestaña del navegador. Actualmente dice *"Miniport by HTML5 UP"*. |
| `<meta charset="utf-8">` | Permite mostrar correctamente tildes y caracteres especiales. |
| `<meta name="viewport">` | Adapta la página a pantallas de distintos tamaños (celulares, tabletas, computadoras). |
| `<link rel="stylesheet">` | Vincula la hoja de estilos `assets/css/main.css`. |

---

## 3. Cuerpo del documento (`<body>`)

El `<body>` contiene la clase `is-preload`, utilizada por la plantilla para activar animaciones de carga inicial.

### 3.1 Navegación (`<nav id="nav">`)

Menú superior con cuatro enlaces internos que dirigen a cada sección de la página:

- **Inicio** → `#top`
- **Yo** → `#work`
- **Trabajos** → `#portfolio`
- **Contacto** → `#contact`

### 3.2 Sección de Inicio (`#top`)

Presentación principal del portafolio. Está dividida en dos columnas:

- **Columna izquierda:** fotografía de perfil (`images/pic00.jpeg`).
- **Columna derecha:** saludo con el nombre del autor, una breve frase de bienvenida y un botón (*"Esto es lo que hago"*) que desplaza suavemente hacia la siguiente sección.

### 3.3 Sección "Yo" (`#work`)

Presenta las cualidades personales del autor mediante tres tarjetas (`box style1`), cada una con un ícono, un título y una descripción:

1. **Comunicación para trabajar en equipo**
2. **Creativo**
3. **Mentalidad positiva**

Al final se incluye un botón que dirige a la sección de proyectos.

### 3.4 Sección de Trabajos (`#portfolio`)

Muestra seis proyectos en formato de cuadrícula. Cada tarjeta (`box style2`) contiene una imagen, un título y una breve descripción:

| Proyecto | Descripción |
|---|---|
| Juego simple de Quiz | Preguntas y respuestas de fútbol. |
| Una pequeña app de hábitos | Sencilla pero útil. |
| Calculadora de Propinas | Enfocada en aprender con cosas sencillas. |
| Adivina el Impostor | Más variables, más diversión. |
| Arma el 11 | Armado de un equipo completo. |
| Tateti | Juego clásico. |

> **Nota:** los enlaces de cada proyecto utilizan `href="#"`, por lo que aún no dirigen a ningún sitio. Deberán reemplazarse por la dirección real de cada proyecto.

### 3.5 Sección de Contacto (`#contact`)

Se compone de tres partes:

1. **Formulario de contacto:** campos para nombre, correo, asunto y mensaje, con los botones *Enviar* y *Borrar Todo*.
2. **Redes sociales:** lista de íconos (Twitter, Facebook, Dribbble, LinkedIn, Tumblr, Google+ y GitHub). Varias líneas adicionales se encuentran comentadas y pueden activarse si se desea.
3. **Pie de página (`<footer>`):** derechos de autor y crédito a HTML5 UP.

> **Nota:** el formulario utiliza `action="#"`, por lo que actualmente **no envía** los datos a ningún destino. Para que funcione se requiere un servicio externo (por ejemplo, Formspree) o un servidor propio.

---

## 4. Scripts (al final del `<body>`)

Se cargan al final para no retrasar la visualización de la página.

| Archivo | Función |
|---|---|
| `jquery.min.js` | Biblioteca base de JavaScript. |
| `jquery.scrolly.min.js` | Genera el desplazamiento suave entre secciones. |
| `browser.min.js` | Detecta el navegador y el sistema del usuario. |
| `breakpoints.min.js` | Gestiona el diseño según el tamaño de pantalla. |
| `util.js` | Funciones auxiliares de la plantilla. |
| `main.js` | Script principal: activa el menú, animaciones y demás comportamientos. |

---

## 5. Clases CSS más utilizadas

| Clase | Significado |
|---|---|
| `wrapper style1…style4` | Define el estilo y color de fondo de cada sección. |
| `container` | Centra y limita el ancho del contenido. |
| `row` y `col-X` | Sistema de cuadrícula en columnas (12 en total). |
| `col-12-small`, `col-6-medium` | Ajuste de columnas según el tamaño de pantalla. |
| `button large scrolly` | Botón grande con desplazamiento suave. |
| `image fit` / `image featured` | Imágenes adaptadas al ancho de su contenedor. |
| `icon … fa-*` | Íconos de la biblioteca Font Awesome. |

---

## 6. Créditos

- Plantilla: **Miniport** por [HTML5 UP](https://html5up.net) (@ajlkn).
- Licencia: [Creative Commons Attribution 3.0](https://html5up.net/license).
- Contenido personalizado: Piloni Bruno.
