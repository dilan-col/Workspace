## 1. ¿Cómo se documenta el código? Diferencias entre Backend y Frontend

Documentar código significa poner explicaciones dentro del código para saber qué hace cada parte. Esto ayuda a que nosotros u otras personas podamos entender el código más fácilmente.

Una forma sencilla de documentar es utilizando comentarios.

En JavaScript podemos hacer un comentario de una línea utilizando `//`:

```javascript
// Esta variable guarda el nombre del usuario
let nombre = "Dilan";
```

También podemos hacer comentarios de varias líneas:

```javascript
/*
Este código realiza una operación
con dos números.
*/
```

### Backend

El Backend es la parte del programa que trabaja detrás de la aplicación. Se encarga de cosas como guardar información, trabajar con bases de datos y procesar los datos que envía el usuario.

Al documentar el Backend podemos explicar qué hace una función, qué datos recibe y qué resultado entrega.

Ejemplo:

```javascript
// Busca un usuario por su nombre
function buscarUsuario(nombre) {
    // Código para buscar el usuario
}
```

### Frontend

El Frontend es la parte que podemos ver y utilizar. Por ejemplo, los botones, formularios, textos y menús de una página.

Al documentar el Frontend podemos explicar para qué sirve un botón, una función o una parte de la interfaz.

Ejemplo:

```javascript
// Muestra un mensaje cuando el usuario presiona el botón
function mostrarMensaje() {
    alert("Hola");
}
```

En resumen, el **Backend** se encarga principalmente de la parte interna de la aplicación, mientras que el **Frontend** se encarga de la parte que ve y utiliza el usuario.

---

## 2. ¿Cómo se documenta código para JavaScript?

En JavaScript se puede documentar utilizando comentarios. Los comentarios no afectan el funcionamiento del programa, solamente sirven para explicar el código.

Para un comentario corto se utiliza `//`.

```javascript
// Suma dos números
function sumar(a, b) {
    return a + b;
}
```

Para un comentario más largo se utilizan `/* */`.

```javascript
/*
Esta función recibe dos números
y devuelve el resultado de la suma.
*/
function sumar(a, b) {
    return a + b;
}
```

También podemos escribir comentarios para explicar variables:

```javascript
// Guarda el nombre del usuario
let nombre = "Dilan";

// Guarda la edad del usuario
let edad = 16;
```

Es importante no poner comentarios innecesarios en todas las líneas. Lo mejor es utilizarlos cuando una parte del código necesita una explicación.

Por ejemplo, en este código el comentario ayuda a entender qué hace la función:

```javascript
// Calcula el precio total
function calcularTotal(precio, cantidad) {
    return precio * cantidad;
}
```

---

## 3. ¿Cómo se documenta código para React, en específico?

React también utiliza JavaScript, por lo que podemos utilizar los mismos comentarios. Sin embargo, en React es común documentar principalmente los **componentes**, las **funciones**, los **estados** y las acciones que realizan los botones.

Por ejemplo, podemos documentar un componente:

```jsx
// Componente que muestra un saludo
function Saludo() {
    return <h1>Hola</h1>;
}
```

También podemos documentar una función:

```jsx
// Esta función muestra un mensaje
function mostrarMensaje() {
    alert("Hola usuario");
}
```

Si utilizamos `useState`, podemos explicar para qué sirve:

```jsx
import { useState } from "react";

function Contador() {

    // Guarda el número del contador
    const [contador, setContador] = useState(0);

    // Aumenta el contador
    function aumentar() {
        setContador(contador + 1);
    }

    return (
        <div>
            <p>{contador}</p>
            <button onClick={aumentar}>Aumentar</button>
        </div>
    );
}
```

También podemos documentar las partes importantes de un formulario:

```jsx
// Guarda el nombre escrito por el usuario
const [nombre, setNombre] = useState("");
```

En React es importante que los comentarios expliquen qué hace cada componente o función cuando no sea fácil entenderlo solamente viendo el código.

En conclusión, para documentar código en React podemos utilizar comentarios para explicar los componentes, funciones, estados, botones y otras partes importantes de la aplicación.
