# Sistemas de archivos

Un sistema de archivos o sistema de ficheros (Filesystem) es el encargado de la asignación de espacio para los ficheros, la gestión de espacio libre o el acceso a los datos (permisos a usuarios sobre los archivos)

- Fat
- Fat32
- NTFS
- Ext4

## Fat

Fue creado por el sistema operativo MS-DOS.

Se basa en una tabla que indica dónde están los archivos dentro de la partición donde se está ejecutando el SO, así como los sectores de disco ocupados, los libres y los defectuosos. 

Desventajas:

- Nombres cortos (8 caracteres para el nombre y 3 de extensión) para los archivos.
- Tamaño de 2 Gb de partición como máximo.
- Clusters demasiado grandes, por lo que se desaprovechaba el espacio.
- Mucha desfragmentación.

## Fat 32

FAT32 utiliza entradas de 32 bits por el que se puede guardar más información en ellas.

Estas particiones admiten un tamaño de clúster más pequeño por lo que se desperdicia menos espacio. Permite trabajar con particiones de más de 2 GB.

Se introdujo con la aparición de Windows 98.

## NTFS

Fue creado para Windows NT y soportado por los sucesivos SO creados por Microsoft.

Proporciona características de rendimiento, protección, seguridad, cifrado, compresión y permisos en los archivos así como cuotas de espacio en disco.

Evita de forma eficiente la desfragmentación de manera que aprovecha mejor el espacio.

## EXT

Sistema de archivos de Linux.
Actualmente versión ext4 (mejora compatible de ext3). Fue diseñado para Rémy
Card para vencer las limitaciones del sistema MINIX.
Las mejoras son :
• Soporte de volúmenes hasta 1024 Pebibyte.
• Menor uso de la CPU y
• Mejoras en velocidad de escritura y lectura.

