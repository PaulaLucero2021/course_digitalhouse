---
title: "Front End II"
author: "Liliana Ospina"
output: PDF_document
lang: es-ES
toc: TRUE
---

<style>

@import url('https://fonts.googleapis.com/css2?family=Roboto+Mono&display=swap');
t {
    font-size: 50px;
    color: #006d77;
    font-family: 'Roboto Mono', monospace;
    letter-spacing: 5px;
}
h1 {
color: #f2cc8f
}
h2 {
color: #e07a5f;
}
h3 {
color: #cd9777
}
r {
color: #03045e;
background-color: #90e0ef;
}
</style>

<t>Front End II</t>

---

## Índice

1. Bienvenida e Introducción a Javascript Front
- [C1 - Bienvenida](#c1)
    - [Introduccion a la materia](#c1a)
    - [Origen de JavaScript](#c1b)
    - [DevTools: Consola](#c1c)
    - [console.log()](#c1z)
    - [alert()](#c1y)
    - [Vinculando HTML y JavaScript](#c1s)
- [C2 - Introducción a JavaScript Front](#c2)
2. Manipulacion del DOM
3. Web reactica
4. Validacion del lado del cliente
5. Asincronismo y APIs
6. implementación practica, animaciones y librerias


# C1 - Introduccion <a id='c1'></a>


[Modulos de Front End](https://view.genial.ly/60ab9dbe27391f0d8711d89a) <a id='c1a'></a>

## Origen de Javascript <a id='c1b'></a>

> Ver video: Conociendo Javascript

<!-- inicio resumen video -->

Primero llamado *Mocha*, luego *LiveScript* luego ***Javascript***

![JavaScript](./img/c1.1.png)

### Cronologia

![JavaScript2](./img/c1.2.png)
![Js](./img/c1.3.png)

### Evolucion Javascript

![Progreso](./img/c1.3.png)

<!-- Fin resumen video -->

> ver repaso PDF: repaso-javascript

***

## Conociendo la consola del navegador <a id='c1c'></a>

> Ver pdf: devtools

<!-- Inicio resumen pdf -->

La consola es una herramienta que tenemos los desarrolladores en el navegador para tomar decisiones sobre nuestro proyecto al mismo tiempo que es interpretado por Chrome.

¿qué podemos hacer con ella?Cuando algo no funciona como queremos, podemos pasar mucho tiempo intentando descubrir cuál es el problema y arreglarlo. Por eso, la consola nos sirve para agilizar este proceso porque nos señala qué ocurre cuando ejecutamos una tarea o petición al servidor. Puede ser que nos devuelva el dato que buscábamos, un error o un aviso (warning). A este proceso se lo llamadepurar el código o debugging.

**Elements y Styles**

En la pestaña Elements veremos el código HTML y en Styles, nuestro CSS. Si hacemos clic en la flecha indicada en la imagen y luego, colocamos el mouse sobre los elementos en pantalla, nos daremos cuenta fácilmente dónde se encuentran en el código para poder manipularlos y apreciar el cambio sin tener que ir al editor de texto y guardar.

## Tipos de errores

Existen varios tipos de errores, en la consola se muestran en color rojo. Por ahora, los más comunes que vamos a conocer son: 
- **SyntaxError**: Representa un error de sintaxis en el lenguaje representado en JavaScript.
- **TypeError**: Representa un error que ocurre cuando una variable o parámetro no es de un tipo válido, es decir, `undefined`.

## Responsive

Muchas veces necesitamos adaptar nuestra web para poder visualizarlas correctamente en distintos dispositivos. En la parte superior del inspector hay un icono de dispositivo, al hacer clic podemos determinar la resolución de pantalla o, directamente elegir un dispositivo.

## Application

Con la pestaña Application podremos ejecutar tareas respecto a los datos que se guardan por el cliente en nuestra web por cierta cantidad de tiempo. Como, por ejemplo, borrar de la memoria los datos ingresados en el login de un usuario.

*Lighthouse* es una herramienta que genera reportes para comprobar ciertos recursos que debe tener la web para que sea óptima. Algunos de ellos son:

- performance, 
- accesibilidad y 
- SEO.

<!-- fin resumen pdf -->

> Ver PDF: Javascript: Baby steps

<!-- inicio resumen pdf -->

## Primeros pasos en JavaScript

### `console.log()` <a id='c1z'></a>

Ahora que conocemos la consola como parte de las herramientas que debemos utilizar al desarrollar, pongamos en práctica algunas líneas de código.

Lo clásico sería mostrar un mensaje por consola, para eso, debemos implementar el método `log()` del objeto `Console`. Entonces, ¿cómo sería?

```javascript
console.log('Esto es un mensaje por consola');
```
Podemos probar ejecutar la misma sentencia con diferentes mensajes, incluso con
distintos tipos de datos y deberíamos tener el mismo resultado. Por ejemplo:

```javascript
console.log('Hola, soy otro texto');
console.log(25);
console.log(true);
```

**Variantes**

Como alternativas al .log() —pero rara vez implementadas— está bueno saber que
existen otros métodos como:

`.error()` Escribe un error en consola

`.warn()` Escribe una advertencia en consola

`.table()` Escribe una tabla en consola

```javascript
let miObjeto = {
mensaje: "Mensaje de texto",
utilidad: "prueba de JS"
};

let miArray = [ "Primer mensaje del array", "Segundo mensaje del array",
"Tercer mensaje del array"]

console.table(miObjeto);
console.table(miArray);
```

Sigamos probando alternativas, familiarizándonos con la consola del navegador e
implementemos código para obtener distintos resultados. 
**También podemos realizar operaciones aritméticas y relacionales.**

```javascript
let numero = 5;
let numeroEnLetras = "5";

console.log(numero == numeroEnLetras);
console.log(numero === numeroEnLetras);
```

### `alert()` <a id='c1y'></a>

Así como mostramos mensajes por consola, los cuales son muy útiles para debbuggear nuestro código, también tenemos mensajes de alerta que puede ver el
usuario.
El método `alert()` pertenece al objeto `window`, pero para utilizar podemos
directamente implementarlo en la consola.

```javascript
alert('Esto es una alerta');
```
El método muestra una caja de alerta con el mensaje que le pasamos por parámetro y un botón de OK. Justamente es implementado para mostrarle al usuario cierta información que creamos importante. De esta manera simple y rápida ya podemos comunicarnos con el usuario.

No se trata de la interfaz más bonita del mundo, pero al menos así podemos mostrar
un cartel inevitable a la vista.


**Quizz**

¿Qué combinación de teclas abre la consola del navegador? 
Ctrl, Shift + I
¡Correcto! Además de F12, podemos utilizar la combinación Ctrl, Shift + I

Puedo crear una variable directamente en la consola. 
Verdadero

La consola solo es visible para los usuarios que están logueados. 
Falso

A través de la consola puedo modificar páginas web.
Verdadero

¿Cuál es la función principal de la consola? 
Depurar páginas web.

¿Puedo activar o desactivar la consola en mi sitio web? 
Jamás, es una herramienta del navegador.

Al cerrar la consola pierdo todos los cambios que realicé en la misma. 
Falso
¡Correcto! Las variables se mantienen hasta que se cierre o cambie de página el sitio.

<!-- inicio pdf clase sincronica c1 -->

> Ver pdf: Vinculando HTML y JavaScript.pdf

## Vinculando HTML y JavaScript <a id='c1s'></a>

### Vinculación interna

Nos permite escribir código JavaScript directamente en nuestro archivo HTML. Sin embargo, esta no es la forma más prolija de trabajar.

```javascript
<body>

<script>
console.log(“HolaMundo!”);  
</script>

</body>
```

### Vinculación externa

Nos permite linkear nuestro archivo HTML con un archivo JavaScript externo

```javascript
<body> 

<script src="js/main.js"> </script>

</body>
```

Recordemos que, con el uso de la vinculación externa, no es necesario escribir las etiquetas `<script>` dentro de nuestro archivo con extensión **.js**

```javascript
let saludo='Hola mundo!';

console.log(saludo);
```
<!-- fin pdf clase sincronica -->


# C2 - Introducción a JavaScript Front <a id='c2'></a>
