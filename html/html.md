# HTML

HTML (HyperText Markup Language) es un lenguaje de marcado de texto. Se utiliza para darle una estructura al sitio web que estás visitando. Es un lenguaje interpretado.

---

### Estructura básica de HTML en una página Web

<p align="center">
  <img src="../imagenes/grafico4.webp" width="200">
</p>

- Container: Contenedor principal
- Header: Cabecera de la página. Aquí usualmente encuentras el logo y el menú de navegación del sitio.
- Main content: Estructura principal. Por ejemplo, el feed o lista de publicaciones de una red social.
- Sidebar: Contenido secundario de una página, que usualmente se encuentra a los lados del contenido principal (o main).
- Footer: Pie de página. Esto se encuentra al fondo del sitio web, salvo en casos de sitios web donde el scroll (o navegación hacia abajo) es infinito, por ende, no tendría sentido ponerlo al fondo.

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
        <link rel="stylesheet" href="../css/styles.css">
    </head>
</html>

---

En el body, ira todo el contenido que el usuario va a ver.