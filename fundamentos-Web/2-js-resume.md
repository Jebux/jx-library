# JS: JavaScript

## 0. Comentarios

```javascript
    //Una línea 

    /*

        Múltiples líneas

    */
```

## 1. Declaración de variables

```javascript
    let x = 10;       // variable modificable
    const PI = 3.14;  // constante (no cambia)
    var y = 5;        // NO recomendado (forma vieja)
```

## 2. Tipos de datos

```javascript
    let numero = 10;          // Number
    let texto = "Hola";        // String
    let booleano = true;       // Boolean
    let nada = null;           // Null
    let indefinido;            // Undefined
    let objeto = { nombre: "Ana", edad: 25 };  // Object
    let lista = [1, 2, 3];     // Array
```

## 3. Operadores

### 3.1. Aritméticos

```javascript
    +, -, *, /,   //Suma, resta, multiplicación, división
    %,            //Modulo 
    **            //
```

### 3.2. Comparación

```javascript
    ==   // igual (compara valor)
    ===  // estrictamente igual (valor y tipo)
    !=   !== // diferente
    >    <    >=    <=  // mayor, menor, mayor o igual, menor o igual
```

### 3.3. Lógicos

```javascript
    &&   // AND
    ||   // OR
    !    // NOT
```

## 4. Strings

```javascript
    let nombre = "David";
    console.log("Hola " + nombre);
    console.log(`Hola ${nombre}`); // template strings
```

Métodos útiles

```javascript
    "texto".length
    "hola".toUpperCase()
    "HOLA".toLowerCase()
    "hola".includes("ho")
```

## 5. Funciones

```javascript
    function sumar(a, b) {
        return a + b;
    }

    const restar = (a, b) => a - b;   // función flecha
```

## 6. Condicionales

```javascript
    if (edad >= 18) {
    console.log("Mayor de edad");
    } else {
    console.log("Menor");
    }

    //Ternario 
    edad >= 18 ? console.log("Mayor de edad") : console.log("Menor");
```
```javascript
    switch (dia) {
    case 1: console.log("Lunes"); break;
    case 2: console.log("Martes"); break;
    default: console.log("Otro día");
    }
```

## 7. Bucles

```javascript
    for (let i = 0; i < 5; i++) {
        console.log(i);
    }

    let j = 0;
    while (j < 5) {
        console.log(j);
        j++;
    }

    for (let item of lista) {
      console.log(item);
    }

    lista.forEach(item => console.log(item));
```

## 8. Arrays / listas

```javascript
    let nums = [1, 2, 3];
    nums.push(4);       // agregar
    nums.pop();         // quitar último
    nums.shift();       // quitar primero
    nums.unshift(0);    // agregar al inicio
    nums.includes(2)    // verificar existencia
    nums.indexOf(3)     // índice de un elemento
```

métodos avanzados

```javascript
    nums.map(x => x * 2);          // transformar
    nums.filter(x => x > 1);       // filtrar
    nums.reduce((a, b) => a + b);  // reducir a un valor

```

## 9. Objetos

```javascript
    let persona = {
        nombre: "Luis",
        edad: 30,
        saludar: function() {
            console.log("Hola, soy " + this.nombre);
        }
    };
    console.log(persona.nombre); // acceder a propiedad
    persona.saludar();           // llamar método
```

## 10. Eventos del DOM

```javascript
    document.getElementById("miBoton").addEventListener("click", function() {
        alert("Botón clickeado");
    });
```

## 11. Manipulación del DOM

```javascript
    document.querySelector("h1").textContent = "Nuevo título";
    document.querySelector(".caja").style.background = "red";

    document.querySelector(".miClase").style.color = "red";
    let nuevoElemento = document.createElement("div");
    nuevoElemento.innerText = "Hola Mundo";
```
 
## 12. Import / Export (módulos)

```javascript
    // archivo math.js
    export function sumar(a, b) {
        return a + b;
    }

    // archivo main.js
    import { sumar } from './math.js';
    console.log(sumar(2, 3));
```

## 13. Adicionales

- JSON
- Fetch API
- Promesas
- Async/Await
- OOP
- Errores
- try/catch
- Timers (setTimeout, setInterval)