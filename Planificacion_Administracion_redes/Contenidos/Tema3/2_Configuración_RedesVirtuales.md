# Configuración de redes virtuales

Lan, incluye tres capas:

- Capa de acceso: Incluyendo usuarios y a los grupos de trabajo.
- Capa de distribución: Encargada de encaminamiento, limitar los dominios de broadcast y multicast, y de la seguridad de la red (filtrado de paquetes). Encargada en la conectividad entre todos los dispositivos y el acceso a la WAM.
- Capa de núcleo. Dirigir tráfico lo más rápido posible a los destinos que no pertencen a la red interna.

## Características de las VLAN

- Posible comunicación entre dispositvios no localizados en la misma red física
- Utilizan gestores de software para compartimentizarlos

## Ventajas

- Pueden convertir un solo conmutador en múltiples conmutadores de manera virtual
- Ventaja económica
- Gestión de red más sencilla
- Optimiza la gestión y el uso de hardware
- Reduce el tamaño de los dominios de difusión
- Mayor flexibilidad
- Mejor control de tráfico
- Escalabilidad

## Tipos de VLAN

- Basados en el puerto: En la interfaz se conecta un dispositivo que pertenecerá a una VLAN u otra.
- Basadas en MAC: Clasifican las tramas en una VLAN u otra en funcioón de la MAC de origen

- VLAN de datos: Para transmitir datos, tráfico generado por usuarios.
- VLAN predeterminada: Creada por defecto.
- VLAN nativa: Asiganada a un puerto troncal. Pudiendo cirtucar tráfico de otras VLAN.
- VLAN de administración: Gestión y administración de conmutadores
- VLAN de Voz: Se usan para VoIP. Poder garantizar un ancho de banda y minima latencia entre las llamads de voz

## Tipos de enlaces

- Access: Trabaja únicamente en una VLAN. Normalmente para conectar dispostiivos terminales (portátiles, teléfonos)
- Trunk: Se puede transcurrir tramas de distintas VLAN. Se utiliza para conectar con otros conmutadores o encaminadores.

## Implantación y configuración

Tres redes - Administrativa - profesorado y alumnado, configuración ejemplo (dos edificios)

![image](https://github.com/user-attachments/assets/4ebdd749-fbca-4c37-8013-ccd690528816)

![image](https://github.com/user-attachments/assets/cc155b59-7afd-4c77-9785-ef9a9f100b78)

![image](https://github.com/user-attachments/assets/ad2f1f3b-06c6-4d14-a3af-047ce9d0e2ba)

## Protocolo IEEE 802.1Q

Define cómo se etiquetan las tramas que viajan por un canal para identificar la VLAN a la que pertenecen. 

![image](https://github.com/user-attachments/assets/fb251c4f-df39-4e25-b5f7-ba019df17e63)

![image](https://github.com/user-attachments/assets/cfa00e83-9459-4b81-8dbe-a0852468d155)

![image](https://github.com/user-attachments/assets/96ac506a-46c5-48ed-96ec-b37d3b3c9c59)

## Interconexión entre la VLAN

![image](https://github.com/user-attachments/assets/4f2a69ff-9c50-4f6e-814c-c92ce74d4bc4)

(Necesitamos un router)

![image](https://github.com/user-attachments/assets/40aa335e-ef40-4234-91a5-a4d8acf9258c)

![image](https://github.com/user-attachments/assets/916f0beb-ab3b-4c20-a894-ba2a2b1b1da0)

Enlace troncal y sub interfaces

![image](https://github.com/user-attachments/assets/b88f63a5-3580-4dbe-a0f6-8c46feb6161a)

Esta técnica se conoce como router-on-a-strick y utiliza en el router sub interfaces virtuales para superar las limitaciones de disponer de un número finito de interfaces físicas en los dispostivos.

![image](https://github.com/user-attachments/assets/ed77f33f-15f0-4925-9949-1cba698b3ce1)

![image](https://github.com/user-attachments/assets/65f2af48-5833-4dc1-90c9-0db92bf15dcf)

## Protocolos de adminsitración centralizadada de VLAN

VTP (Virtual Trunking Protocol) Permite configurar VLAN de manera centralizada, propagando la configuración de las VLAN a los conmutadores de la red. 

Modos de funcionamiento.

- Modo servidor: Modificar, crear o eliminar, transmitido al resto
- Modo cliente: No permite crear, modificar o eliminar las LVAN, solo sincronizarse
- Modo transparente: Manera similar al cliente, solo se modificar de manera local y no se procesa

![image](https://github.com/user-attachments/assets/b56f052e-187f-4d1b-8d13-7135827f83e6)

![image](https://github.com/user-attachments/assets/2d8f2d53-caf4-4237-83a1-a89feb5e1933)

![image](https://github.com/user-attachments/assets/52d17036-31c6-4a34-8cea-253393fd5619)

DTP (Dynamic Trunking Protocol), Se encarga de sincronizar el funcionamiento de las interfaces que unen dos conmutadores.

- Modo Acess: Coloca el puerto en modo no troncal
- Modo Dynamic auto: Queda a disposció nde negociar la configuración
- Dynamic desirable: Puerot intenta activamente pasar a modo troncal
- Trunk: Establece la interfaz como troncal
- Nonegotiate: No envía tramas DTP, y solo se configura el enlace com otroncal si al otra interfaz se configura como troncal.

![image](https://github.com/user-attachments/assets/241014bd-d491-4142-9c33-2b2abbd8b464)

![image](https://github.com/user-attachments/assets/ead80829-fd10-4aeb-b783-9e4133deef33)
