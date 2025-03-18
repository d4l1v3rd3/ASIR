# Subnetting o segmentación de redes

# Introducción

- Identificar la utilidad de la subredes
- Reconocer en una dirección IP las partes esenciales para poder cosntruir subredes
- Interpretar la información de una máscara de subred
- Obtener máscaras de subred para una situación dada
- Construir bloques CIDR
- Obtener las direcciones incluidas en un bloque CIDR

## Subredes

Consiste en dividir un espacio de direcciones IP en subredes lógicas, dividir una red grande en pequeas. Subconjunto de alguna de lacses de red 

### Factores

- Situación geográfica de los dispostivios
- Propósito de los dispositivos.

### Maneras

- Dividir el espacio de driecciones en redes del mismo tamaño.
- Dividir el espacio de direcciones en redes de diferente tamaño.

## Ventajas

- División de tráfico de la red entre las subredes que la componen.
- Reduce el tamaño de los dominios de broadcast
- Hace que la red sea más manejable, administrativamente hablando
- Más seguridad

## Division de la dirección IP en 3 niveles

- Parte de red: Podemos identificar la red, y la clse (NIC)
- Parte de host: Identificamos el equipo dentro de lared

- Identificador de red
- Identificador de subred
- Identificador de equipo

## Máscaras de subred

Al divir una red en subredes, los equipos que forman parte se consideran equipos de redes distintas.

Para conseguir que los equipos se vean habrá que modificar la máscara de subred.

Para construir la máscara de subred se cogen prestados bits de la parte de hosts que van a estar a 1 en la máscarata

![image](https://github.com/user-attachments/assets/4a5fd146-7774-49b3-a48f-d6b18094a19a)

PArtimos de una máscara e nlos primeros 16 bits identifican a la parte de red, con lo cual esta´riamos hablando de una clase b. cogemos 3 bits extra para identificas a las subred de esta forma se identifica por los 19 primeros bits los siguientes 13 son para identificar el hosts

### Tener en cueta

- Según la clase con la que trabajemos, podemos coger más o menos bits
- Como minimos cada subred tiene que tener 1 hosts y dos direcciones reservadas que identifiquen la subred y el broadcasts

![image](https://github.com/user-attachments/assets/cc3ce757-8401-4bf4-b154-dae2a6d629a6)

- Nunca se puede quitar bits al identificador de red
- Cuantos más bits pongamos para el identificado, menos quedaran para el número de hosts
- Para determinas que dos equipos pertenecen a la misma subred, deben tener los mismos valores en los bits de su dirección IP

## Notación CIDR

CIDR viene de ClassLess Inter-Domain ROuting. Esta estrateguia fuen introducida por 1993 por EFT y es una mejora en la manera de interpretar direccones IP de IPv4. 

Permitió una mayor flexibilidad para determinar el número de subred a partir de la máscara. 

### Ventajas

- Uso más eficiente de las direccion Ipv4
- Facilita el encaminamiento al permitir agrupa las direcciones IP en una sola entrada de la tabla de rutas

## Sintaxis y bloques CIdr

El conjunto que se agrupa mediante CIDR se llama nombre de bloque CIDR. Estos bloques comparten una misma secuencia inicial de bits

Los bloques CIDR ipv4 se identificas con una sintaxis parecida a las direcciones IPv4, 4 números decimales separados por puntos, seguidos por una barra de divisón y un numero de 0 a 32. 

128.111.3.67/24 - 255.255.255.0 

![image](https://github.com/user-attachments/assets/7f117ec5-5c47-4168-945e-3004cd80b33b)

## CIDR Y máscaras de subred

- 118.64.238.67/10: Indica que la dirección, perteneciente a una red clase A, utiliza 2 bits extra de la parte de host para número de subred, pudiendo definir hasta 4 subredes
- 195.0.167.23/27: Red de clase c con 3 bits que se cogen extra de la parte de hosts, hay un máximo de 8 subredes, como número de bits que restan para especificar el número de equipo son 5, cada subred puede tener un máximo de 32 direcciones, 30 equipos.

## Efecto

Cuando dividimos una red en subredes, sólo los routers y equipos que están dentro de la red deben conocer la existencia de las subredes y hacer uso de la máscara adecuada. Los routers externos no tiene porque. Simplicamos las tablas de ecaminamiento de estos routers, dando lugar a subred puede tener única entrada para toda la red.

![image](https://github.com/user-attachments/assets/1bd79378-04e2-407a-9173-22d0b8455d00)

## División en subredes de longitud fija

![image](https://github.com/user-attachments/assets/df029ce9-bed8-4a76-ac2b-faec607acb41)

![image](https://github.com/user-attachments/assets/de56711f-3f33-46b0-b2f0-b35289bcecd5)

