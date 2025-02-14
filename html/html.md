# HTML

HTML (HyperText Markup Language) es un lenguaje de marcado de texto. Define la estructura y el contenido de una pagina web. Es un lenguaje de alto rendimiento, interpretado y de codigo abierto. Fue creado por Tim Berners-Lee en 1990.

<p align="center">
  <img src="../imagenes/grafico7.png" width="600">
</p>

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
        <link rel="stylesheet" href="../css/styles.css">
    </head>
</html>
```
---

### Index y su estructura básica: body

El `body` es la etiqueta que identifica la parte visible de nuestro sitio web. Dentro del `body`, se añadirán las etiquetas para marcar los elementos visuales del sitio web, como logotipo, menús de navegación, contenido principal, entre otros.

```html

<!DOCTYPE html>
<html lang= "es"> 
    <body>
        <header>
            <nav>
            </nav>
        </header>
        <main>
            <section>
                <article>
                <h1></h1>
                <p></p> <!--Parrafo-->
                <a href="#">Link</a>
                </article>
            </section>
            <ul> <!--Lista Desordenada-->
                <li>item</li>
            </ul>
            <ol> <!--Lista Ordenada-->
            </ol>
        </main>
        <footer>
        </footer>
    </body>
</html>

```
---

### Anatomía de una etiqueta de HTML

<p align="center">
  <img src="../imagenes/grafico6.png" width="350">
</p>

---

### Texto

**Texto Semantico**

Etiquetas que ayudan a dar más significado a palabras o frases.

``` html
<!-- Ejemplos: -->
<p>Párrafo (Elemento de Bloque)</p>
<em>Énfasis</em>
<i>Voz alternativa</i>
<b>Atención utilitaria</b>
<strong>Gran importancia</strong>
<small>Pequeño comentario</small>
<span>Uso con atributos (Elemento de Línea)</span>

<!-- Truco para evitar salto de línea -->
<p>Estas&nbsp;palabras&nbsp;no&nbsp;saltan&nbsp;líneas&nbsp;en&nbsp;ventanas&nbsp;pequeñas</p>

```
**Encabezados**

``` html
<!-- Encabezados -->
<h1>Título</h1>
<h2>Subtítulo</h2>
<h3>Subtítulo</h3>
<h4>Subtítulo</h4>
<h5>Subtítulo</h5>
<h6>Subtítulo</h6>
```
OJO: Es una buena practica tener un solo titulo por pagina. 

**Listas**
```html
<!-- Listas desordenadas -->
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
<!-- Listas ordenadas -->
<ol>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ol>
<!-- Listas de definición -->
<dl>
    <dt>HTML</dt>
    <dd>Es un lenguaje de marcado de texto.</dd>
    <dd>Se utiliza para el desarrollo de páginas de Internet.</dd>
</dl>
```
OJO: Es recomendable el uso de listas anidadas, si las listas son demasiado largas.

**Formato**

``` html

<!-- Codigo -->
<p>Utiliza este código en CSS:
    <code>{ background: blue; }</code>
</p>

<p>Utiliza este código en HTML:
    <code>&lt;body&gt;</code>
</p>

<!-- Superíndice y subíndice -->
<p>CO<sub>2</sub></p>
<p>n<sup>2</sup></p>
<p>Referencia a un libro.<sup>1</sup></p>

```
**Citas**

``` html
<blockquote> <!--En bloque-->
    Primero, las máquinas harán muchos trabajos por nosotros y no serán súper inteligentes. Eso debería ser positivo si lo gestionamos bien. Unas décadas después de eso, la IA puede ser bastante fuerte como para ser una preocupación. <sup>[1]</sup>
</blockquote>
<p>1."<cite>Bill Gates dice que deberías preocuparte por la inteligencia artificial</cite>". Forbes. Febrero de 2015.</p>


<p>José Mujica dijo: <!--En linea (Citas Cortas)-->
    <q>Ser libre es gastar la mayor cantidad de tiempo de nuestra vida en aquello que nos gusta hacer.</q>
</p>

```
**Tiempo** 

```html 

<!-- Fechas y Tiempo -->
<p>Nos vemos a las 
    <time datetime="2024-04-20 10:00-0800">10</time>
</p>

```

---

### Practica 1: Lista de Compras

**Codigo**

``` html

<!DOCTYPE html>
<html lang= "es"> 
    <head>
        <meta charset= "UTF-8" />
        <meta name="description" content="Esta pagina es mi lista de compras" />
        <meta name="robots" content="index,follow"/>
        <title>Lista de Compras</title>
        <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
        <link rel="stylesheet" href="../css/styles.css">
    </head>
    <body>
        <main>
            <h1>Lista de Compras</h1>
            <ul>
                <li>Carnes</li>
                    <ol>
                        <li>Pechuga de Pollo🐔</li>
                        <li>Pescado🐠</li>
                        <li>Res🥩</li>
                    </ol>
                <li>Vegetales</li>
                    <ol>
                        <li>Aguacate🥑</li>
                        <li>Zanahorias🥕</li>
                        <li>Tomates🍅</li>
                    </ol>
                <li>Frutas</li>
                    <ol>
                        <li>Cerezas🍒</li>
                        <li>Arandanos🫐</li>
                        <li>Frutillas🍓</li>
                    </ol>
            </ul>
        </main>
        <footer>
            <p>Febrero, 2025</p>
        </footer>
    </body>
</html>

```
**Output**

<p align="center">
  <img src="../imagenes/grafico5.png" width="200">
</p>

---
### Tipos de imágenes

**Lossless (Sin pérdida)**

No pierden informacion. Pueden comprimirse, pero se podrá reconstruir su imagen al estado original.

Ejemplos:

- GIF (No se puede comprimir) (Ideal para animaciones simples)
- PNG 8 (Ideal para iconos) (Permite uso de transparencias)
- PNG 24
- SVG (Vector) (Ideal para logotipos y graficos)

**Lossy (Con pérdida)**

Pierden informacion. Por lo que pueden reducir su tamaño, son mas livianos que los archivos lossless. Son ideales para usar en sitios, donde el tamaño del archivo y la velocidad de descarga son importantes.

Ejemplos: 

- JPG/JPEG (Ideal para imagenes fijas y fotografias) (Optimas para la carga en una pagina web) 

---
### Optimizacion de imagenes

El tamaño optimo de una imagen para la web es de 70KB, en promedio. 

Para alcanzar este tamaño puedes usar paginas como: 

- [TinyPNG](https://tinypng.com/) (Comprime imagenes)
- [verexif](https://www.verexif.com/) (Elimina los metadatos en una imagen)

Puedes obtener imagenes gratuitas para tus proyectos en:

- [pexels](https://www.pexels.com/es-es/)
- [unsplash](https://unsplash.com/es)

---




