# NF1 ARQUITECTURA DE SISTEMAS

## Modelo Lógico o arquitectura Von Neumann

La arquitectura de Von Neumann se refiere a la manera de agrupar los elementos de un sistema:

- Memoria
- Procesador
- Unidad de entrada/salida
- Conexión entre elementos

![image](https://github.com/user-attachments/assets/7c518591-440a-4714-9df7-9d863f5471ae)

Los datos que entran se procesan en base a una serie de reglas que residen en la memoria.

- Los datos entran a través de la unidad de Entrada/Salida
- El procesador evalúa y procesa según las reglas.
- El conjunto de dichas reglas están almacenadas en la memoria.
- Los datos pasan vía un bus de conexión.

Las instrucciones que seguirá el procesador:

- Aritméticas
- Lógicas
- Transferencia
- Salto

### Procesador

El procesador dispone de un ALU (Unidad Aritmética y lógica) para poder realizar operaciones aritméticas y lógicas.

### Unidad de control

Encargada de interpretar instrucciones que lea del programa residente en la memoria.

### Memoria y sistema E/S

Residen las instrucciones que el procesador debe seguir y donde se guardan los datos adquiridos de la unidad/es E/S

### Bus de datos

Sistema por el cual se comunican todos los dispositivos anteriores

![image](https://github.com/user-attachments/assets/de611896-2ecf-4064-84d2-b6ce05bd95df)

## Estructura de un Ordenador

### CPU

Constituye el núcleo central del ordenador, encargada en que funcionen los demás componentes.

### Almacenamiento

Su elemento prinicipal es el "biestable" permitiendo adoptar dos estados (0 y 1). 

Un biestable es la parte más atómica de una memoria. 

Su funcionamiento se llamada síncrona.

### Operacion

En función del procesamiento tenemos operadores en paralelo, (procesan la información de una sola vez).

Operadores en serie (trabajan con un bit de cada operando cada vez).

### Interconexión

Se realiza con buses de conexión, podemos encontrar:

- De datos
- De direcciones
- De control

### Unidad central de proceso (CPU)

Dispone de una serie de registros:

- Registros RI : Almacenan la instrucción que se está ejecutando
- Registros CP : Almacenan la dirección de memoria de la siguiente instrucción.
- Registros generales  : Almacenan datos para acceder inmediatamente.

## La memoria

Dividida en celdas que almacenan valores binarios llamados bits. Conforman instrucciones de los programas que van a ser ejecutados.

- Ancho de banda : Tamaño que se puede leer o escribir simultáneamente
- Direcciones de memoria: Identifican cada palabra en la memoria

### Memoria RAM

Memoria volátil, se puede modificar, cambiar, reescribir y leer.

### Memoria ROM

Solo se puede leer y no está sujeta a modificaciones ni reescrituras. Almacena información aún que no exista corriente.

### Memoria Cache

Utilizada en los módulos de la memoria principal. Dividida en subniveles:

- L1 y L2
- L3

### Memoria Principal

### Memoria virtual o memoria swap

Se dedica a suplir a la memoria principal cuando esta se agota.

### El subsistema de E/S

- Polling: Unidad centrada de procesos, encarga en transferir los datos
- Interrupciones: Responsable de la transferencia de datos igual que la anterior, pero esta vel el periferico es el que pregunta.
- DMA: Realiza el trabajo de transferencia de información.

## Tipos de arquitectura de BUS

- Bus de datos: Transfiere la información de un lugar a otro
- Bus de direcciones: Transfiere la posición de la memoria que será utilizada en ese momento
- Bus de control: Transfiere la operación a realizar

## Función de los dispositivos

- Dispositivos de entrada
- Dispositivos de salida
- Dispositivos de almacenamiento

## Factor de Forma

Referencia a dimensiones, forma y especificaciones físicas del hardware.

## Componentes físicos de los sistemas informáticos

- Chasis, alimentación y refrigeración. 

## Placa base

- R
