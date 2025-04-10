# Arquitectura de sistemas

Aprendes componentes internos de un equipo informático.

## Configuración de equipos y periféricos. Arquitectura de ordenadores

### Modelo lógico o arquitectura Von Neumann

Agrupa estos elementos:

- Memoria
- Procesador
- Unidad de entrada/salida
- COnexión entre elementos

![image](https://github.com/user-attachments/assets/5a3be8e1-b6aa-4c96-a529-4ec0052aa853)

Los datos de esta arquitectura que entran se procesan en base a una serie de reglas que residen en la memoria.

- Los datos se adquieren o entran a través de la unidad de E/S
- El procesador se encarga de evaluarlos y procesarlos según unas reglas
- El Conjunto de las reglas que utiliza el procesador par evaluar los datos se alamacenan en la memoria en forma de programa.
- Los datos pasan de un bloque a otro mediante bus de conexión

Instrucciones queda:

- Aritmeticas
- Logicas
- Transferencia
- Salto

La arquitectura de Von Neumann tendrá un programa diferente por
cada planteamiento al que le tenga que dar solución, haciendo así
que el sistema basado en esta arquitectura sea lo suficientemente
flexible para solucionar diferentes tipos de problema

En la memoria se almacenarán tanto los datos como las instrucciones,
cada uno en su posición de memoria correspondiente para acceder
de forma independiente

Las instrucciones se leen de forma secuencial, primera, segunda, etc.

El procesador a de disponer  de una ALU (Unidad aritmética y lógica) realizando las operaciones aritméticas y lógicas de nivel básico

También esta la unidad de control, encargada de interpretar memoria para generar el conjunto de señales que pasan por ALU, el procesador dispondrá una serie de registros o elementos de almacenamiento de información.

Otros elementos:

- Memoria
SIstema de entrada y salida

Residen instruicciones que el procesador debe seguir.

## Esquema funcional y estructura de un ordenador. Componentes funcionales del sistema informático

![image](https://github.com/user-attachments/assets/63e8cc99-1a75-432f-bad9-a93951a6c02a)

La CPU constituye el núcleo central del ordenador, encargada en el funcionamiento de los demás componentes.

Tipo de funcion que realizan:

- Almacenamiento: Su elemento principal es el biestable o flip-flop, permite adopar dos estados (0 o 1) (síncrona)
- Operación: operadores en paralelo o operadores en serie, dependiendo el número pueden ser monadicos o didadicos
- Interconexión: Realizada en bus de conexión, como calles transportan elementos, datos, dirección, control..
- Unidad Centra del proceso: CPU encragada del control, administración y ejecución de instrucciones

- Registros RI: Alamacenan instrucciones
- Registros CP: ALmacenan direccion de memoria
- Registros generales: ALmacenan datos al os que la ALu accede de forma inmediata

- MEmoria: Dividida en valores binarios llamados bits.



