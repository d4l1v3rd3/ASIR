<h1 align="center"> Gestión de la información  y de recursos en una red </h1>

- Conoceremos los diferentes sistemas de archivos.
- Exploraremos las automatizaciones de acciones, monitorizar rendimiento.
- Permisos usuarios

# Administración de la información

# Sistema de archivos

Permite la organización de los datos en dispostivios de almacenamiento del equipo. Viene determinado por una jerarquía, espacio, tratamiento de los datos, etc.

## Sistema FAT (File allocation Table)

- Windows y Linux
- Actualización de tabla lenta
- Los archivos se escriben en los primeros huevos libres que existan en la partición.

### Existen tres tipos de sistemas FAT:

- FAT12, espacio máximo de 32Mb y máximo de archivo 32Mb
- FAT16, espacio máximo 2Gb
- FAT32, Espacio máximo de 2Gb y un máximo de archivo de 2Tb.

También existen otros como, extFAT o HPFS.

### Sistema NTFS (NT Files System)

- Desarrollado para Windows NT
- Almacena a través de metadatos las características de los archivos.
- La información se guarda en un sitio y el archivo en otro.
- Soporta dominios y almacena datos, mejora rendimiento en escritua/lectura.
- Puede albergar arhcivos de hasta 16TB y alcanzar hasta 256TB

### ReFS (resilient File System)

- Último sistema desarrollado por Microsoft, sucesor NTFS
- Optimiza la disponibilidad de los datos y gestionar de manera más eficiente

## Sistema de archivos extendido

Es el utilizado principalemnte para Linux:

- Ext2fs
- Ext3fs
- Ext4fs

# Gestión de sistemas de archivos mediante comandos y entornos gráficos

![image](https://github.com/user-attachments/assets/77377e75-e701-4ef9-9178-a907abbd3302)

# Gestión de links

Existen dos tipologías de links o enlaces para acceder y trabajar archivos.

Enlaces simbólicos o enlaces directos.

Enlaces duros directamente al nodo.

# Estructura de directorios de sistemas operativos libres y propietarios

- Archivos/Fichero: Parte de la memoria del disco duro, guarda una serie de datos, identificados con un nombre y una extensión.
- Directorio/Carpeta: Agrupaciones de archivos o otros directorios, respecto a permsos o acciones.
- Ruta absoluta: "ruta"
- Ruta relativa "..\"

# Búsqueda de información del sistema mediante comandos y herramientas gráficas

Exploradores de carpeta y ficheros.

Herramienta de busqueda

# Identificación de software

- Astericsco
- Interrogación

