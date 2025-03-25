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

## Procesar

```
<?php
  echo $_POST['nombre'];
  echo $_POST['email'];
?>
```

# Arrays, Condicionales y bucles

### Array

- Array: Es una variable especial que permite contener muchos valores con un único nombre
- Para acceder a los valores de un array se utiliza un índice numérico que se indica con 0.

```
$nombres = array ("Eva", "Toni", "Olga", "Juan");

// echo $nombres[2]; # Comentario

for($i=0;$i<count($nombres);++$i){ # Variable i cuenta todos los elementos
  if(fmod($i,2)==0) # Si la división entre 2 = 0 (par) se muestra por pantalla (si es impar no se muestra)
  echo $nombres[$i]."<br>"; # Hacemos que se muestre y de un salto

}
 
```

## Estructuras de control

- Condicionales : if, else, elseif, switch
- Bucles o iteraciones: for, while, do while

# Sesiones en PHP

Permite almacenar variables que podemos utilizar en diferentes páginas a cada usuario que accede se le asigna una ID única.

```
<?php
  session_start(); # empieza la sesión
  $_SESSION['usario'] = 'Pons'; #variable global y su nombre
  $_SESSION['importe'] = 1000;
  echo "el usuario es: ".$_SESSION['usuario']."y el importe es: ".$_SESSION['importe']; # dos variables concatenadas
  echo "<br><a href='sesion2.php'>Ir a la sesion 2</a>"
  session_unset(); #Quitar todas las variables
?>
```

```
<?php
  sesion_start();
  echo $_SESSION['usuario']; # sigue funcionando aunque no haya sido declarada la variable
?>
```

# Bucle Foreach

Estructura de control de tipo bucle = Foreach (Permite recorrer de manera sencilla los elementos de una array)

```
<?php
$personas = array ("Olga", "Juan", "Luis", "Ana");

foreach ($personas as $i) { #Coge cada valor de todos los elemenots de la array
    echo "$i <br>"; # Outputeamos los elementos en pantalla
}
?>





