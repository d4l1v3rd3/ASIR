# Direccionamiento MAC

## Direccionamiento a nivel de enlace de datos y a nivel de red

### Elementos necesarios

- Esquema de direcciones : Permitiendo identificar el origen del mensaje y del destino de la misma
- Método de encaminamiento: Permite usando el esquema de direcciones, localizar el destino de la información

El mensaje enviado es troceado y etiquetado por los protocolos de la máquina origen, puesta en la puerta de salida y enviada, atravesando encaminadores. 

![image](https://github.com/user-attachments/assets/58f07336-f64e-4343-8fa6-81247f980b34)

En la figura tenemso direcciones físicas (MAC) que corresponden con el nivel de enlace y direcciones IP o direcciones lógicas.

## Protocolos Usados

- Los protocolos usados para el direccionamiento a nivel de enlace tienen características distintas según se trate de redes LAN o WAN:

- Las redes WAN usan redes punto a punto
- Las LAN son redes de difusión que usan medios compartidos.
- Para distinguis las estaciones conectadas en el mismo enlace de difusión usamos la direccion de enlace
- Para la administración de al red y facilitar la localización de un destinatario se usa el direccionamiento a nivel de red
- En las LAN coexisten, casi siempre, ambos tipos de direccionamiento

## Direccionamiento físico o de enlace de datos

- La dirección MAC (Media Acces Control) identifican de forma única el adaptador de red
- Los identificadores MAC tradicionales de los adaptadores de red están formados por 48bits (MAC-48) esta dirección es denominada IEEE 802 representada por 6 bloques hexadecimales
- Los primeros 24 bits identifican al fabricante, estos bits reciben de nombre identificador único de la organización (OUI), IEE es quién asigna los valores de OUI a cada fabricante.
- Los siguientes 24 identifican al adaptador de red para ese fabricante.
- La dirección MAC también se conoce como dirección física
- Es única para cada dispositivo
- Va grabada por el fabricante en el adaptador de red

![image](https://github.com/user-attachments/assets/a32154d5-4c01-44cf-8442-7577dcd7f9e9)

En el número dado al fabricante por la IEEE hay dos bits que quedan libres para que el administrador los modifique si quiere

- Bit U/L Primer byte, es el penúltimo bit menos significativo. Se está a 0 significa que IEEE fue quien suministró la dirección y es una dirección Universal.
- Bit I/G El bit menos significativo

El nuevo estándar aumenta los identificadores a EUI-64 aumentando el tamañó de identificador sigue teniendo 24 bits por el id de extensión aunmenta a 40

- Dirección MAC de difusión: Hay una dirección compuesta solo por 1S que es especial
- Dirección MAC de multicast: Tiene un funcionamiento parecido al anterior, la trama puede ser aceptadada por varios equipos a la vez

## Comandos

Windows

```
ipconfig /all # Muestra la información de cada uno de los adaptadores de la red del pc
```

Linux

```
ifconfig
```

## Como modificar la MAC

Windows : Panel de control > Sistema e Seguridad > Sistema > Gestor de dispositivos de sección de adpatadores de red > Propiedades 

Linux 

```
sudo ifconfig eth0 down
sudo ifconfig eth0 hw ether 00:A1:BB:CC:DD:EE
sudo ifconfig eth0 up
```

