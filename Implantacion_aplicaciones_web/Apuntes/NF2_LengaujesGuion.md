# Integrar Scripts de PHP en HTML

Podemos incrustar código PHP en un archivo .php o en un archivo .html 

Sintaxis php:

```
<?php
echo "Hola Mundo";
echo 2+5;
?>
```

# Variables en PHP

## ¿Cómo definimos una variable?

- El nombre de la variable se inicia con el símbolo $
- Seguido de una letra o del símbolo guión bajo
- Después puede contener letras, números o el símbolo guión bajo
- PHP distingue entre mayúsculas y minúsculas

## Tipos de datos

- PHP es un lenguaje no tificado
- Tipos de datos

```
String, Integrer, Float, Booleano, Array, Objeto, NULL, recurso
```

- La misma variable puede contener diferentes tipos de datos
- Existen sentencias para saber que tipo de dato tiene una variable

```
<?php
  $nombre = "Eva"; # Crear variable 
  $numero= 7; # Crear variable Númerica
  $float = 5.3; #Variable Float
  $true = true; # = 1 o false = 0 # Booleano
  echo "Nombre: ".$nombre. "<br>";
  var_dump($nombre) #Ver tipos de datos
?>
```



