Protocolo: Representa comunicaciones entre distintos dispositivos lógicos o físicos
localizados en la misma capa (Comunicaciones horizontales)

Interface: Representa comunicaciones entre capas adyacentes dentro del mismo
dispositivo (Comunicaciones Verticales)

## Arquitecturas de red

Arquitectura de red: Un conjunto de capas y protocolos

Pila de protocolos: Conjunto de protocolos utilizados en una arquitectura de red

## ¿Qué es OSI?

- Open Systems Interconnection o Interconexión de Sistemas Abiertos
- Es el fundamento de las redes
- Mantiene interoperabilidad entre aplicaciones y dispositivos en las redes
- Establece una estructura conceptual de relación en las redes de forma universal
- Herramienta clave para resolución de problemas en las redes

## Capas del modelo OSI

![image](https://github.com/user-attachments/assets/e4ceb2f8-9f29-4f1a-9f36-d10f099ed678)

### Capa física

- Primera capa de interconexión.
- Capa de transmisión digital y señalización
- Se definen especificaciones de conectividad
- Capa más baja de comunicación
- Características eéctricas y mecánicas de la red (cables, conectores, señales
- eléctrica, etc)

### Capa de enlace

- Segunda capa de interconexión
- Método de acceso o estrategia para compartir el medio físico de transmisión.
- Encapsulación y sincronización
- Link lógico y control de flujo
- LAN Switching
- ARP (Address Resolution Protoc
- Unidad de datos: Trama

### Capa de red

- Tercera capa de interconexión
- Direccionamiento y enrutamiento de los paquetes en red
- Se establece la dirección IP
- Encapsulación de paquetes
- Es donde se reenvía la información (forwarding).
- Enrutamiento
- Dispositivo: Routers
- Protocolos comunes: IPv4, IPv6, ICMP,IGMP,IPSec..
- Unidad de información: Paquete

### Capa de transporte

- Cuarta capa de interconexión
- Es ña responsable del envío al destino del mensaje entero.
- Proporciona servicios de comunicación confiable de extremo a extremo o servicios de comunicación rápida son garantía de orden ni entrega. Servicios orientados a la conexión y no orientados a la conexión.
- Segmenta y ordena datos
- Multiplexa conexiones simultaneas de transporte en una única red.
- Fragmenta datos de la capa superior en unidades menores si es necesario.
- Puertos, sesiones, control de flujo, recuperación de errores. Previene el desbordamiento del receptor.
- Protocolos: TCP, UDP
- Unidad de datos: Segmento

### Capa de sesión

- Quinta capa de interconexión
- Iniciar, establecer, mantener y finalizar una sesión
- Controla las conectividades entre dos sistemas
- Define autentificación y autorización
- Establece si la conectividad se va a establecer o no
- Define si la conectividad sincronizará o no
- Protocolos de control de comunicaciones

### Capa de presentación

- Sexta capa de interconexión
- Formato de datos. Representación, codificación, compresión y cifrado de datos.
- Conversión de la data
- Traduce la información para las aplicaciones
- Encriptación y desencriptación. De una aplicación a otra los datos van cifrados. Ejemplo: Certificados

### Capa de aplicación

- Séptima capa de interconexión
- Funciones de usuario final (Transferencia de archivos, e-mail, páginas web, et)
- Presenta la interface de intercomunicación
- Es donde ocurren servicios, aplicaciones y administración
- Entrada y salida de la data
- Responsable de desplegar la interface al usuario
- HTTP, Telnet, SMTP

## Encapsulación

La forma que adopta una porción de datos en cualquier capa se denomina “unidad de
datos del protocolo (PDU)”. Durante la encapsulación, cada capa encapsula las PDU
que recibe de la capa inferior de acuerdo con el protocolo que se utiliza. En cada
etapa del proceso, una PDU tiene un nombre distinto para reflejar sus nuevas
funciones. 

- Datos: término general para la PDU que se utiliza en la capa de aplicación.
- Segmento: PDU de la capa de transporte.
- Paquete: PDU de la capa de red
- Trama: PDU de la capa de enlace de datos
- Bits: PDU de la capa física que se utiliza cuando se transmiten datos físicamente por el medio
- PDU: Protocol Data Units

![image](https://github.com/user-attachments/assets/c9ee36c9-2f6a-4aea-8b24-68e72caa3b6f)

## Modelo TCP/IP

- Transport Control Protocol/Internet Protocol
- Fue concebido para establecer de una manera conceptual como se comunica un nodo con otro nodo. Trabaja en paralelo al Modelo OSI
- Tiene 4 tapas: Red(subred), Internet(Intered), Transporte y Aplicación


### Capa 1 (Acceso a la red o Red o Subred)

- Punto de interacción o interfaz entre la red local y los protocolos TCP/IP
- Responsable de aceptar paquetes IP y realizar su transmisión sobre una red específica.

### Capa 2 (Internet o Intered)
 
- Al igual que la capa 3 del modelo OSI, recibe la petición de enviar un segmento de la capa de transporte y una dirección de destino para el paquete.
- Se encarga del direccionamiento lógico, enrutamiento, fragmentación, reenvío, etc.
- Se define un formato de paquetes y protocolo IP (Internte Protocol).
- IP,RIP,OSPF,ICMP,IPV6

### Capa 3 (Transprote)
 
- Proporciona servicios de comunicación confiable de extremo a extremo o servicios de comunicación sin garantía de entrega, segmenta y ordena datos, multiplexa conexiones simultáneas
- Define como una pareja de entidades de aplicación realiza una conversación sobre protocolo IP.
- Realiza detección/corrección de erroresy control de flujo.
- Identifica la aplicación específica de origen y destino.
- Define dos protocolos TCP y UDP

- TCP (Trasmision Control Protocol)
- Prococolo confiable
- Orientado a la conexión
- Permite que el flujo de bytes sea entregado a la máquina detino sin errores y en correcto orden.
- Realiza fragmentación de pensajes y control de flujo

- UDP (User datagram procol)
- Protocolo no confiable
- No orientado a conexión
- Permite mejores tiempos de respuesta o el uso de controles diferentes alos de TCP

![image](https://github.com/user-attachments/assets/fb2c0f82-7a1c-4f53-80fa-df1427188203)

### Capa 4 (Aplicación

- Representa la capa 5,6 y 7 del modelo OSI
- Abarca todos los protocolos de alto nivel: HTTP,FTP,SMTP,SNMP,DHCP,DNS, etc

## OSI vs TCPIP

La capa de aplicación del modelo TCP/IP es similar a las capas 5, 6, 7 combinadas del
modelo OSI, el modelo TCP/IP no tiene una capa de sesión. La capa de transporte de
TCP/IP abarca las responsabilidades de la capa de transporte OSI y algunas de las
responsabilidades de la capa de sesión OSI. La capa de acceso a la red del modelo
TCP/IP abarca el enlace de datos y las capas físicas del modelo OS








