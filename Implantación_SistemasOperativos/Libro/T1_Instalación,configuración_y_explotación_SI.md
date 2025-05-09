# INSTALACIÓN, CONFIGURACIÓN Y EXPLOTACIÓN DEL SISTEMA INFORMÁTICO

# ÍNDICE

- [Introducción](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#introducción)
- [Estructura y componentes Sistema informático](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#introducción)
- [Cables red](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#introducción)
- [Mapa red](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#mapa-físico-y-lógico-de-una-red)
- [Topología red](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#topología-de-red-disposición-física-de-los-elementos-de-la-red-en-forma-de-dibujo)
- [Arquitectura SO](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#arquitectura-de-un-sistema-operativo)
- [Funciones SO](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#funciones-de-un-sistema-operativo)
- [Tipos de SO](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#tipo-de-sistemas-operativos)
- [Tipos de aplicaciones](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#tipos-de-aplicaciones)
- [Licencias](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#licencias-y-tipos-de-licencias)
- [Gestores de arranque](https://github.com/d4l1v3rd3/ASIR/edit/main/Implantación_SistemasOperativos/Libro/T1_Instalación%2Cconfiguración_y_explotación_SI.md#gestores-de-arranque)

# INTRODUCCIÓN

- Partes de un sistema informático, comunicación y arquitecturas.
- Licencias de software, diferencias prestaciones, código abierto y propietarios.
- Configuraremos usuarios y grupos, vulnerabilidades, máquinas virtuales.

# INSTALACIÓN DE SOFTWARE LIBRE Y PROPIETARIO

## ESTRUCTURA Y COMPONENTES DE UN SISTEMA IINFORMÁTICO

- Hardware: Todos los elementos físicos que componen el sistema.

- Todos los dispositivos giran en torno a la CPU (Unidad central de procesamiento), todo lo que se conecta a esta se denomina "dispositivo periférico". LLegando al microprocesaodr.

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

!! Hay dispositivos como "adaptadores de red, pantallas táctiles" que son de entrada como de salida. !!

- Cuanto más reducido y compacto, más fácil de transportar pero mejor rendimiento por calor.


# Red 

- Tenemos dos tipos de conexión por red (RJ45/Ethernet) (WIFI)

## En este caso es la clasificación de cables de red:

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

# Topología de red: Disposición física de los elementos de la red. En forma de dibujo.

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

### Aplicaciones de control

Coordinan y administran el funcionamientos de los elementos del sistema (memoria, almacenamiento, etc)

- Gestión del procesador: Encargados de las peticiones que llegan al prcesaodr.
- Gestión de memoria: Asignan y monitorizan almacenamiento de datos en la memoria.
- Gestión de entradas/salidas: Aplicación que se encarga de funcionamiento y gestión de información que "entra" y "sale"
- Gestión de datos: Encargado en la operacion como copiar, modificar, eliminar, etc.
- Gestión del sistema: Supervistan al resto de aplicaciones para una buena ejecución

### Aplicaciones de proceso

Sirven a los desarrolladores para crear nuevas aplicaciones y para darle al usuario una forma más óptima

- Traductores: Traduce las instrucciones de una aplicación para que las entienda el ssitema

Intérpretes
Compiladores
Ensambladores

- Programas de servicio: Gestión y administración de bloques de datos.

## Licencias y tipos de licencias

Licencias de software propietario: Autorizan el uso del software en función del rol contratado. 

- Licencia de administrador
- Licencia completa
- Licencia limitada

Licencia de software libre: Permite ejectura el programa, adaptarlo y modificarlo según necesidaes de cada usuario.

- Con copyleft
- Sin copyleft
- GPL
- BSD
- OpenSource Initiative
- Freeware
- Donationware
- Shareware

## Gestores de arranque

Softwarte que carga la memoria interna del sistema, diseñado para cargar los elementos que el sistema necesita para iniciarse.

Se ejecuta nada mas cargar el sistema.

![image](https://github.com/user-attachments/assets/ab2b8dc0-b051-4b7d-a71a-3e5aa8027e80)







