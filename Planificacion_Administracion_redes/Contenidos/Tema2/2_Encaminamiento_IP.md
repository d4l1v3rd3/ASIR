# Encaminamiento IP

# Encaminamiento

Enrutamiento es el prcoeso de reenviar paquetes entre dos redes conectadas. En redes basadas en TCP/IP, el enrutamiento forma parte el protocolo IP

Todos los equipos que ejecutan TCP/IP toman decisiones de enrutamiento. 

- Cuando configuran las interfaces de red del equipos, se va completando automaticamente su taba de encaminamiento local
- En cada fila de ta tabla se específica
- La dirección IP y máscas de la red que puede alcanzar
- La interfaz por ala que debe salir el paquete
- Como puede haber más de un camino para un mismo destino, se usa métrica para especificar el camino

![image](https://github.com/user-attachments/assets/776fe223-9b59-4afc-bcc7-b4d5f79d3476)

## Ejemplos

- LAN 1: 216.89.3.0. Máscara de subred:255.255.255.0
- LAN 2: 192.64.126.0 Máscara de subred: 255.255.255.0
- LAN3:188.119.0.0 Máscara de subred:255.255.0.0

3 Encaminadores A B Y C 

![image](https://github.com/user-attachments/assets/81e3d9ab-58ca-48eb-92db-cfa8050bb0ea)

El router, cuando tiene un paquete de datos con una IP y quiere saber porqué interfaz tiene que enviar, consulta la tabla. Lee y procesa la orden de cada una de las filas. Si se encuentra coincidencia entre al red destinodel paquete y al red dará finalizado el trabajo, enviaraá el apquete por la interfaz correspondiente al siguiente puerto de entrega

![image](https://github.com/user-attachments/assets/58e7b9c0-30ad-4171-a210-7d57c0f23d2e)

- - Las dos primeras filas se corresponden con direcceiones de redes locales directamente conectadas al router. La dirección de red es 216.69.3.0 con máscara 255.255.255.0 indica que se puede alcanzar la red 216.89.3.0 desde el router. La interaz tiene la IP 216.89.3.1
- - Las dos últimas filas son para redes que están fuera de alcance directo en erutador. La IP que aparece en el campo siguiente puerto es la de el otro router alcanzable por una de las dos LAN que estan conectadas
  - El enrutador dará salida a los paquetes que vayan a la red 118.119.0.0 enviandolos al encaminador B. La IP del encaminados B es un Gateway
  - El enrutador A dará salida al resto de los paquetes con destino a redes distintas.
 
![image](https://github.com/user-attachments/assets/16916827-71a3-41a3-b42c-d2e5e544a3ad)

- Si la IP destino está la misma red que el enrutador, el valor del número de saltos o métrica es 0, en este caso indicará que la interfaz de salida es la salida del enroutador
- Si la red destino no es directamnete alcanzable, en la red de la tabla correspondiente se especificará la IP del puerto del siguiente enrutador, Gateway

![image](https://github.com/user-attachments/assets/9c735d66-4983-4523-a9f1-0ad639495e37)

 - La dirección IP 23.65.211.80 pertenec a un encaminador externo que no se encuentra dentro de internet

## Tablas de enrutamiento Locales

### NTSTAT

Permite ver las tablas de enrutamiento, las estadísticas de las distintas intefaces de red y las conexiones que hay en este momento en la red

El servicio más comun del comando netstats muestra conexiones y los servicios disponibles

```
netstat -r
```

![image](https://github.com/user-attachments/assets/28df10a3-faf1-4644-96b3-78d561eea25e)

![image](https://github.com/user-attachments/assets/9c894e60-f18b-4eb0-98fa-eb9e7572fade)

```
ip route show
```

## Rutas de Red WIndows

![image](https://github.com/user-attachments/assets/1a0b230a-5c89-425d-bb48-a1c41af13fe9)


