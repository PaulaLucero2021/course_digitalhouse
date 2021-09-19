---
title: "Programacion rientada a objetos"
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

<t>Programacion rientada a objetos</t>

---

## Índice

1. Introducción a la programación orientada a objetos
- [C1- Que es Java](#c1)
    - [Bienvenida](#c1a)
    - [Primer acercamiendo a Java](#c1b)
    - [Primer programa](#c1c)
    - [Tipos de datos](#c1d)
    - [¿Qué es un tipo de dato?](#c1z)
    - [Actividad PG](#c1pg)
    - [Sintaxis Java](#c1y)
    - [Estructura de control if, for, while, switch](#c1e)
    - [clase en vivo](#c1s)

2. Programacion orientada a objetos en Java
3. Patrones de disenio


# C1 - Que es Java <a id='c1'></a>

## ¡Les damos la bienvenida a la materia Programación Orientada a Objetos! <a id='c1a'></a>

Durante la cursada de esta materia vas a adquirir las bases y desarrollar la capacidad de modelar y programar desde la perspectiva del paradigma orientado a objetos. También te va a permitir comprender y analizar los diferentes desafíos que enfrentan los actuales equipos de trabajo al momento de desarrollar.

Los conceptos se aplicarán en el lenguaje de programación Java, uno de los más utilizados para desarrollos en empresas IT hoy en día y el conocimiento de patrones de diseño que resultan fundamentales al momento de diseñar un software.

## Primer acercamiendo a Java <a id='c1b'></a>

> ver video: Que es Java
>
> Ver PDF: Instalación IntelliJ Idea y JDK.docx.pdf

## Primer programa <a id='c1c'></a>

> Ver video: Metodo main.mp4
>
> Ver PDF: Primer programa en Java.pdf

<!-- Resumen pdf-->

en Java el nombre de la clase y el nombre del archivo
deben coincidir —incluso en mayúsculas y minúsculas—.

Esta funcion indica el comienzo del programa

```java
public static void Main(String args[])
```

la forma de mostrar algo por consola,

```java
System.out.println("Mi primer ejemplo ");
```

Con esta instrucción también podemos concatenar un texto literal y una variable. 
Por ejemplo:

```java
int num=10;

System.out.println("El valor es " + num);
```

<!-- fin resumen -->

## Tipos de datos <a id='c1d'></a>

### Sintaxis en Java

Vamos a ver cómo se utilizan en Java algunas herramientas que ya conocemos. En algunos conceptos la sintaxis es similar a JavaScript, pero tiene algunas variaciones. Una de las cosas que es bastante diferente es el tratamiento de variables. Vamos a verlo a continuación 

> ver PDF: ¿Qué es un tipo de dato_.pdf

<!-- Resumen pdf -->

## ¿Qué es un tipo de dato? <a id='c1z'></a>

### Un lenguaje tipado

Decimos que el lenguaje de programación Java es un lenguaje fuertemente tipado.
Pero esto, ¿qué quiere decir? <r>Un lenguaje tipado es el que me exige una declaración explícita de la variable antes de comenzar a usarla.</r>

### Declaración de una variable

Entonces, para declarar una variable, es necesario indicar el tipo de dato y nombre que se le asigna. Recordar que Java es un lenguaje case sensitive, los tipos de datos siempre se escriben en minúscula. Para los tipos comunes vamos a ver una excepción: el tipo String que siempre lo inicializamos con mayúscula, como en el ejemplo a continuación.

```java
int valor;
double coeficiente;
String nombre;
```

### Uso de las variables

<r>Una vez declarada la variable, sólo podrá utilizarse con datos del tipo indicado</r>, es decir, una variable de tipo int no podrá almacenar un valor de tipo double, una variable de tipo String no podrá almacenar un valor numérico que se utilice para hacer operaciones aritméticas

### Operaciones aritméticas

Respecto a las operaciones aritméticas, debemos tomar en cuenta que <r>si se opera entre dos variables de tipo entero, el resultado es siempre un valor de tipo entero.</r>
Esto pasa con todos los tipos de datos, es decir, <r>una operación solo puede realizarse con variables del mismo tipo y el resultado mantiene el tipo de dato.</r>
Pero hay una operación en la que podríamos querer cambiar el tipo de dato y que el resultado se diera en otro.

Veamos varias situaciones 
<!-- Ver pdf situaciones con enteros y floats -->

> Ver video: Declaracion de variables.mp4

### Actividad PG <a id='c1pg'></a>

**Ejercicio 1**
Es hora de que crees tus primeras variables en java
La idea es que crees tres variables una que se va a llamar numeroEntero y va a ser de tipo int una que se va a llamar numeroConComa de tipo double y por último una llamada nombre de tipo string

Luego de declararlas asignarles un valor acorde a su tipo

```java
package com.company;
 
public class Main {
 
    public static void main(String[] args) {
        int numeroEntero = 10;
        double numeroConComa = 3.5;
        String nombre = "Lili";
    }
}
```

> Como en muchos otros lenguajes de programación, en Java podemos realizar diversas operaciones. Vamos a necesitar realizarlas para poder resolver problemáticas con nuestros futuros programas. A continuación, nos encontramos con ejercicios de operaciones y una Java cheat sheet muy útil con los principales operadores que podemos utilizar en este lenguaje. 

**Ejercicio 2**

Ahora ya te damos dos variables creadas, numeroEntero y numeroConComa;
El objetivo del ejercicio es que le asignes un valor acorde a su tipo a cada variable, el valor puede ser cualquiera mientras que respetes el tipo de dato
Luego vas a declarar la variable suma de tipo double, sumar ambos valores y asignárselos a suma

```java
package com.company;
 
public class Main {
 
    public static void main(String[] args) {
        
        int numeroEntero = 10;
        double numeroConComa = 3.4;
        double suma;
        suma = (double)numeroEntero + numeroConComa;
    }
}
```

## Sintaxis Java <a id='c1y'></a>

> Ver PDF: Sintaxis Java

Matematicos |  |
------- | -------
Suma | +
Resta | -
División | /
Multiplicación | *
Módulo | % (devuelve el resto de una división entera)
Operador unario sumar 1 | ++
Operador unario restar 1 | --


Operadores logicos | |
------------------ | -------
Y | && (devuelve verdadero si las dos evaluaciones son verdaderas)
O | 2palitos (devuelve verdadero si una de las dos evaluaciones son verdaderas)
No | ! (devuelve lo opuesto al resultado de la evaluación)


Operadores relacionales | |
------- | -------
Mayor | >
Menor | <
Igual | == o .equals()
Mayor o igual | >=
Menor o igual | <=
No igual | !=

Tipos de datos primitivos | |
------- | -------
byte | Números enteros entre -128 y 127
short | Números enteros entre -32768, 32767
int | Números enteros entre -2147483648 y 2147483647
long | Enteros muy grandes, entre -9223372036854775808 y 9223372036854775807
float | Número con coma -3.402823e38 a 3.402823e38
double | Número con coma, mayor capacidad -1.79769313486232e308 a -1.79769313486232e308
string | Cadena de caracteres 
char | Un carácter (Ej: ‘a’) Unicode
boolean | Verdadero o falso (true /false)


## Estructura de control en Java <a id='c1e'></a>

Las estructuras de control en Java tienen la misma sintaxis que en JavaScript. Contamos con:

Decisión if - switch
Repetición while - for

A continuación recordemos brevemente cómo es su sintaxis.


### Estructura de decision:

```java
if (condición){
//código que se corre si la condición es verdadera
} else if(condición){
//código que se corre si la primera condición no fue verdadera y la segunda sí es verdadera
}else {
// código que se corre si ninguna condición anterior fue verdadera
}
```

```java
switch (variable){
case valor1:
//código que se ejecuta si la variable tiene valor1
break;
case valor2:
//código que se ejecuta si la variable
tiene valor2
break;
.
.
default:
//código que se ejecuta si la variable tiene algún valor no enumerado
}
```

### Estructuras de repetición:

```java
for(Integer i = 0; i < valorMaximo; i++){
//código que se ejecuta cada vez
}
```

```java
for(Object object : listaDeObjetos){
//código que se va a ejecutar por cada objeto en la lista
}
```

```java
while(condición){
//hacer este código
}
```

> Ver video: Ciclo for
>
> Ver PDF: Ejercitacion estructuras.pdf 

### Ejercitacion estructuras <a id='c1act'></a>

Ejercitación Estructuras

Ejercicio 1
Definir dos números enteros. Asignarles un valor a cada uno. Comprobar si un número es
divisible por el segundo e indicar mediante un mensaje el resultado obtenido.
NOTA: Que sea divisible quiere decir que al dividir da un valor exacto, es decir, sin
decimales.

```java
package Sincro;

public class C1ejercitacionEstructuras {
    public static void main(String[] args) {
        int num1 = 10;
        int num2 = 5;

        if (num1%num2 == 0){
            System.out.println("El numero "+num1+" es divisible por "+num2);
        } else {
            System.out.println("Los numeros no son divisibles");
        }
    }
}

// Muestra en consola: El numero 10 es divisible por 5
```

> Ver PDF: Definiendo mascotas / Ejercitacion tipo variables.pdf <a id='c1s'></a>




