# HTML: HyperText Markaup Language 

![](/img/img-fundamentos-web/estructura-documento-html.png)

## Etiquetas relevantes

### 1. Etiquetas de texto

```html
<p>Parrafo</p>
<h1>Título 1</h1>  <!-- h1–h6 -->
<strong>Negrita semántica</strong>
<b>Negrita visual</b>
<em>Énfasis</em>
<i>Cursiva visual</i>
<u>Subrayado</u>
<br />  <!-- Salto de línea -->

```

### 2. Enlaces

```html
    <a href="#">Link</a>
    <a href="#" target="_blank" rel="noopener">Abrir en nueva pestaña</a>
```

### 3. Multimedia

```html
    <!-- Imágenes -->
    <img src="img.png" alt="Descripción" />

    <!-- Video -->
    <video src="video.mp4" controls></video>

    <!-- Audio -->
    <audio controls>
    <source src="audio.mp3" type="audio/mpeg" />
    </audio>
```
### 4. Listas

```html
    <!-- Lista desordenada (unorder) -->
    <ul>
        <li>Elemento</li>
    </ul>

    <!-- Lista ordenada (order)-->
    <ol>
        <li>Elemento</li>
    </ol>

    <!-- Lista descriptiva -->
    <dl>
        <dt>Término</dt>
        <dd>Descripción</dd>
    </dl>
```

eg. lista descriptiva

    <dl>
        <dt>HTML</dt>
        <dd>Descripción</dd>
    </dl>

### 5. Tablas

```
    <table>
        <tr>
            <th>Columna1</th>
            <th>Columna2</th>
        </tr>
        <tr>
            <td>Dato1</td>
            <td>Dato2</td>
        </tr>
    </table>

```

### 6. Formularios

```html
    <form action="/submit" method="POST">
        <input type="text" name="nombre" required />
        <input type="email" name="correo" />
        <input type="password" name="pass" />
        <input type="number" name="edad" />
        <textarea name="mensaje"></textarea>

        <select name="pais">
            <option value="co">Colombia</option>
            <option value="mx">México</option>
        </select>

        <input type="checkbox" name="acepto" />
        <input type="radio" name="genero" value="m" />

        <button type="submit">Enviar</button>
    </form>

```
    
### 7. Contenedores y estructuras

```html
    <div>Bloque genérico</div>
    <span>En línea</span>
    <header>Encabezado</header>
    <nav>Navegación</nav>
    <section>Sección</section>
    <article>Artículo</article>
    <aside>Lateral</aside>
    <footer>Pie de página</footer>
```

#### Html Semántico
![](/img/img-fundamentos-web/html-semantico.png)
- Usar etiquetas que describen el propósito del contenido en lugar de etiquetas genéricas como "div"
- Beneficios:
    - Mejora accesibilidad, facilita el SEO y aumenta la legibilidad del código.

### 8. Metaetiquetas importantes

```html
    <meta charset="UTF-8" />
    <meta name="description" content="Descripción de la página" />
    <meta name="keywords" content="html, css, web" />
    <meta name="author" content="Tu nombre" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
```
### 9. Scripts  y estilos

```html
    <link rel="stylesheet" href="styles.css" />
    <script src="app.js"></script>
```

### 10. Atributos globales clave
```html
id="identificador"
class="clase"
style="color: red;"
title="tooltip"
data-id="123"
```
### 11. Caracteres especiales

- [Códigos HTML - Tabla de caracteres y símbolos](https://ascii.cl/es/codigos-html.htm)

# CSS:Cascading Style Sheets

## 1. Conectar CSS

```html 
    <!-- Archivo externo -->
    <link rel="stylesheet" href="styles.css">

    <!-- En el mismo archivo de HTML -->
    <style>
        h1 { color: red; }
    </style>

    <!-- Inline -->
    <h1 style="color:red;">Hola</h1>
```

## 2. Selectores básicos

```css 
    // etiquetas 
    h1 { }
    p { }

    // Por clase
    <style>
        h1 { color: red; }
    </style>

    // Por id
    <h1 style="color:red;">Hola</h1>

    //Selección de hijos
    div p { }     /* p dentro de div */
    div > p { }   /* hijo directo */

    //Selección múltiple
    h1, h2, h3 { color: blue; }
```

## 3. Propiedades

- Texto
- Colores
- Fondos
- Modelo de caja (Box Model)
    - Dimensiones
    - Padding, border, margin
- Display
- Flexbox
- Grid
- Posicionamiento
- Bordes y esquinas
- Sombras
- Transiciones
- Tranformaciones
- Overflow
- Z-index

## 4. Unidades comunes

```css
    px      /* píxeles */
    %       /* porcentaje */
    em      /* relativo al font-size del elemento */
    rem     /* relativo al font-size del html */
    vh      /* 1% del alto del viewport */
    vw      /* 1% del ancho del viewport */

```

## 5. Media Queries (responsive)

```css
    @media (max-width: 768px) {
        body {
                background: lightblue;
            }
    }
```

## 6. Variables CSS

```css
    :root {
        --color-primary: #00bfff;
    }

    button {
        color: var(--color-primary);
    }
```

## Animaciones

```css
    @keyframes mover {
        from { transform: translateX(0); }
        to   { transform: translateX(100px); }
    }

    div {
        animation: mover 2s infinite;
    }

```


## Ejemplos

```html 
            <!-- 01 crear carpeta -->
            <!-- 02 abrir foldel visual -->
            <!-- 03 crear archivo -->
            <!-- 04 code. html5 -->
            <body>
                <h1>
                    Hello world 
                </h1>
                <div style="height: 155px; width:335px; background-color: black; display:flex; flex-direction: column ;align-items: center; justify-content: center;">
                    <h1 style="color:white">Dentro de la caja</h1>
                    <input type="text" placeholder="Digite su nombre" style="width: 150px; margin-bottom: 10px;">
                    <button>Enviar</button>
                </div>
            </body>


```
<div style="display:flex; flex-direction: column; align-items: center; justify-content: center; margin: 20px; border: 2px dotted black; padding:15px;">
    <h1>
        Hello world 
    </h1>
    <div style="height: 155px; width:335px; background-color: black; display:flex; flex-direction: column ;align-items: center; justify-content: center;">
        <h1 style="color:white">Dentro de la caja</h1>
        <input type="text" placeholder="Digite su nombre" style="background: white; width: 200px; margin-bottom: 10px;">
        <button>Enviar</button>
    </div>
</div>

```html
    <head>
        <style>
            div{
                height: 155px; 
                width:335px; 
                background-color: black; 
                display:flex; 
                flex-direction: column ;
                align-items: center; 
                justify-content: center;
                }
            h1{
                color:white
                }
            input{
                width: 150px; 
                margin-bottom: 10px;
                }
        </style>
    </head> 
```
