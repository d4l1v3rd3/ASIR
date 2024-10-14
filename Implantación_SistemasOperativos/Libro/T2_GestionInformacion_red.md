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

- Ext2fs: Aprovecha mucho más el espacio libre y reduce la fragmentación interna de los archivos en comparación del FAT, volumen de 4TB y albergar archivos de 2TB.
- Ext3fs: Mejor que la anterior. Es más rápido y eficiente aunque, no existen grandes diferentes, volumen de 32 TB y albergar archivos de 2TB.
- Ext4fs: Se sustituye el esquema de guardado tradicional de las dos anteriores, se reduce aún más la fragmentación, y tanto la lectura y escritura aumentan. Volumen de 1EB y almacenamiento hasta 16TB.

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

# Identificación de software mediante comandos y herramientas gráficas

- Astericsco: Sustituye a una cadena completa de caracteres a la hora de buscar, pudiendo reemplazar el nombre completo
- Interrogación: Reemplaza solo un carácter.

# Gestión de la información del sistema. Rendimiento

Para poder ver la "salud de nuestro" equipos podemos verlo accediendo a "Propiedades de Equipo/Evaluación" por otro lado existe la herramienta "Monitor de rendimiento"

# Montaje y desmontaje de dispositivos en sistemas operativos

El concepto "montar" hace referencia al hecho de que una unidad de almacenamiento sea accesible por el propio sistema. 

Cada unidad que se "monta" se asigna una letra, como si fuera otra unidad de almacenamiento, aunque se trate de otra particiçon. 

```
 Tenemos nuestra carpeta de Música compartida con
varios usuarios, donde todos ellos están copiando archivos
de audio. Esto provoca que nuestra unidad de disco se esté
llenando cada vez más. Pero si tenemos alguna partición libre
(en nuestro equipo o en un recurso que tengamos en la red),
podemos crear una carpeta que se llame Rock, otra que se lla-
me Blues y otra que se llame Country, y que cada una apunte
a una partición vacía distinta, consiguiendo de este modo que
no se sature nuestra unidad de disco.
```

# Automatización

Existen tareas dentro del sistema que deben de automatizarse, con una periocidad concreta.

### Windows

/ Sistema y seguridad / Herramientas administrativas /
Administración de equipo / Programador de tareas

Procedimiento:

- Elección de las tareas a automatizar
- Nombre de archivo con extensión .bat
- Programción de las tareas automatizadas

# Herramientas de administración de discos. Particiones y volúmenes. Desfragmentación y revisión

- Desfragmentación del disco: Si en un disco se producen muchas operaciones de guardado, eliminación y modificación de los archivos, dará lugar a la fragmentación de la información, lo cuál afecta negativamente al rendimiento. Defragmentar supone localizar las partes de un mismo archivos que estan fragmentadas y consolidarlas en espacios de memorias contiguos.
- Liberar espacio en disco: Eliminar archivos que no son útiles, bien porque son temporales o caché.
- Convertir sistemas de archivos: No se produce perdida de datos y siempre se hará con el enfoque de aumentar el rendimiento de las operaciones del disco.

# Permisos locales de acceso a archivos y directorios

- Permisos explícitos: Los que se le configuran a un directorio o archivo.
- Permisos heredados: Son los que se propagan a un subdirectorio o archivo secundario al ser creado desde un directoio o archivo principal.

# Cuotas de disco

Son límites que un administrador aplica a un usuario o grupo,  para evitar que supere cantidad de recursos de un sistema de archivos, o crear una jerarquía de accesos a los usaurios.

También aplican a los archivos de forma individual.

# Comprensión de datos

Archivo comprimido = menor espacio

Winzip, Winrar o 7-zip




