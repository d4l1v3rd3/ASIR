# Introducción a las bases de datos

- Base de datos: Colección organizada de datos que se pueden acceder, gestionar y actualizar de manera eficiente.

- La mayoría de las bases de datos modernas son sistemas de bases de datos relacionales, almacenan los datos en tablas relacionales que se conectan entre sí a través de calves primarias y claves foráneas.

- Las bases dedatos permiten al realización de consultas y búsquedas de datos, facilitando la obtención de información.

Pueden existir varios tipos de bases de datos:

- Bases de datos centralizadas.
- Bases de datos distribuidas.
- Bases de datos orientadas a objetos
- Bases de datos NoSQL

En las bases de datos las utilizamos como grandes contenedores donde se guarda información, como textos, imágenes y vídeos.

Es fundamental tener en cuenta la integridad de los datos, asegurandonos que son precisos y coherentes. Mendiante restricciones y validaciones de datos, a través de implementaciones y procedimientos de seguridad y recuperación.

## Ficheros (Planos, indexados, acceso directo, entre otros)

Los ficheros son grupos de registros de infromación que comparten una temática común, organizados.

Clases:

- Ficheros planos: Almacenan información en formato ASCII (texto plano), utilizan un carácter especial para separarlos, el acceso es de forma secuencial accediendo al programa uno a uno.
- Ficheros indexados: Permiten organizar y acceder a la información mas rápidamente y eficiente, se le asigna una clave o índice único con una ruta exacta.
- Ficheros relativos: Cada uno tiene una clave asignada relacionada con una ubicación física, dentro de ellos existen los "accesos directos" que almacenan los registros de datos de posiciones específicas en memoria.

## Bases de datos, Conceptos, usos y tipos según el modelo de datos, la ubicación de la información

A los ficheros pueden acceder múltiples usuarios y aplicaciones al mismo tiempo. Para gestionar esto se utilizan "sistemas gestores de bases de datos" (SGBD)

La razón de usar bases de datos es para poder modificar la estructura de datos sin tener que cambiar los programas que utilizan esa información.

Para lograr esto se divide en niveles:

- Nivel físico
- Nivel lógico
- Nivel externo

![image](https://github.com/user-attachments/assets/184d12c0-1e25-4ea1-9c3f-a6d3eb9624c3)

![image](https://github.com/user-attachments/assets/24d6b965-59cd-4dc7-bae5-f947d76d07af)

Las vistas son una representación virtual de una o varias tablas de la BD. Utilizadas por usuarios o aplicaciones como si fuera una tabla real.

Puede haber tantas como el usuario quiera.

Una vista es una consulta predefina que se ejecuta sobre una o varias tablas devolviendo un conjunto de resultados representados en tablas independientes.

![image](https://github.com/user-attachments/assets/66c3413e-267e-41ae-8836-a2135bc76576)

Pasos para crear una consulta SQL:

1- Crear la consulta incluyendo las tablas que deseamos combinar, por ejemplo "clientes y ventas"  y combinarlas.

```
SELECT c.nombre, c.apellido, v.fecha, v.monto
FROM clientes c
INNER JOIN ventas v ON c.id_cliente = v.id_cliente;
```

- INNER JOIN : Combina la tabla clientes y ventas usando la columna "id_cliente" como clave de relación.

2- Una vez tengamos la consulta, podemos crear una vista usando "CREATE VIEW"

```
CREATE VIE vista_clientes_ventas AS
SELECT c.nombre, c.apellido, v.fecha, v.monto
FROM clientes c
INNER JOIN ventas v ON c.id_cliente = v.id_cliente
```

La visa se llama "vista_clientes_ventas" y combina las tablas "clientes y ventas"

3- Una vez creado podemos utilizar otras consultas como si fuera una tabla real. Imaginamos que queremos ver las ventas realizadas por los clientes durante el año 2022

```
SELECT * FROM vista_clientes_ventas
WHERE fecha
BETWEEN '2022-01-01'
AND '2022-12-31';
```

Los modelos de datos son herramientas conceptuales que sirven para describir de forma abstracta la esctrucuta de la base de datos.

### Modelos lógicos basados en objetos

Utilizados para describir datos en el nivel conceptual y externo.

- Modelo entidad-relación: Consiste en la elaboración de un diagrama que representa el modelado de los datos de un sistema información.
- Modelo orientado a objetos: Presenta el paradigma de la programación orientada a objetos, los elementos almacenados adquieren características y propeidades de la vida real.

### Modelos lógicos basados en registros

Utilizados para describir datos en el nivel conceptual y físico, "modelos relacionales, de red y jerárquicos"

### Modelos físicos de datos

Se utilizan para descubrir cómo se almacenan los datos. modelo "unificador y memoria de elemntos" (Funcionan ebajo nivel para representar la manera de como se almacenan)

## Sistemas gestores de base de datos. Funciones, componentes tipos y objetivos

Las principales funciones de los (SGBD), tambíen llamados DBMS (Data Base Management Systems), son definir, construir, manipular y controlar las bases de datos.

![image](https://github.com/user-attachments/assets/e923447f-c1fb-4ec4-a76d-571b0b6b5f87)

Componentes:

- Diccionario de datos: Libro de instrucciones de una BD, guarda la información acerca de como se utilizan los datos, como se crea, define, etc..
- Lenguajes de SGBD: Permiten definir las características de la BD y manipular los datos.
  - Lenguaje de definición de datos (LDD o DDL): Utilizados para diseñadores y administradores para especificar características.
  - Lenguaje de manipulación de datos (LMD o DML): Utilizado por todos los usuarios para consultar y actualizar la información.
 
![image](https://github.com/user-attachments/assets/f2fc48e9-e2e4-451d-b586-9c32b8a07ce9)

Dentro del LMD existe los LMD procedimentales, en el que el usuaio debe especificar los datos que queire y cómo acceder a ellos, los LMD no procedimentales, son los que el usuario indica directamente lo datos que necesita sin especificar como obtenerlos.

Ejemplo de DDL pra crear una tabla.

```
CREATE TABLE test (a INT NOT NULL
AUTO INCREMENT, PRIMARY KEY (a), KEY(b) )
TYPE=MyISAM SELECT b,c FROM test2;
```

Consulta para obtener un dato concreto:

```
SELECT persona FROM empresa WHERE sueldo>1000;
```

- Mecanismos: Garantizas la seguridad e integrada de los datos controlando que solo usuarios autorizados puedan entrar.
- Administración: Maximo nivel de privilegios.

## Tipos de usuarios y de lenguajes de bases de datos.



