La función principal de la capa de red es la de llevar a cabo el enrutamiento o encaminamiento, este debe averiguar por cuál interfaz digirlos para que continúen su camino. 

El router utiliza un protocolo de encaminamiento, que utiliza un algoritmo. 

## Configuración y administración de protocolos dinámicos. 

Los protocolos se dividen:

- Encaminamiento estático.
- Encaminamiento dinámico.

### Protocolos Routers y protocolos de encaminamiento

- El protocolo define el funcionamiento a realizar, o conseguir algo.
- Un algoritmo es el conjunto de instrucciones ordenadas para solucionar o conseguir ese algo. Un protocolo no produce un resultado pero el algoritmo si.

- Un protocolo de routin o encaminamiento define como elegir camino hacia el destino.

### Protocolos de encaminamiento interior y exteiror

En Internet se dan como mínimo, dos nivelees jerárquicos de routing: uno dentro de un sistema autónomo y otro entre. El primero interno (IGP, Interior Gateway protocl) y el segundo externo (EGP, Exterior Gateway Protocol). 

Un punto neutro de interconexión interconecta sistema autónomos. 

## Encaminamiento estático vs encaminamiento dinámico

- Encaminamiento estático: establece de manera estática las rutas hacia las redes de destino. Se utiliza la capacidad de la línea, el tráfico. Cuando se utiliza este tipo de encaminamiento no intercambia información al adaptar la ruta.
- Encaminamiento dinámico: Las rutas se calculan continuamente. En base a la información de interconexión.

## Algoritmos de Encaminamiento

- Principio de optimalidad

### Encaminamiento por el camino más corto y métricas

- La capacidad que soporta el enlace
- Tráfico medio
- Retardo
- Fiabilidad

### Basado en flujo

Basado en el tráfico medio de los enlaces. 

### Por inundación

Si se recibe un paquete se rrenvía por el resto de interfaces. 

- Inundación selectiva
- Incorporación de un contador de saltos

### Vector Distancia

Se basa en la construcción, por cada router, de una tabla donde se calcula la distancia mínima hacía todos los posibles destinos. 

Una vez calculada la tabla, cada router intercambia con los routers vecinos y actualiza la suya propia, volviendo a calcular la distancia hacia cada router con al nueva información. 

## Por enlace

- Averiguar quiénes son los router vecinos y direcciones
- Calcula la distancia
- Hacer un paquete con toda la informació ny enviarlos a otda la red
- Con toda la información, calcula cuál es el camino con menos distancia

![image](https://github.com/user-attachments/assets/134772d7-fb80-48cf-a234-dfe82fb51d3c)

## Protocolo RIPv2

RIP es acrónimo de Routing Information Protocol. Protocolo de encaminamiento interior basado en el algoritmo del vector distancia.

![image](https://github.com/user-attachments/assets/ec88130f-765d-4166-b32a-727f4a9cf9cd)

![image](https://github.com/user-attachments/assets/2965e015-c676-41e9-af23-19891fd13f93)

## Configuración y adminsitración de RIPv1

![image](https://github.com/user-attachments/assets/c785b9cc-98b4-487b-9eeb-dc7d66b26551)

Comprobar el protocolo de encaminamiento 

```
show ip protocols
```

Comprobar las rutas que ha aprendido

```
show ip protocols
```

Cómo se intercambian la información de encaminamiento

```
debug ip rip
```

Parar de ver mensajes

```
undebug all
```

![image](https://github.com/user-attachments/assets/315070f4-d6bf-49b6-8c4c-0191d841d3b5)

## Administración y configuración de RIPv2

![image](https://github.com/user-attachments/assets/ea250846-7ecc-40e2-9309-8092aa7a8f08)

