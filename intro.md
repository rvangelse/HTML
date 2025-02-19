# HTML

HTML (HyperText Markup Language) es un lenguaje de marcado de texto. Define la estructura y el contenido de una pagina web. Es un lenguaje de alto rendimiento, interpretado y de codigo abierto. Fue creado por Tim Berners-Lee en 1990.

<p align="center">
  <img src="imagenes/grafico7.png" width="600">
</p>

---

### Estructura básica de HTML en una página Web

<p align="center">
  <img src="imagenes/grafico4.webp" width="200">
</p>

- Container: Contenedor principal
- Header: Cabecera de la página. Aquí usualmente encuentras el logo y el menú de navegación del sitio.
- Main content: Estructura principal. Por ejemplo, el feed o lista de publicaciones de una red social.
- Sidebar: Contenido secundario de una página, que usualmente se encuentra a los lados del contenido principal (o main).
- Footer: Pie de página. Esto se encuentra al fondo del sitio web, salvo en casos de sitios web donde el scroll (o navegación hacia abajo) es infinito, por ende, no tendría sentido ponerlo al fondo.

---

### Document Object Model (DOM)

Es el arbol que se forma en el archivo html, es decir, la representacion del HTML en tu pagina.

La raíz de la estructura de árbol de HTML es la etiqueta `<html>`, que contiene dos
nodos principales: `<head`> y `<body>`

---

### Index y su estructura básica: head

El primer archivo .html en tu proyecto debe llamarse `index.html`, es la primera pagina que va abrir el servidor, por default, al abrir tu proyecto.
Si no lo haces e `index.html` no existe, el servidor te devolvera toda la estructura de carpetas de archivos de tu proyecto.

En el `head` van todos los metadatos importantes para que el navegador pueda cargar el proyecto. Esto no es visual para el usuario.

``` html
<!DOCTYPE html>
<html lang= "es"> 
    <head>
        <meta charset= "UTF-8" />
        <meta name="description" content="Esta pagina te mostrara fotos de gatos" />
        <meta name="robots" content="index,follow"/>
        <title>Es mi pagina</title>
        <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
        <link rel="icon" href="/favicon.ico" /> <!-- Icono -->
        <link rel="preload" href="/font.woff2" as="font" type="font/woff2" crossorigin="anonymous" /> <!-- Fuente importada -->
        <link rel="stylesheet" href="css/style.css" /> <!-- CSS -->
        <script src="js/script.js"></script> <!-- JS -->
    </head>
</html>
```
---

### Index y su estructura básica: body

El `body` es la etiqueta que identifica la parte visible de nuestro sitio web. Dentro del `body`, se añadirán las etiquetas para marcar los elementos visuales del sitio web, como logotipo, menús de navegación, contenido principal, entre otros.

```html

<!-- Estructura Semántica-->
<!DOCTYPE html>
<html lang= "es">
<body>
    <nav></nav>
    <!-- Encabezado -->
    <header>
        <h1></h1>
    </header>
    <!-- Contenido principal -->
    <main>
        <!-- Artículo: Unidad de información -->
        <article></article>
        <!-- Secciones de contenido -->
        <section></section>
        <!-- Contenido de lado -->
        <aside></aside>
    </main>
    <!-- Pie de página -->
    <footer></footer>
</body>

```
OJO: No uses divs ni tablas para agrupar contenido. Usa etiquetas semánticas.

---

### Anatomía de una etiqueta de HTML

<p align="center">
  <img src="imagenes/grafico6.png" width="350">
</p>
