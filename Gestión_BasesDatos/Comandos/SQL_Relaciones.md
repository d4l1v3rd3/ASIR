CLAVE PRIMARIA = Clave principal 

CLAVE FORANEA = Clave principal en tabla secundaria

- CREAR PRIMARIA

```
CREATE TABLE nombreTabla (
		nombreCampo tipo (lengt) PRIMARY KEY,
		campo2 ...,
);
```

```
CREATE TABLE nombreTabla (
		nombreCampo tipo (lengt),
		campo2 ...,
		PRIMARY KEY (nombreCampo)
)
```

- AÑADIR PRIMARIA

```
ALTER TABLE nombreTabla ADD PRIMARY KEY(nombreCampo);
```

- ELIMINAR PRIMARIA

```
ALTER TABLE nombreTabla DROP PRIMARY KEY
```

- CREAR FORANEA

```
CREATE TABLE nombreTabla (
	nombreCampo propiedades,
	...
	FOREIGN KEY(campoHijo) REFERENCES otraTabla (campoPadre)
	ON DELETE RESTRICT ON UPDATE CASCADE
);
```

- MODIFICAR FORANEA

```
ALTER TABLE nombreTabla
ADD FOREIGN KEY (campoHijo) REFERENCES otraTabla (campoPadre)
ON DELETE RESTRICT ON UPDATE CASCADE;
```

- BORRAR

```
ALTER TABLE nombreTabla DROP FOREIGN KEY;
```

- WHERE

```
SELECT campo1, campo2, campo3
FROM tabla1, tabla2
WHERE campo1a = campo2b
```

- JOIN + WHERE

```
SELECT *
FROM tablaA JOIN tablaB
WHERE tablaA.campoA = tablaB.campoB
```

- JOIN + ON

```
SELECT *
FROM tablaA JOIN tablaB
ON tablaA.campoA = tablaB.campoB
```

AÑADIMOS TABLA CON CAMPO PARA QUE EN CASO EN DOS TABLA HAYA EL MISMO CAMPO RECOJA EL QUE NOSOTROS NECESITAMOS

```
tabla.campo
```

![[Pasted image 20241030103621.png]]

- CONSULTA 2 O MÁS TABLAS

```
SELECT *
FROM tablaA
JOIN tablaB ON tablaA.campoA = tablaB.foraneaA
JOIN tablaC ON tablaC.campoC = tablaB.foraneaC 
```

O

```
SELECT *
ON tablaA.CampoA = tablaB.foraneaA
AND tablaC.campoC = tablaB.foraneaC
```

