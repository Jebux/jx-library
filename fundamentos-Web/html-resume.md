# HTML: HyperText Markaup Language 

![](https://remnote-user-data.s3.amazonaws.com/3OpV88urUOxsHXHL84ulO95Xmo3EOMFgcwWAfbKsdP0XTtDkeAd4yvKg78Gn3YB7XXVEeBVWvKkpouuzDevbRkxpYVex6yRow-q1eXhNCINNpIbeoDyESKCI6-lD0hDj.png)

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
![](https://remnote-user-data.s3.amazonaws.com/fnlKBfx8YXKJwq98v-ck5CqOd2g0RFS1jyW7ITfC_HUABWRlV6v4Y3Qsc8hqxsZ03wmrQW4INHrEMPTtlEgkZgntYDqNLTu7BJ6IW2hwVUuqCLMXVeLbbXttRwqUtRbo.png)
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
        <input type="text" placeholder="Digite su nombre" style="width: 150px; margin-bottom: 10px;">
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
