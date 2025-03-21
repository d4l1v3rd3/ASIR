# Seguridad, rendimiento y recursos

# Aseguramiento de la información

## Extensión de un volumen. Volúmenes distribuidos. RAID0 por software

Un volumen de almacenamiento se puede extender si contiene un sistema de archivos NTFS, aumentando el espacio.

Tenemos entonces lo que llamamos "volúmenes distribuidos" formados por varios espacios en disco distribuidos en diversas unidades de disco. 

RAID con características especiales:

- Capacidad
- Tolerancia a fallos
- Disponibilidad y seguridad
- Rendimiento

## Tolerancia a fallos de hardware RAID1 y RAID5 por software

Para implementar técnicas de tolerancia a fallos lo más común:

- RAID1: Replicada en un volumen "gemelo" Mantener una copia exacta de la información en otro sistema de discos. (Espejo)
- RAID5: Almacenados por bloques y la información redundante se almacena de forma cíclica entre todos los volúmenes

## Tolerancia a fallos de software de los datos

Existe una serie de componentes de backup o de emergencia que asegurarán la no interrupción del ssitema y realizarán la tarea que deberia estar ejecutando.

- Hardware: Componente físico ocupa el lugar de lque ha fallado, como un servidor de resptaldo o unidad de disco
- Software: Información que puede ser replicada en varias tablas o bases de datos.
- Energía: Pueden suministrar corriente si se detecta un fallo en la línea principal.

## Tipo de copias de seguridad

- Completa: Todo el contenido cada vez que se ejecuta
- Incremental: Primera copia de tipo "completa" y luiego se copia la información posterior
- Diferencial: COpia que replica todos los datos creados y modificados desde la última copia de seguridad completa
- Espejo: Refleja todos y cada uno de los comportamientos de al fuente
- Sintética ocmpleta: Réplica de la copia completa a partir de incrementales y/o diferenciales.

### Origen y destino

- Locales
- Externas
- Remotas
- Online

### Según el usuario

## Plantes de copias de seguridad. Programación de copias de seguridad

Windows + I - Actualización y seguridad

![image](https://github.com/user-attachments/assets/bd25e3d7-a060-47cc-8e22-bd8a9674be64)

Copia de seguridad

![image](https://github.com/user-attachments/assets/065c55e9-fbb9-4e96-8616-bc8db59cee06)

![image](https://github.com/user-attachments/assets/75831472-a000-42d8-9c24-ac1ede342da8)

Mas opciones

![image](https://github.com/user-attachments/assets/7e0b8369-fdd9-4f6d-9e73-bb7bbc74d7e5)

## Recuperación en caso de fallo del sistema

- Actualización mal hecha, borrado de archivos clave, virus, mala gestión de particiones

- Restaurar el sistmea
- Reparación bloque de inicio
- Reparación de imagen del  sistema
- SImbolo del sistema
- Diagnóstico de Windows

## Discos de arranque. Discos de recuperación

Unidad de recuperación

![image](https://github.com/user-attachments/assets/ec8e50fc-a06e-4ed4-abe8-423058beb11c)

Realizar copia de seguridad - siguiente

![image](https://github.com/user-attachments/assets/343af199-9910-46d9-b30b-0ab1f875a208)

![image](https://github.com/user-attachments/assets/7f11abda-a11b-4e60-bc18-f578ca8dccc0)

![image](https://github.com/user-attachments/assets/42585ae7-8165-4201-b4a5-310b249e2f43)

## Copias de seguridad del sistema. Recuperación del sistema mediante consola. Puntos de recuperación


