# INSTALACIÓN, CONFIGURACIÓN Y EXPLOTACIÓN DEL SISTEMA INFORMÁTICO

# ÍNDICE

# INTRODUCCIÓN

Conoceremos las partes de un sistema informático, comunicación y arquitecturas.

Licencias de software, diferencias prestaciones, código abierto y propietarios.

Una vez todo montado, administraremos el sistema. Configuraremos usuarios y grupos, vulnerabilidades, máquinas virtuales.

# INSTALACIÓN DE SOFTWARE LIBRE Y PROPIETARIO

## ESTRUCTURA Y COMPONENTES DE UN SISTEMA IINFORMÁTICO

- Hardware: Elementos físicos que componen el sistema.

Todos los dispositivos giran en torno a la CPU (Unidad central de procesamiento), todo lo que se conecta a esta se denomina "dispositivo periférico". LLegando al microprocesaodr.

### Dispositivos de entrada:

- Teclado
- Ratón
- Webcam
- Digitalizadores audiovisuales
- Sensores

### Dispositivos de salida:

- Pantallas
- Impresoras
- Trazadoras/plóters

### Dispositivos de almacenamiento:

- CD/DVD
- USB sticks o pendrives
- Discos duros mecánicos
- Discos duros SSD
- Tarjetas de memoria

Hay dispositivos como "adaptadores de red, pantallas táctiles" que son de entrada como de salida.

Cuanto más reducido y compacto, más fácil de transportar pero mejor rendimiento por calor.

Tenemos dos tipos de conexión por red (RJ45/Ethernet) (WIFI)

En este caso es la clasificación de cables de red:

![image](https://github.com/user-attachments/assets/509de3c8-c796-4e3b-a057-25b3d7960210)

La frecuencia determina la potencia de red, anchura y porcentaje de pérdida de datos, conforme crece la longitud. Cuánto más largo sea el cable, mayor potencia se pierde.

- Apantallamiento: "Blindaje" del cable que protege la corriente.

Dependiendo del apantallamiento tenemos diferentes cables:

### UTP (Par trenzado no apantallado)

- Cable sin apantallamiento.
- Instalaciones domésticas o equipo a equipo.
- Malo cerca de campos electromagnéticos

### FTP (Par trenzado o pantalla global)

- Recubrimiento por la parte interna, protegiendo contra las interferencias externas

### STP (Par trenzado apantallado)

- Cada par de cables rodeado por una malla.
- Instalaciones eléctricas que par por dentro de pared.

### SFTP (Par trenzado blindado y apantallado)

- Combinación FTP Y STP
- Rodeados por una malla, y a la vez recubrimiento extra
- Evita interferencias eléctricas y preparados para tiras largas.

## MAPA FÍSICO Y LÓGICO DE UNA RED

- Red: Conjunto de dispositivos conectados entre sí, para la transferencia de información. (Routers, Hubs, Swiches)

### Mapa de red lógico

Describe la manera en que fluirá la información dentro de la red.

- Subredes que puedan existir, máscara, IP. etc
- Elementos físicos, como routers o firewalls
- Protocolos de comunicación y enrutamiento

### Mapa de red físico

Describe la forma "real" que compone la red, físicamente ubicados.

- Topología de red: Disposición física de los elementos de la red. En forma de dibujo.

### Topología de bus

- Conectado mediante una conexión central.
- Posee dos puntos de conexión.
- Se configura fácilmente y poco cable.

![image](https://github.com/user-attachments/assets/ba618fcf-23b7-4647-b2db-8de9ee5cdec8)

- Si el bus centra falla, toda la red cae.

### Topología de anillo

- Conectados entre si de forma circular.
- Mejor eficencia que bus.
- Fácil insertar o quitar elementos.
- Usando en WAN como en MAN

![image](https://github.com/user-attachments/assets/0cfc4393-e68b-43f8-8f53-d7a426bc3e28)

- Si un nodo falla, toda la red se ve afectada.

### Topología en estrella

- Un hub o Switch controla la información.
- Si un nodo o conexión con el elemento central cae, la red no se ve afectada.

![image](https://github.com/user-attachments/assets/6daa11a7-7d36-4293-82cc-cdbaa60990ae)

- Todo el peso es del concentrador.

### Topología en malla

Aquí tenemos dos variantes:

- Topología de malla completa: Todos los nodos conectados entre sí.

![image](https://github.com/user-attachments/assets/e9b92715-acbe-492d-ac3f-abd5b376efa5)

- Topología de malla parcial: Los nodos que mas comunicación tienen son los que están conectados

![image](https://github.com/user-attachments/assets/35c66afc-ffb1-41f7-a8f8-f1a8e78eff4f)

## ARQUITECTURA DE UN SISTEMA OPERATIVO

- Monolítico: Arquitectura antigua, único programa central que aborda múltiples rutinasque pueden llamarse entre sí.
- Por Capas: Cada capa contiene una serie de rutinas, comunicadas por la capa superior.
- Máquinas Virtuales: Emulan mediante Software sistemas operativos.
- Cliente/Servidor: El SO organiza rutinas y subprogramas dentro de módulos, pudiendo pedir o servidor información a otros módulos.
- Microkernels: Compuestos por un nucleo principal de coordinación de procesos y reserva de memoria, proporciona capa de comunicación entre procesos.

## FUNCIONES DE UN SISTEMA OPERATIVO

Debe estar diseñado y optimizado para satisfacer una serie de necesidades al usuario.

- Eficencia: Gestionar de forma optima los recursos.
- Escalabilidad: Incorporar de forma sencilla nuevos dispositivos o actuliazaciones.
- Modificable: Corección de fallos o paquetes.
- Evolución: Nuevas funcionalidaes.
- Comodidad: Ha de servidor para que el usuario realice tareas de mayor o menos complejidad.

## TIPO DE SISTEMAS OPERATIVOS

- MS-DOS: Diseñado por Microsoft, 1980, línea decomandos y permitía gestión de información desde distintos soportes de memoria.
- Microsoft Windows: Microsoft, ordenadores personales, interfaz gráfica.
- MacOS: Apple, ordenadores personales, Vinculación con hardware y también interfaz gráfica.
- UNIX: Bell Corp, 1970, lenguaje en C, desplegado en microcomputdores o hasta servicodres. Base de MacOS o Solaris.
- LINUX: Dominio público, Linus Torvalds. Kernel (núcleo) + paquetes - Debian, ubuntu, Redhat.
- iOS: Apple, hardware movil.
- Android: Google bajo Linux, hardware movil.
- HongMeng OS/Harmory OS: Huawei, propio hardware.
- OpenVMS: DEC, Compaq y HQ, entornos de tiempo compartido, tiempo real, procesamiento por lotes.

## TIPOS DE APLICACIONES






