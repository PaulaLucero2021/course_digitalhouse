---
title: "Infraestructura I"
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

<t>Infraestructura I</t>

## Índice <a id='up'></a>

1. Inmersion
- [C1 - Introducción a la materia & the big picture](#c1)
    - [Bienvenida](#c1a)
    - [Introducción a la materia](#c1b)
    - [El centro de computadoras](#c1c)
    - [The big picture](#c1d)

2. Automatizacion
- [C2 - Automatizacion](#c2)
    - [Automatizacion de la intraestructura](#c2a)
        - [5 Tareas mas comunes de automatizar](#c2a1)
        - [Configuracion y mantenimiento del sistema](#c2a2)
        - [Infraestructura y servicios](#c2a3)
        - [Manejo del codigo](#c2a4)
        - [Contenedores](#c2a5)
        - [Ambientes de trabajo](#c2a6)
        - [Monitores de red](#c2a7)
        - [Lenguajes de scripting](#c2a8)
    - [Virtualizacion](#c2b)
        - [Historia virtualizacion](#c2b1)
        - [Componentes virtualizacion](#c2b2)

3. Containers
4. Cloud computing
5. Cierre


# C1 - Introducción a la materia & the big picture <a id='c1'></a>

[Modulos infraestructura](https://view.genial.ly/61263a284987a50dae61ca14) <a id='c1a'></a>

***

## Introducción a la materia <a id='c1b'></a>

En la actualidad, la actividad cotidiana depende en un porcentaje elevado del correcto funcionamiento de los sistemas informáticos —y saber operar con dichos sistemas—. La dependencia del ámbito productivo con los complicados sistemas informáticos es tal, que un problema en una terminal de trabajo deja prácticamente sin efecto la capacidad operativa de cualquier usuario. Ante situaciones de esta naturaleza —considerando la complejidad de las actuales plataformas tecnológicas y la multiplicidad de usuarios con diversos niveles de acceso y experticia—, se hace necesaria la presencia de un profesional confiable que intervenga, rápida y eficazmente, con habilidades y destrezas mayores a las del operador habitual.

La función de este profesional —conocido como administrador de infraestructura— es brindar respuestas a los problemas habituales de hardware y software en cualquier ámbito informatizado, planteándose desde una problemática y evaluando su mejor solución. Este servicio debe estar en manos de profesionales que orienten, configuren, prevengan y resuelvan eventualidades, manteniendo sus equipos en un estado óptimo. Además, el administrador de infraestructura debe ser capaz de prestar servicios de administración y soporte de sistemas de base y elementos de infraestructura para el procesamiento de aplicaciones informáticas, tales como servidores, dispositivos de almacenamiento masivo, otros dispositivos de hardware, sistemas operativos, máquinas virtuales y administradores de redes, servicios de comunicaciones a través de redes públicas y privadas, dispositivos de switching, firewalls, motores de bases de datos, entre otros. Podrá además brindar servicios de administración de la infraestructura tecnológica en la cual opera el software de estas aplicaciones interviniendo en forma puntual para resolver los problemas que experimente esa infraestructura o su eficiencia operativa y realizar un diagnóstico de incidentes que se presenten en la operatoria habitual del sistema.

La intención es contribuir con soluciones concretas a la problemática del soporte de infraestructura IT que se presentan en la casi totalidad de las instituciones públicas y/o privadas, acelerando los tiempos en materia de formación de recursos humanos capacitados y demandados por todas aquellas organizaciones que cuentan con una infraestructura IT.


## ¿Qué es infraestructura de IT?

La infraestructura de tecnología de la información, o infraestructura de IT, se refiere a los componentes combinados necesarios para el funcionamiento y la gestión de los servicios de IT de la empresa y los entornos de IT.


## ¿Quién hace infraestructura?

Estudiar una carrera profesional no consiste solamente en los años que le vas a dedicar a terminar tus estudios. Después de obtener tu título te espera un largo camino de crecimiento profesional y, si bien muchas veces tenemos una idea de las opciones profesionales que existen, a veces tenemos nociones erradas o no hemos explorado correctamente todas las posibilidades que hay disponibles. Por eso, a lo largo de la carrera te compartiremos las opciones en el campo laboral que tienen todos aquellos que decidan ser profesionales de sistemas.

Es evidente que estamos en una era en la que casi cualquier tipo de tarea es mediada por un computador. Por eso, el conocimiento de un profesional de sistemas es necesario en sectores tan diversos como, por ejemplo, el entretenimiento o el mundo empresarial. A través de esta materia adquirirán conocimientos aplicables a las tareas que deben desarrollar en cualquier sector de IT.

## ¿Cuál es el perfil de un analista de infraestructura?

Las funciones que ejerce un analista de infraestructura, entre otras, son:

- Administrar servidores, software de base, comunicaciones y demás subsistemas, maximizando el aprovechamiento de los recursos y anticipando posibles eventualidades.
- Administrar redes de comunicación de datos (cableadas o no), asegurando la accesibilidad de los servicios y optimizando los recursos.
- Atender incidentes que afecten al soporte de infraestructura de IT, diagnosticar las causas que los originan y resolverlos o coordinar su solución.
- Instalar o reemplazar componentes de soporte de infraestructura de IT o adaptarla a nuevas condiciones de servicios externos minimizando riesgos para la seguridad y continuidad del servicio.
- Migrar o convertir sistemas, aplicaciones o datos tratando de minimizar riesgos para la seguridad y continuidad del servicio.
- Entender temas de contingencias y riesgos que puedan afectar al soporte de infraestructura de IT.
- Generar propuestas innovadoras y/o emprendimientos productivos propios del ámbito de la gestión de soporte de infraestructura de IT.

Esta persona se desempeña en centros de procesamiento de datos, ya sean de empresas u organizaciones de cualquier tipo usuarias de tecnología de la información. Su posición ocupacional suele denominarse administrador de red o administrador de sistemas, y trabaja solo o en pequeños grupos para administrar los recursos de infraestructura de tecnología de la información y atender y resolver incidentes, a fin de minimizar la posibilidad de interrupciones al servicio que brindan las aplicaciones informáticas a las organizaciones.

Por lo general, depende directa o indirectamente de un gerente de tecnología responsable por toda la operación y —en función de la dimensión de la organización en la cual se desempeñe— puede trabajar solo, en pequeños grupos o en grupos más grandes que permitan su especialización en determinadas tecnologías. En la mayoría de los casos, no tiene personal a cargo, aunque puede coordinar las actividades de pequeños grupos operativos. En algunos casos en que la infraestructura es muy pequeña puede brindarle sus servicios profesionales externamente atendiendo a los centros de procesamiento en forma presencial o a distancia.

## ¿Por qué es tan importante la infraestructura de IT?

La tecnología es el motor de prácticamente todos los aspectos de las empresas actuales. Desde el trabajo de un empleado individual hasta las operaciones de bienes y servicios. Si se conecta correctamente, la tecnología se puede optimizar para mejorar la comunicación, crear eficiencia y aumentar la productividad.

Si una infraestructura de IT es flexible, fiable y segura, puede ayudar a una empresa a cumplir sus objetivos y a ofrecer una ventaja competitiva en el mercado. De forma alternativa, si una infraestructura de IT no se implementa correctamente, las empresas pueden afrontar problemas de conectividad, productividad y seguridad, como infracciones e interrupciones del sistema. En general, contar con una infraestructura correctamente implementada puede ser un factor clave para la rentabilidad de un negocio.

Con una infraestructura de IT, una empresa puede:

- Ofrecer una experiencia del cliente positiva proporcionando acceso ininterrumpido a su sitio web y la tienda en línea.
- Desarrollar y lanzar soluciones al mercado con rapidez.
- Recopilar datos en tiempo real para tomar decisiones rápidas.
- Mejorar la productividad de los empleados.

***

## Arquitectura cliente-servidor <a id='c1c'></a>

La arquitectura cliente-servidor persigue el objetivo de procesar la información de un modo distribuido. De esta forma, pueden estar dispersos en distintos lugares y acceder a recursos compartidos.

Además de la transparencia y la independencia del hardware y del software, una implementación cliente-servidor debe tener las siguientes características:

- Utilizar protocolos *asimétricos*, donde el servidor se limita a escuchar en espera de que un cliente inicie una solicitud.
- El acceso es transparente, multiplataforma y multiarquitectura.
- Se facilitará la *escalabilidad*, de manera que sea fácil añadir nuevos clientes a la infraestructura —escalabilidad horizontal— o aumentar la potencia del servidor o servidores, aumentando su número o su capacidad de cálculo —escalabilidad vertical—.

Ahora veamos las características de los tres componentes de la arquitectura cliente-servidor.

[Arquitectura cliente-servidor](https://view.genial.ly/609fd90a72150f0d1205fa78)

> Ver video: La importancia del centro de datos

<!-- Resumen video -->

dentro de los middleware estan:

## DBMS

Sistema de administracion de base de datos que permiten:

- crear
- Recuperar
- Actualizar 
- Administrar datos

## APIs

Interfaz de programacion de aplicaciones que brindan un conjunto de subrutinas funciones y procedimientos para ser utilizados en otro software

## Sistema operativo

El motor que va a aprovechar los recursos de la infraestructura, 
conjunto de programas capaz de administrar los recursos fisicos del servidor
asi como los protocolos de ejecucion de otro software


<!-- fin resumen --> 

[Caracteristicas fundamentales de un sistema operativo](https://view.genial.ly/60a81847f631260d39c063ca)

### Soporte de red

Es indispensable que tengan un soporte completo para poder brindar conectividad.

### Amplia compatibilidad con el hardware

Un punto fundamental para el aprovechamiento pleno de las características del servidor es que el S.O. <r>sea capaz de exprimir al máximo las características técnicas del hardware</r> en donde se ejecuta, es por ello que <r>se debe priorizar el uso de S.O. actualizados y con un soporte importante de controladores</r>. 
Por ejemplo, que nuestros controladores permitan acceder a características avanzadas de gestión de discos rígidos, con el propósito de realizar arreglos redundantes para tener mayor velocidad y tolerancia a fallos.

### Seguridad 

Teniendo en cuenta el rol que cumple el servidor, es de vital importancia que <r>el S.O. instalado sea seguro</r>; eso implica <r>no solo que este actualizado con todos los parches/actualizaciones, sino que además debe tener aplicadas políticas estrictas de acceso</r> para prevenir accesos no autorizados o ataques. 

Adicionalmente esa seguridad <r>debe reforzarse con la instalación de Firewalls (por software o hardware) y antivirus</r>. 

En este ítem también debemos incluir <r>el respaldo de la información</r>, ya sea por medio de herramientas que el propio S.O. nos ofrezca o instalando software externo, con el propósito de tener la menor pérdida de datos posible en caso de fallos fatales.

### Dispositivos físicos de protección

Debemos priorizar S.O. que en su arquitectura <r>permita una tolerancia a fallos</r>, ya sea mediante la generación de granja de servidores, que interconectados, operen como una gran unidad de proceso, dando la posibilidad <r>que ante la caída de uno de los integrantes de la granja, otro puede tomar su rol y responsabilidad</r>.

<!-- fin link -->

Conocidas estas características casi innegociables a la hora de elegir un S.O. para servidores, es común preguntarnos por qué se utilizan sistemas operativos y versiones específicas para el entorno de servidores y no usamos los mismos S.O. que tenemos instalados habitualmente en nuestras computadoras o estaciones de trabajo; eso se basa en algunas diferencias, a destacar:

### Manejo diferente del hardware:
Debido al diferente propósito, <r>los S.O. de estaciones de trabajo no pueden aprovechar todo el hardware disponible</r>, como, por ejemplo, el manejo de memoria RAM —teniendo el caso de Windows 10 64-bit que puede manejar 6TB de RAM, mientras que Windows Server 2019 alcanza los 24TB—.

### Características soportadas:
Hay funcionalidades que nativamente un S.O. de estación de trabajo no es capaz de brindar, ya que en su versión de kernel están limitadas o deshabilitadas —casos tales como la virtualización en algunas versiones de Windows 10—.

### Soporte:
Algo muy importante a tener en cuenta es, cuando nuestro negocio o aplicación depende de un S.O., es el <r>soporte por parte del fabricante/desarrollador</r>. En el caso de los S.O. de estación de trabajo, el soporte/cobertura que tenemos es para un uso específico, <r>si sobre esa base quisiéramos desplegar una arquitectura, por ejemplo, de servidor web, si bien es probable que nos funcione, vamos a carecer de soporte técnico</r> ya que el fabricante nos indicará que para ese propósito esta la version “Server” del producto.

Ya entrando en el terreno de las opciones disponibles para un S.O. de servidor, nos vamos a encontrar con dos opciones predominantes en el mercado:

![img unix vs windows](https://assets.digitalhouse.com/content/ar/td/inf/Gr%C3%A1fico_Mesa%20de%20trabajo%201C1A.png)

En el grupo de los UNIX (o UNIX-like) tenemos a:

- GNU Linux
- FreeBSD
- macOsServer

En el grupo de Windows, integrado por toda la familia de Windows Server, tenemos las versiones que van desde la versión 2003 a 2019.

En el transcurso de la cursada nos vamos a centrar en GNU Linux y Windows, ya que son las opciones más utilizadas; iremos conociendo algunas características que ofrecen, como así también sus diferencias.

[juego unir conceptos](https://view.genial.ly/612678272e794b0d1e71472d)

![juego respuesta](./img/c1.1.png)

***

## ¿Querés saber todo lo que vas a aprender en esta materia? <a id='c1d'></a>

Los profesores te van a dar la bienvenida a esta gran aventura. Comenzarán explicándote cómo se compone y funciona un centro de cómputos. De esta manera, te abrimos la ventana al mundo de la infraestructura.

Te vamos a dar una visión teórica sobre el paradigma cliente-servidor y te vamos a llevar de viaje desde la PC de un cliente hacia el data center. Vas a aprender acerca de sistemas operativos en el contexto del data center. A saber la diferencia entre los distintos sistemas operativos que existen en el mercado. Y, como si fuera poco, vas a saber sobre los usos y servicios que se les pueden dar.

Seguiremos con la historia de la virtualización, analizando las capas de servicios con sus funcionalidades y, sobre todo, sabrán de los beneficios de esta tecnología. Te sumergiremos en el mundo de las redes mostrándote el modelo OSI, descubriendo sus protocolos y te llevaremos de viaje con un paquete de una estación de trabajo a otra. Vas a entender el famoso chiste del que hablan los informáticos sobre capa 8. Te mostraremos el mundo de los procesos ITIL: service request management, incident management, problem management y change management; por si llegás a tener que ver algún caso en una herramienta de tickets en tu carrera, vas a saber y poder diferenciarlos.

Además, te introduciremos en el maravilloso mundo de la criptografía. Vas a ver cómo puede ser utilizada para autenticar partes, principalmente, en el contexto de SSH y HTTPS. Aprenderás los comandos básicos para el copiado, borrado y creación de archivos y directorios. También te explicaremos los comandos básicos para la obtención de datos desde un web service y posterior proceso.

Estudiarás qué es el pipeline en la consola y te explicaremos Bash como lenguaje de scripting.

Luego, vamos a pasar por PowerShell, otro lenguaje de automation muy utilizado en las empresas hoy en día. Vas a saber cómo instalar, abrir y ejecutar comandos en una consola y los distintos módulos que existen que te van a ayudar a simplificar muchos futuros scripts.

Para que no te quedes afuera de los lenguajes de scripting, vas a ver también Python, uno de los más reconocidos hoy en día. Te vamos a dar una perspectiva de para qué es y para qué sirve y vas a poder reconocer las aplicaciones —que tanto usás en el día a día— que fueron creadas en ese lenguaje.

Seguimos el camino de esta carrera mostrándote configuration management y Ansible. A esta altura vas a usar el emoji con los anteojitos de sol o los de lectura, el que te guste más.

Continuaremos con una tecnología que nos encanta (y a vos seguro también): Docker. Recorreremos todos los productos de esta simpática ballenita y vamos a ver todos sus usos y mejores prácticas.

Terminaremos este viaje que es Infrastructura I mostrándote todo lo relacionado a cloud computing. Analizaremos los modelos de responsabilidad y vas a poder diferenciar los modelos IaaS, PaaS y SaaS. Conocerás modelos como nube híbrida y serverless. Te mostraremos diferentes nubes: Azure, Google y AWS. Practicarás con AWS Educate y armaremos un pequeño ambiente.

Del otro lado somos un equipo que armamos con mucha pasión todo el contenido de esta materia, con los requerimientos que el programa pide y de lo que nos hubiese gustado aprender a nosotros en el paso que ahora están haciendo. Te agradecemos enormemente tu tiempo y esperamos que nuestro aporte te sea de mucha utilidad en tu carrera. ¿Comenzamos?

![infra](./img/c1.png)

***

![Actividad grupo 7](./img/actividad-grupo-7.png)

# C2 - Automatizacion <a id='c2'></a>

## Automatizacion de la infraestructura <a id='c2a'></a>

Habitualmente resulta cansador realizar las mismas tareas rutinarias en el área de sistemas. ¿Por qué mejor no automatizamos la infraestructura? Es decir, que esa tarea la realice un sistema sin errores y más eficientemente. En esta clase vas a conocer cómo implementar la automatización en infraestructura. 

> Ver PDF: Automatización de la infraestructura..pdf

<!-- inicio resumen pdf -->

**Automatización de la infraestructura**

Como vimos anteriormente, <r>la Infraestructura IT es el conjunto de dispositivos y aplicaciones de software necesarios para que cualquier empresa opere.</r>  Esta se compone de elementos como: 
- software, 
- hardware, 
- redes, 
- instalaciones 
- y todo lo que se requiera para desarrollar, controlar, monitorear y dar soporte a los servicios que ofrece el departamento de IT.
Por otro lado, <r>la automatización consiste en usar la tecnología para realizar tareas casi sin necesidad de las personas.</r> Se puede implementar en cualquier sector en el que se lleven a cabo tareas repetitivas.

La automatización de la IT —también denominada automatización de la infraestructura— <r>**consiste en el uso de sistemas de software para crear instrucciones y procesos repetibles a fin de reemplazar o reducir la interacción humana con los sistemas de IT.**</r>

## ¿Por qué automatizar?

Automatizar tareas permite ganar tiempo y maximizar la productividad de nuestra infraestructura IT. En tiempos de **cloud computing**, este es el mensaje que se repite una y otra vez: <r>cómo hacer más con menos</r>, cómo conseguir que los profesionales IT de nuestra empresa dediquen más tiempo a generar valor para la compañía y menos a tareas repetitivas que se podrían realizar de forma automática.

## Beneficios de automatizar

- Elevar la productividad empresarial.
- Reducir costos operativos.
- Tener una mejor capacidad de respuesta.
- Facilidad de adaptación.
- Disminuir los riesgos de fallas.
- Elevar la seguridad de la información.
- Alojar una mayor cantidad de datos.
- Elevar la competitividad del negocio.

<!-- fin resumen pdf -->

![5 tareas mas comunes en TI para automatizar](./img/c2.jpg) <a id='c2a1'></a>

> Ver PDF: Configuración y Mantenimiento del sistema.pdf

<!-- inicio resumen -->

## Configuración y mantenimiento del sistema <a id='c2a2'></a>

Retomando el concepto que vimos:

>“La automatización de la infraestructura consiste en el uso de sistemas de software para crear instrucciones y procesos repetibles a fin de reemplazar o reducir la interacción humana con los sistemas de TI”.

Este plantea una visión muy amplia, ya que tiene que abarcar los diversos rubros de las empresas que poseen su área de sistema. Según el tipo de organización en la que trabajamos, es el grado de automatización con el que nos vamos a encontrar en la infraestructura de TI.
Uno de los roles del equipo de trabajo del área de sistemas es el **DevOps** engineer, encargado de **automatizar** los procesos del área de **Development** y **Operations**. Su función es hacer más amigable y eficiente la relación entre estos dos equipos de trabajo.

![Servicios](./img/c2a.png)

## Infraestructura y servicios <a id='c2a3'></a>

Primeramente tenemos que analizar los dispositivos que tenemos en nuestra red de IT. Si contamos con servidores **`legacy`** o servicios contratados por un **`cloud providers`**. 
De las dos opciones anteriores, lo que tenemos que tener en cuenta es el sistema operativo con el que trabajan (MAC, Linux, Windows).

De los cloud providers más conocidos contamos con:

- AWS
- Google Cloud
- Microsoft Azure

![c2a1](./img/c2a1.png)

Para la elección se evalúan los costos y la oferta de **servicios que disponen**. Esta última es cada vez más robusta y completa (load balancing, backup, clustering, security, etc.).

## Manejo del código <a id='c2a4'></a>

Partimos desde donde alojamos nuestro código de trabajo si somos programadores. 
Por excelencia el gestor de versionado e integrador de código más utilizado es **Git**. 
Los alojamientos de estos repositorios más conocidos en la nube son GitLab, GitHub, Bitbucket, Gitea, entre otros. 
En estos se almacena nuestro código de las aplicaciones que
pueden estar en lenguajes de programación diversos según lo que necesitemos —por ejemplo: Python, JavaScript, Java, .NET, etc.—.
También podemos automatizar el deploy de nuestro código con CI/CD (refiere a las prácticas combinadas de integración continua y entrega continua). 

Algunas herramientas para hacerlo son:
- Jenkins
- GitActions
- JetBrains

## Contenedores <a id='c2a5'></a>

Los contenedores se están convirtiendo en el modelo de empaquetado de software del producto que desarrollamos. <r>Permiten la virtualización de ambientes de trabajo compatibles transportables, totalmente configurados para que nuestro código funcione en todos los equipos.</r> El más popular es **Docker**.

Cuando manejamos muchos contenedores, tenemos que migrar a un clúster de
contenedores, dirigidos por los orquestadores de contenedores. Por ejemplo:
Kubernetes o Docker Swarm.

## Ambientes de trabajo <a id='c2a6'></a>

Luego, hay que tener en cuenta en qué ambiente está nuestro clúster.

En cada ambiente se trabaja con distintas tecnologías, según el grado de exposición del producto. Automatizando estos procesos vamos a tener más eficiencia, transparencia, facilidad de replicación y recuperación. 

Los ambientes más populares son:

- Ansible
- Chef
- Puppet
- Terraform

## Monitores de red <a id='c2a7'></a>

Es muy importante tener la supervisión de los dispositivos que hay en nuestra red y de los servicios, y programar alertas en caso de que suceda algún cambio. 

Para esto podemos utilizar: 
- Nagios, 
- Prometheus, 
- Icinga2 o 
- DataDog.

## Lenguajes de scripting <a id='c2a8'></a>

Necesitamos trabajar en estrecha colaboración con los desarrolladores y el administrador del sistema para automatizar tareas de los operadores y desarrolladores (como pueden ser
backups, cron jobs, system monitoring).

Según el sistema operativo, podemos usar: 
- Bash o 
- PowerShell.

Pero también existen lenguajes de scripting independientes del SO, como:
- Python, 
- Ruby o
- Go. 
El más popular es `Python`, ya que posee muchas librerías y es de fácil lectura y aprendizaje.

**Conclusión**

Estas tecnologías expuestas para automatizar la infraestructura TI no son todas las que están en el mercado, sino una visión general de las que hoy son las más populares. Hay que tener en cuenta que cada día se están desarrollando nuevas herramientas y metodologías de trabajo para cada empresa, como también empresas que brindan el servicio de automatización outsourcing de la organización. 
<r>Siempre hay que tomar la decisión basándose en la necesidad, recursos disponibles y experiencia que cuenta la empresa.</r>

<!-- fin resumen pdf -->

## Virtualizacion <a id='c2b'></a>

¿Cómo viene todo hasta acá? Ahora vamos a refrescar algunos conocimientos que ya vimos en Introducción a la Informática, principalmente la virtualización, dado que es una de las formas de automatización más utilizadas en la infraestructura IT.

## Introducción a la virtualización

La **virtualización** permite mejorar la agilidad, la flexibilidad y la escalabilidad de la infraestructura de IT, al mismo tiempo que proporciona un importante ahorro de costos.

Algunas **ventajas** de la virtualización son:

- Mayor movilidad de las cargas de trabajo.
- Aumento del rendimiento.
- Menos esfuerzo en los upgrades/updates del sistema.
- Mejor disponibilidad de los recursos o la automatización de las operaciones:
- Simplifican la gestión de la infraestructura de IT.
- Permiten reducir los costos de propiedad y operativos.

A continuación, encontrarás la historia de la virtualización y sus componentes. 

## Historia de la virtualizacion <a id='c2b1'></a>

![cronologia](./img/c2b.jpg)

## Componentes de la virtualizacion <a id='c2b2'></a>

[Componentes](https://view.genial.ly/60a95ee45e2a3d0d271c0bbd)

![c2b2](./img/c2b2.png)

**Maquinas virtuales**

En la actualidad se pueden crear sistemas operativos guest del tipo Microsoft y Linux en casi todas sus versiones, se deben tener en cuenta las versiones de cada sistema operativo y la compatibilidad con el sistema host.

**Administrador de maquinas virtuales**

Desde la herramienta de management se administran todos los recursos físicos y virtuales de los guest que son las instancias virtuales que se crean para usos específicos. Desde el mismo management podremos establecer clustering con otros virtual machines manager para tener alta disponibilidad y tolerancia a fallos. Además, administra todos los recursos virtuales de nuestras virtual machines.

**Sistema operativo base**

Es el sistema operativo encargado de administrar los dispositivos físicos (hardware) y proveer una capa de abstracción a los entornos virtuales. 

**Hardware (Servidores fisicos)**

Los microprocesadores, tanto los de Intel como los de AMD, tienen una característica llamada virtualización de CPU. Se aplica a servidores o máquinas de escritorio. 

> Ver pdf: Instalacion virtual box y vagrant
>
> Ver actividad: crear mv

<!-- actividad sincronica -->
### actividad sincronica
para pasar a root
```bash
su -
```

- **APT** es un proyecto gigante y su plan original incluia una interfaz gráfica. Está basado en una biblioteca que contiene la aplicación central y apt-get fue la primera interfaz — basada en la línea de órdenes — desarrollada dentro del proyecto. apt es un segundo frontend de linea de comandos proporcionado por APT el cual soluciona algunos errores de diseño de la orden apt-get.

- **Su** El programa su permite usar el intérprete de comandos de otro usuario sin necesidad de cerrar la sesión actual. Comúnmente se usa para obtener permisos de root para operaciones administrativas sin tener que salir y reentrar al sistema.

- El servidor HTTP Apache es un servidor web que ofrece muchas y potentes funciones. Entre ellas se incluyen módulos que cargan de forma dinámica, soporte de medios robusto y una amplia integración con otro software popular.

- Me resolto familiar, como un escritorio remoto

<!-- fin actividad sincronica -->




<!-- subir al inicio -->
[subir al indice](#up)