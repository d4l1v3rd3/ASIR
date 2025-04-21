# Configuración de Acceso a Interner desde una LAN

## Arquitectura de acceso a Internet

1. Formado por las redes de los operadores globales. Conectadas entre sí. Llamadas el blackbone, la troncal de Internet.
2. Formado por operadores que no alcanzan estar conectados a todos los puntos de Internet. Para poder alcanzar se conectan al Nivel 1
3. Formador por los operadores, por los ISP

Las LAN se conectan a Internet, normalmente a través de proveedores de nivel 3

## Tecnologías de acceso a Internet

- Cableada: Par trenzado, BPL, Coaxial, Fibra óptica
- Inalámbrica: Wireless, MAN, WAN

## Direccionamiento Interno y Direccionamiento Externo

- Direccionamiento Interno utilizado dentro de las LAN y el externo fuera.

- Direccionamiento privado:

- Clase A: 10.0.0.0
- Clase B: 172.16.0.0 a 172.31.0.0
- Clase C: 192.168.0.0 a 192.168.255.0

![image](https://github.com/user-attachments/assets/1d66e68d-7ab2-48de-ad23-e3790b564ae1)

## Origen NAT y Destino NAT

El NAT traduce, convierte direcciones IP públicas en privadas y viceversa.

NAT en origen cambia la dirección IP de origen. 

![image](https://github.com/user-attachments/assets/c6a26575-1be5-4299-af8b-128374582e00)

## NAT estático, dinámico, de sobrecarga e inverso

- Nat estático: Forma más sencilla, uno a uno. Consiste en cambiar una dirección IP interna por una externa y viceversa.

![image](https://github.com/user-attachments/assets/34860ea7-f669-4980-b76d-65fcc47ebfc3)

- NAT dinámico: Tradue de varios a varios y es capaz de cambiar varias direcciones IP privadas por distintas direcciones IP públicas.

![image](https://github.com/user-attachments/assets/a0daf11c-de61-4dab-8cfe-cbf1a8777eea)

- PAT: Varios dispositivos de la LAN, lo puden hacer compartiendo la misma ip Externa.

![image](https://github.com/user-attachments/assets/a0acc1d5-24c0-43d0-aa72-86419d689b64)

![image](https://github.com/user-attachments/assets/664298c1-8f06-46b2-9f5a-8bec3f0e3e02)

- NAT inverso: Se abren los puertos sin hacer realizado antes una conexión desde dentro de la LAN.

![image](https://github.com/user-attachments/assets/d48ff9f2-8852-4ff7-8e5c-87e35a9bf355)

![image](https://github.com/user-attachments/assets/3154c559-8206-4b63-812a-c615185720d9)

![image](https://github.com/user-attachments/assets/4ef46168-957f-4d85-9fc8-b497665c41fe)

## Configuración de NAT

![image](https://github.com/user-attachments/assets/f84c57c0-3c82-4747-8424-985aecb14882)

![image](https://github.com/user-attachments/assets/0704b191-f9e9-4828-842a-eca20282e18f)

## Configuración de PAT

![image](https://github.com/user-attachments/assets/9de78fa7-a64d-4ca1-bb9f-bd1b2704257e)

![image](https://github.com/user-attachments/assets/becc78ba-2bbf-42ea-b34e-0e2b222da08c)

## Redirecciones y Puertos

![image](https://github.com/user-attachments/assets/6c0d8ecb-2f4b-4dce-a123-247cecd31b7c)

![image](https://github.com/user-attachments/assets/c5955082-0b53-42fc-baf0-d2d16da403e0)

![image](https://github.com/user-attachments/assets/a9318bcf-3e9b-4e27-ae03-487ce621dceb)

## Diagnóstico de incidencias de NAT

![image](https://github.com/user-attachments/assets/81fc8821-3f53-4129-a599-6d3c97dad1a6)






