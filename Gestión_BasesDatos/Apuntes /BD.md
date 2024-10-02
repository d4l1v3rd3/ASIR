# ¿Qué es una Base de datos?

Una base de datos es un sistema de almacenamiento de información estructurada y vinculada, que se encarga de ordenar y facilitar la manipulación y consulta de los datos

- Sistema de almacenamiento de información: La información que queremos usar esta guardada en un sitio (Digitalmente)
- Tiene información estructurada: Datos estructurados por grupos
- Vinculada: Relaciones entre datos de un mismo registro, diferentes tablas, etc.
- Ordenar: Permite ordenar los datos dependiendo filtros o criterios
- Manipulación: Nos debe permitir escribir datos, modificar datos o eliminarlos.
- Consulta: Colección de datos que requeramos en cada ocasión

## Características funcionales

- Independiente del software y hardware (sistema operativo o dispositivo)
- Acceso simultáneo de múltiples usuarios (Leídos por mucha gente al mismo tiempo o modificación al mismo tiempo)
- Seguridad de acceso (Los datos deben estar protegidos impidiendo el acceso a usuarios no autorizados)
- Respaldo y recuperación (Copias de seguridad, o importar o exportar datos)
- Acceso a través de lenguajes de programación (acceso simultáneo dando igual el lenguaje)

# Lenguajes

## SQL

Lenguaje de bases de datos utilizado para controlar y manejar la estructura de la BD

Structured Quert Languaje (Lenguaje de consultas estructuradas)

## Sitemas gestores de bases de datos SGBD

Software de servidor de datos que permite administrar los lenguajes

- Motor SQL (Ejecución de comandos)
- Índice (estrucutración)
- Integridad referencial
- Seguridad
- Acciones programadas

Todos los SGBD utilizan la misma sintaxis de SQL:

- MySQL
- Microsoft SQL Server
- Oracle Database
- MongoDB
- SQLite
- PostgreSQL
- MariaDB

## Clientes de BD

Programas que disponen de GUI, facilitando la comunicación con los SGBD (A sí no tenemos que utilizar todos los comandos de SQL)

- PHPmyADMIN
- Workbench
- Microsoft Acess
- dBase
- FileMaker

# Sublenguajes de SQL

Divididos en encargarse todas las funciones del lenguaje SQL

Eng | Esp | Explicación | Comandos
--- | --- | --- | ---
DDL (Data definition Language) | LDD (Lenguaje de definición de datos) | Definición y modificación de la estructura de los elementos | CREATE, RENAME, DROP, ALTER
DML (Data Manipulation Language) | LMD (Lenguaje de manipulación de datos) | Consulta y modificación de los datos | INSERT, UPDATE, DELETE, SELECT
DCL (Data Control Language) | LCD (Lenguaje de control de datos) | Controlar permisos de acceso a los datos | GRANT, REVOKE


# Componentes SQL

- Tablas: Colecciones de datos que estan esctructuras en filas y columnas. (Denominadas Campos) Indicando el tipo de dato que contine.
- Registro: Conjunto de datos asociativos, enlazados entre sí (No pudiendose intercambiar con otros)
- Entidad de datos: Cada tabla almacena esto mismo si hay muchas

# Operaciones básicas SQL

BBDD | Tablas | Campos | Registros | DESCRIPCIÓN
--- | --- | ---| --- | --- |
CREATE DATABASE | CREATE TABLE | ALTER TABLE ADD | INSERT | CREAR
... | RENAME TABLE | ALTER TABLE CHANGE | UPDATE | MODIFICAR
DROP DATABASE | DROP TABLE | ALTER TABLE DROP | DELETE | BORRAR
... | ... | ... | SELECT | CONSULTAR
