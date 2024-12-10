DDL : Lenguaje de modificación y estructuración de elementos (Crea tablas, campos y base de datos)


```
cd \xampp\mysql\bin
```

dentro abrimos mysql

```
mysql -h localhost -u root -p 
```

La primera veza accedemos sin pass

- Ver bases de datos
```
SHOW databases;
```
- Meternos o usar una base de datos
```
USE test;
```
- Crear tabla
```
CREATE TABLE personas (nombre VARCHAR (50));
```
Caracter var
50 caracteres longitud

- Insertar registros
```
INSERT INTO personas VALUES ("Juan"), ("Andrea"), ("Maria");
```

- Ver datos de una tabla
```
SELECT * FROM personas;
```

```
SELECT nombre FROM profesores;
```


- CREAR BASE DE DATOS CON CODIFICACION

```
CREATE DATABASE empresa
DEFAULT CHARACTER SET UTF8
DEFAULT COLLATE utf8_general_ci;
```

- BORRAR BASE DE DATOS

```
DROP DATABASE nombreBaseDatos;
```

- CREAR TABLAS

```
CREATE TABLE nombreTabla (campo1, campo2, campo3, ...);

CREATE TABLE nombreTabla (deptNum INT (4), dptNombre VARCHAR (50), deptLocalidad VARCHAR (50) );

```

- NOMBRE TABLA

```
RENAME TABLE nombreTabla TO nuevoNombre;
```

- BORRAR TABLA

```
DROP TABLE nombreTabla;
```

- AÑADIR CAMPO

```
ALTER TABLE nombreTabla ADD nombreCampo tipo (longitud);

ALTER TABLE cursos ADD aulta INT(3);
```

- CAMBIAR CAMPO

```
ALTER TABLE nombreTabla CHANGE nombreCampo nuevoCampo tipo (logintud);

ALTER TABLE cursos CHANGE aula clase INT(3);
```

- BORRAR CAMPO

```
ALTER TABLE nombreTabla DROP nombreCampo;

ALTER TABLE cursos DROP clase;
```

 - INSERCION REGISTROS (Orden con el mismo campo que el valor)

```
INSERT INTO nombreTabla (campo1, campo2, ...)
VALUES (valor1, valor2, ...);
```

```
INSERT INTO empleados 
VALUES (22, 'Armando Bronca', 'Seguridad', 4),
	   (15, 'Pere Gil', 'Comercial', 6);
```

- CONSULTAR REGISTROS

```
SELECT campo1, campo2, ...
FROM nombreTabla;
```

- CONSULTAR TODOS LOS REGISTROS

```
SELECT *
FROM nombreTabla;
```

- FILTRAR RESULTADOS

```
SELECT campo1, campo2, ...
FROM nombreTabla
WHERE condición
```

```
SELECT *
FROM departamento
WHERE deptNum = 4 ;
```


```
SELECT profesores.nombre, profesores.apellido, profesores.sueldo
FROM profesores
WHERE (profesores.sueldo >= 1500);  
```

- REEMPLAZAR VALORES

```
UPDATE nombreTabla
SET campo1=valor1, campo2=valor2, ...
where condición;
```

```
UPDATE empleados
SET emplPuest = 'Cajera'
WHERE emplNombre = 'Olga Seosa';
```

- CAMBIAR VALORES NÚMERICOS

```

UPDATE profesores
SET sueldo = sueldo + 100
WHERE sueldo <=1200;
```


- BORRAR REGISTROS

```
DELETE FROM nombreTabla
WHERE condición
```

```
DELETE FROM departamento
WHERE deptNum = 5
```

- LISTAR TABLAS

```
SHOW TABLES;
```

- LISTAR BASES DE DATOS

```
SHOW DATABASES;
```

- DESCRIBIR CAMPOS

```
DESCRIBE campo;
```
