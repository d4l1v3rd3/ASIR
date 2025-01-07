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

- Reloj: Regusta y gestiona la velocidad en ejecución
- Memoria CMOS: Almacena información de estado imporante para el equipo
- Conectores de tensión: Repartir la energía
- BIOS: Software grabado en memoria no volátil
- Buses de interconexión:
- Conectores de E/S
- Bahías
- Socket de CPU
- Ranuras memoria
- Chipset

ATX o AT dependiendo del factor de forma

## Procesadores y memorias

- DRAM: Gran capacidad de almacenamiento, necesita refrescarse con cada ciclo de reloj.
- SRAM: Menos capacidad que la DRAM pero más rpápida.
- SDRAM: Tiene las ventajas de las dos anteriores.
- DDRAM: Se actualiza un par de veces por cada ciclo de reloj. Doble de rápida.


Tarjeta gráfica : VRAM (Memoria RAM interna de la tarjeta gráfica) posterior SGDRAM


## Dipositivos de Almacenamiento

- PATA
- SATA
- SCSI
- HDD
- SSD

# Preguntas Ejercicio

## Indica cual es una de las funciones del registro de condición de la CPU:

```
Guardan códigos de condición, generados como resultado de determinadas operaciones
```

## La placa base de nuestro pc es:

```
Un elemento donde coexisten elementos electrónicos como condensadores, resistencias, etc. y permite que la corriente de la fuente de alimentación se reparta de manera correcta entre los elementos que necesitan una determinada tensión para funcionar
```

## El bus de dirección tiene entre otras funciones la de:

```
Transmite direcciones entre CPU y memoria
```

## Indica cual es una de las funciones del registro de dirección de la CPU

```
Contienen las direcciones de memoria  donde se encuentran los datos
```

## Qué es el Overclocking

```
Consiste en forzar los componentes del equipo para que trabajen a una velocidad más rápida que la fijada por fábrica con el objetivo de mejorar el rendimiento del equipo
```

## Indica cual es la función del registro de datos de la CPU:

```
Guardan los datos con los que trabaja la CPU
```

## La alternativa a la BIOS que esta escrita en C y es más actual se conoce como

```
UEFI
```

## El bus de datos tiene entre otras la función de

```
Intercambia datos entre la CPU y las unidades
```

## Cuando hablamos de la memoria propia de la tarjeta gráfica y que es independiente de la memoria propia del ordenador esta memoria es conocida como

```
Memoria VRAM
```

## El bus de control tiene entre otra la función de

```
Controla los elementos de la CPU
```


