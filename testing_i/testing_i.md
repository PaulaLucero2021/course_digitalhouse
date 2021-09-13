---
title: "Testing I"
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

<t>Testing I</t>

---

## Índice

1. Fundamentos de testing y gestión de defectos.
- [C1 - Primeros pasos](#c1)
    - [Bienvenida](#c1a)
    - [Introduccion al testing](#c1b)
    - [Cronologia](#c1z)
    - [Principios del testing](#c1y)
    - [El rol del Tester](#c1c)
    - [Ventajas y desventajas prueba independiente](#c1x)
    - [Equipo - Mesa 3 patas](#c1w)

2. Gestion de defectos
3. Disenio de pruebas
4. implementación de la prueba
5. Analisis de la prueba
6. Planificacion de la prueba
7. Introduccion a TDD 
8. Be testing
9. Introduccion a automation
10. Full stack y DevOps tester


# C1 - Primeros pasos <a id='c1'></a>

## Bienvenida<a id='c1a'></a>

Les queremos dar la bienvenida a este camino que empezamos juntos en el mundo de la calidad del software. Durante la materia de Testing I aprenderemos nuevos conceptos de testing, incorporaremos diferentes metodologías de trabajo y las aplicaremos para resolver diversos problemas que se presentan en el día a día de un tester. No solamente abarcaremos contenido teórico, sino también práctico, para así reforzar los conocimientos.

La idea es aprender juntos y acompañarlos en este proceso de aprendizaje y hacerlo de la manera más interactiva posible. ¿Estamos listos para comenzar?

[Modulos Testing I](https://view.genial.ly/60af8755c081a90d9f95a95e)

## Introduccion al testing <a id='c1b'></a>

> Ver video: Que es el testing

<!-- resumen video -->

se parte de la suposicion que el programa contiene errores
calidad es la satisfaccion del cliente
se toman decisiones a traves de las pruebas
confiabilidad, 
pruebas frecuentes 

factores externos:

- requerimientos poco claros
- mofidicaciones a ultimo momento
- errores de diseno y testers no calificados

Testing sirve para:

- Sirve para encontrar el mayor numero de defectos y remediarlos
- Asegurar que el producto funcione como esta definido en los requisitos
- Proporcionar al producto final un mayor grado de calidad.

<!-- fin resumen video -->

## Cronologia <a id='c1z'></a>

[Evolucion historica](https://view.genial.ly/60ae4430920d0f0dae99949f)

![Evolucion](./img/c1.1.png)

<!-- inicio resumen link -->

### 1950-1960

Después de la Segunda Guerra Mundial, los importantes avances en el desarrollo de software tuvieron lugar en EE. UU. y se generaron en el ámbito de la industria militar. En aquella etapa de la evolución del software, las aplicaciones eran desarrolladas para un hardware dedicado, sistemas que contaban al software como una de sus partes. <r>La calidad asociada a estos sistemas se lograba con pruebas exhaustivas una vez terminado de construir.</r>

### 1960 - 1980

Con los avances en el hardware y la aparición de lenguajes de alto nivel, se estableció una nueva tendencia en el desarrollo: se comenzaron a producir sistemas no militares e independientes del hardware. Los avances estuvieron orientados a producir sistemas de propósito general. 

A partir de los inconvenientes de sobrepresupuesto y tiempo adicional necesarios en la terminación del proyecto de desarrollo del sistema operativo de IBM, <r>se generó una alerta en el sentido de la necesidad de contar con métodos de desarrollo que garantizaran la calidad de los productos de software.</r>

### 1980 - 1990

Esta alerta generó el convencimiento de la necesidad y los primeros esfuerzos en la creación de una nueva disciplina llamada ingeniería de software. 

Mientras esto sucedía, la tecnología seguía avanzando y se contaba con plataformas de bajo volumen y costo que ofrecían la posibilidad de desarrollar software como una oportunidad de negocio a gran escala. 

Luego de su paso por Japón, vuelve a EE.UU. <r>W. Demming e introduce el siguiente concepto “la calidad de un producto está directamente relacionada al proceso utilizado para crearlo”</r>, de esta manera, las empresas estadounidenses comienzan a adoptar la estrategia conocida como Gestión de la calidad total.

### 1990 - 2000

En la década de 1990, el crecimiento de los sistemas se acentuó, con protagonistas como Microsoft —ya convertida en líder mundial— Netscape y Oracle, entre otros. Además, <r>se consolidaron las metodologías de desarrollo de tipo iterativas, las cuales van suplantando a las conocidas como cascada.</r> <r>Aparecieron algunas metodologías llamadas ágiles y el concepto de integración continua y también se sigue trabajando en IVV (Independent Verification Validation)</r>. Estas formas de trabajo tienen una fuerte influencia en la calidad del software.

### 2000 - 2010

El escenario establecido para el desarrollo de software está determinado por <r>un hardware cada vez más poderoso, software de última generación, modelos de desarrollo y metodologías ágiles. </r>

Esta velocidad creciente impuesta por el mercado de productos de software tiene un impacto importantísimo en la calidad de los productos y servicios ofrecidos. Es de notar que estos cambios en la evolución de esta industria hicieron que la preparación de los desarrolladores de hoy día sea muy distinta a la que tenían aquellos programadores de sistemas integrados a un hardware dedicado y con requerimientos estables de los años cincuenta.

### 2010 - actualidad

En esta época <r>se afianza la integración entre la ingeniería del software y la ingeniería de sistemas destacándose el papel de los requisitos no funcionales y, sobre todo, de la seguridad</r>; la <r>importancia de la “ciencia, gestión e ingeniería de los servicios” que requiere un enfoque interdisciplinar —informática, marketing, gestión empresarial, derecho, entre otros</r>— a la hora de abordar el diseño de los servicios; <r>la necesidad de adaptar los métodos de desarrollo de software para trabajar en un “mundo abierto”</r> —teniendo en cuenta la inteligencia ambiental, las aplicaciones conscientes del contexto, y la computación pervasiva)—; los sistemas de sistemas intensivos en software (SISOS) con decenas de millones de líneas de código, decenas de interfaces externas, proveedores “competitivos”, jerarquías complejas, entre otros.

También estamos viendo ya la implantación de la ingeniería del software continua, y su correspondiente tecnología y “filosofía” DevOps, que logran reducir el tiempo entre que se compromete un cambio en el sistema y se implementa en producción; lo que requiere un cambio cultural para aceptar la responsabilidad compartida —entre desarrollo y operación— de entregar software de alta calidad al usuario final.

<!-- fin resumen link -->

## Principios del testing <a id='c1y'></a>

[7 principios del Testing](https://view.genial.ly/609824f9de75770d03eca4dc)

![principios](./img/c1.2.png "principios")

### 1. La prueba muestra la presencia de defectos, no su ausencia

No puede probar que no hay defectos. Reduce la probabilidad de que queden defectos no descubiertos en el software, pero, incluso si no se encuentran, <r>el proceso de prueba no es una demostración de corrección.</r>

### 2. La prueba exhaustiva es imposible

No es posible probar todo —todas las combinaciones de entradas y precondiciones—, excepto en casos triviales. <r>En lugar de intentar realizar pruebas exhaustivas se deberían utilizar el análisis de riesgos</r>, las técnicas de prueba y las prioridades para centrar los esfuerzos de prueba.

### 3. La prueba temprana ahorra tiempo y dinero

Para detectar defectos de forma temprana, las actividades de testing, tanto estáticas como dinámicas, <r>deben iniciarse lo antes posible en el ciclo de vida de desarrollo de software</r> para ayudar a reducir o eliminar cambios costosos.

### 4. Los defectos se agrupan

En general, un pequeño número de módulos contiene la mayoría de los defectos descubiertos durante la prueba previa al lanzamiento o es responsable de la mayoría de los fallos operativos.

### 5. Cuidado con la prueba del pesticida

Si las mismas pruebas se repiten una y otra vez, eventualmente estas pruebas ya no encontrarán ningún defecto nuevo. Para detectarlo, es posible que sea necesario <r>cambiar las pruebas y los datos de prueba existentes.</r>

### 6. La prueba se realiza de manera diferente según el contexto

Por ejemplo, el software de control industrial de seguridad crítica se prueba de forma diferente a una aplicación móvil de comercio electrónico.

### 7. La ausencia de errores es una falacia

El éxito de un sistema no solo depende de encontrar errores y corregirlos hasta que desaparezcan ya que puede no haber errores, pero sí otros problemas. Existen otras variables a tener en cuenta al momento de medir el éxito.

## El rol del Tester <a id='c1c'></a>

> Ver pdf: Aspecto psicologico del testing.pdf

<!-- Resumen pdf -->

> El testing es el proceso de ejecución de un programa con la intención de encontrar errores.

## Aspecto psicológico del testing 

Los seres humanos tienden a ser sumamente orientados a objetivos y el establecimiento de la meta adecuada tiene un efecto psicológico importante. Si nuestro objetivo es demostrar que un programa no tiene errores, entonces, subconscientemente estaremos dirigidos a esa meta, es decir, tendemos a seleccionar los datos de prueba que tienen una baja probabilidad de causar que el programa falle. Por otro lado, <r>si nuestro objetivo es demostrar que un programa tiene errores, nuestros datos de prueba tendrán una mayor probabilidad de encontrarlos.</r>

Más allá del desarrollador o el tester, las tareas de prueba pueden ser realizadas por personas que desempeñan un rol de prueba específico u otro rol —por ejemplo, clientes—.

## Prueba independiente

La forma en que se implementa la independencia de la prueba varía dependiendo del modelo de ciclo de vida de desarrollo de software. Por ejemplo, en el desarrollo ágil, los probadores pueden formar parte de un equipo de desarrollo. En algunas organizaciones que utilizan métodos ágiles, estos probadores también pueden ser considerados parte de un equipo de prueba independiente más grande. Además, en dichas organizaciones, los propietarios de producto pueden realizar la prueba de aceptación para validar las historias de usuario al final de cada iteración.

## Ventajas y desventajas de la prueba independiente <a id='c1x'></a>

|Beneficios potenciales de la independencia de la prueba|Desventajas de la independencia de la prueba|
|----------------------------------|---------------------------|
|Es probable que los probadores independientes reconozcan diferentes tipos de fallos en comparación con los desarrolladores debido a sus diferentes contextos, perspectivas técnicas y sesgos. |Los desarrolladores pueden perder el sentido de la responsabilidad con respecto a la calidad|
|Un probador independiente puede verificar, cuestionar o refutar las suposiciones hechas por los implicados durante la especificación e implementación del sistema|Los probadores independientes pueden ser vistos como un cuello de botella o ser culpados por los retrasos en el lanzamiento o liberación|
| |Los probadores independientes pueden carecer de información importante —por ejemplo, sobre el objeto de prueba—.|

<!-- fin resumen pdf -->

## Equipo / Mesa de 3 patas <a id='c1w'></a>

[Equipo](https://view.genial.ly/609fb88d81ac730cff0404aa)

- Si bien cada actor tiene un rol definido, es necesario un trabajo en comunión entre los 3 actores. Es decir, es necesario que trabajen como equipo. Por eso, utilizamos la analogía con una mesa de 3 patas, pues si falta alguna de ellas, la mesa no podría estar de pie.
- En algunas empresas de software pequeñas o “start up” es posible que una misma persona tenga más de un rol.
- Además, algo importante dentro de las metodologías de desarrollo ágiles, es la reunión de los 3 amigos. Es una sesión en la que participan estos tres roles y cada uno de ellos da su punto de vista respecto al software que está bajo desarrollo. Aquí, más que nunca se pone en manifiesto el funcionamiento de la mesa.

![Mesa de 3 patas](./img/c1.3.png)

### Business analyst / Analista de negocio

Se encarga de detectar los factores clave del negocio y es el intermediario entre el departamento de sistemas y el cliente final.

### Software developer / Desarrollador de software

Su función es diseñar, producir, programar o mantener componentes o subconjuntos de software conforme a especificaciones funcionales y técnicas para ser integrados en aplicaciones.

### QA

La principal función es probar los sistemas informáticos para que funcionen correctamente de acuerdo a los requerimientos del cliente, documentar los errores encontrados y desarrollar procedimientos de prueba para hacer un seguimiento de los problemas de los productos de forma más eficaz y eficiente.

<!-- fin resumen link -->

> Ver actividad: 1
