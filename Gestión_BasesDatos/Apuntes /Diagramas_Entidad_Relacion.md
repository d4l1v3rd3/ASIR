<h1 align="center">Diseño bases de datos</h1>

# Diseño conceptual y lógico

## Diagrama Entidad-Relación (ER) 

- Representación de elementos que se anotan en la base de datos y propiedades.
- Relaciones y características de las relaciones.
- Primer paso de la definición de la base de datos.

## Modelo Relacional

- Se representan las tablas con sus campos.
- Se identifican los campos claves y relaciones que se establecen.

![image](https://github.com/user-attachments/assets/757de141-a867-466e-b21a-dde4c2f91a11)

# BBDD relacionales

![image](https://github.com/user-attachments/assets/2a992610-0ad7-43ea-b38f-95fe3f015198)

# ER- Diagrama Entidad-Relación (ER)

- Representación gráfica utilizada para modelar datos de un sistema de información (plasmamos una situación de la vida real para poder plasmarla porsteriormente)
- Diseño conceptual

### Componentes

- Entidades = Componentes de la vida real (Representación en rectángulo)

```
coche - conductor
```

- Atributos = Características que definen una entidad (circulos)

```
matricula - modelo - color 
nombre - apellidos - DNI
```

```
por ejemplos los elementos claves en este caso de coche=matricula y de conductor=DNI
son atributos que nunca cambian
```

- Relaciones = Describen la asociaciones entre entidades y dependencia (Rombo) (Verbo en su interior)

```
conducir
```

![image](https://github.com/user-attachments/assets/a5f7f41f-ff42-48cf-affa-b795d48f0a42)

![image](https://github.com/user-attachments/assets/e4bd91d7-15f8-4927-bdbf-e2e0e79df1a6)

# ER: Cardinalidad de la relacion

- Representan las interrelaciones que existen entre dos entidades

```
profesor - Impartir - Asignaturas
```

Relación entre profesor - Asignaturas, establecemos el valor minimo y valos maximo de cada relación (Siempre valores maximos al acabar)

```
el profesor puede impartir muchas asignaruas ó pocas asignaturas
```
(0,N)
```
La asignatura es impartida por un profesor como minimo y como máximo
```
(1,1)

Relación : (1,N) (Uno a varios)

## Tipos de cardinalidad de la relación

- Uno a uno = Trabajador (0,1) - "Aparcar" - Plaza (0,0) = (1,1) "Puede el trabajado tener una plaza o no"
- Uno a varios = Equipo (0,1) - "Pertenece" - Jugador (2,N) = (1,N) "Puede el jugador tener o no un equipo pero el equipo tiene que tener 2 o + jugadores"
- Varios a Varios = Coche (0,N) - "Conducir" - Conductor (0,N) = (N,N) "El conductor puede conducir 1 o + igual que puede tener 1 o + coches"

![image](https://github.com/user-attachments/assets/f7850849-344b-4065-80ad-6e9b8d29b4e0)

## Entidades Conceptuales

- Cuandos dos relaciones tienen cadinalidades de varios a varios, para una base de datos es muy malo, con lo cuál lo que hacemos es añadir una relación en medios para convertir esa cardinalidad en una de uno a varios. (Se le llama entidad conceptual) (Pudiendo añadir atributos para diferenciarlo mejor)

![image](https://github.com/user-attachments/assets/643ba927-71d5-4be7-9bfb-5c7af1b0ef5c)

![image](https://github.com/user-attachments/assets/cdad2709-4d8f-4201-a478-c809d0a42957)


# Software de Diagrama ER

![image](https://github.com/user-attachments/assets/e662d040-38fe-42d4-8bb2-466ffb8d855e)

[Giffly](https://www.gliffy.com/?_gl=1*zbmczq*_gcl_au*MTUwNDk0MDk3NC4xNzI4Mjg1MzIz*_ga*MTU4MTQxNjU2MS4xNzI4Mjg1MzIz*_ga_JRGHPHEJZ1*MTcyODI4NTMyMy4xLjEuMTcyODI4NTQyMS42MC4wLjA)
 



