# Contenido

### Contenedores
```html
<!-- Bloque. Se utiliza para agrupar etiquetas -->
<div>Soy un Div</div>
<div>Soy un Div</div>
<div>Soy un Div</div>
<!-- En línea. Se usa para un grupo más pequeño de una o más palabras, junto con atributos -->
<span>Soy un Span</span>
<span>Soy un Span</span>
<span>Soy un Span</span>

```
OJO: Usa `<span>` y `<div>` solo para encapsular estilos que verás en CSS.

### Atributos Globales
```html
<!--Sirve para identificar una etiqueta -->
<p id="parrafo1">No hay nadie como yo</p>
<!-- Sirve para identificar un grupo de etiquetas -->
<p class="muchos">Unidos somos más</p>
<!-- Sirve para marcar como editable un texto-->
<p contenteditable="true">Puedes editar este contenido</p>
<!-- Indica el idioma del parrafo -->
<p lang="es">Esto está escrito en español</p>
<!-- Indica el sentido de la escritura del parrafo -->
<p dir="rtl">Esto está escrito en العربية (árabe)</p>
```
### Accesibilidad
```html
<!-- Sirve para mejorar la accesibilidad de una seccion -->
<div aria-label="H2O">
    <div aria-hidden="true">
        <span>H</span>
        <span>2</span>
        <span>O</span>
    </div>
</div>
```
OJO: No ignores la accesibilidad. No solo se hace por ayudar a los usuarios, también expande el tráfico y mejora el SEO.

---

### Practica 6: Div, Span y atributos

**Codigo**
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejemplo de HTML con Div, Span y Atributos</title>
</head>
<body>
    <header>
        <h1>Ejemplo de HTML con Div, Span y Atributos</h1>
    </header>
    <section>
        <div id="contenedor-1" class="contenedores">
            <span>Este es un div con algunos atributos, como un ID y una clase. Este es un span dentro del div.</span>
        </div>
            <p lang="en">This is a paragraph that is not inside the div.</p>
    </section>
</body>
</html>
```

**Output**
<p align="center">
  <img src="imagenes/grafico14.png" width="450">
</p>