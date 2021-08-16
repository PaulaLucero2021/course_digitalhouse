Existen dos tipos de maquinas virtuales: De sistemas y de  Procesos.

## Maquinas virtuales de sistemas

Emulan una computadora completa
Estas maquinas virtuales las instalamos sobre un `hypervisor`.
Que es una pieza de software que se ejecuta sobre el hardware y administra los recursos de las maquinas virtuales.

Existen 2 tipos de `hypervisor`:

### Los de `Tipo 1`
Donde el `hypervisor` se instala directamente sobre el hardware y controla todos los recursos que este servidor le proporcionara a las maquinas virtuales.

**Ejemplos**

Microsoft Hyper-V
VMware

### En los de `Tipo 2`

El `hypervisor` se instala sobre el Sistema operativo,
es decir, que el Sistema Operativo hace de capa extra entre el hardware y el `hypervisor`.
Aqui, el hypervisor le tiene que solicitar al sistema operativo los recursos que el servidor fisico le a compartir a cada maquina virtual.

**Ejemplos**

- VirtualBox de ORACLE que usamos en clases.

## Maquinas virtuales de procesos o de aplicacion

No emulan la maquina virtual completa, si no un proceso concreto.
Su objetivo es el de proporcionar un entorno de ejecución independiente de la plataforma de hardware y del sistema operativo.

Es util para desarrollar apps para distintos sistemas operativos porque lo puedes hacer desde tu entorno habitual.

**Ejemplos**

- WSL2

permite ejecutar un entorno de trabajo Linux, directamente en windows.

- Maquina virtual de Java

Se crearon diferentes máquinas virtuales java para diferentes arquitecturas, y así, un programa de `java` escrito en Windows puede ser interpretado en un entorno Linux. 
Dandole portabilidad a este lenguaje.

## SIGUE LAURA