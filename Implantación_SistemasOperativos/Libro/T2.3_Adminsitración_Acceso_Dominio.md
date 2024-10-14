<h1 align="center"> Administración del acceso al dominio </h1>

# Equipos del dominio

- Equipos físicos: Ordenadores, impresoras, escáneres, etc.
- Equipos lógicos: Direcotrios de trabajo, unidades de red, carpetas compartidas, etc.
- Usuarios y grupos: Las personas que hay detrás de un equipo y su tipo de agrupación
- Servicios: Listas de distribución, FTP, e-mail, etc.

# Permisos y derechos

- Permisos: Se aplican sobre los recursos y variarán en función del usuario o grupo que intente acceder a ellos, (lectura, escritura, borrado)
- Derechos: Se aplica sobre la forma en la que el usuaio o grupo accede al sistema, lo que pueden o no hacer (copias de seguridad, inicio de sesión, etc)

# Administración del acceso a recursos. SAMBA. NFS

El sistema operativo Linux tiene su propio sistema para compartir carpetas en red: NFS (Network File system) y para Windows utiliza el protocolo SAMBA

## NFS

Diseñado para compartir recrusos entre ordenadores Linux. 

La gran mayoría de distribuciones incluye ya el servicio, hay que iniciar sesión y configurarlo.

NFS se basa en la arquitectura cliente-servidor, ya que existe la posiblidad de configurar un equipo como servidor y el resto como clientes.

El equipo que actua como servidor, además de llevar la esguridad y configurar los permisos, albergá toda la información de usuarios/equipos conectados a NFS

## SAMBA

Este protocolo permite a ordenadores Linux compartir archivos y directorios con ordenadores Windows. 

También con arquitectura cliente-servidor, los sistemas Linux actuan como si feuras Windows, incluyendo ser controladores de dominio.

Tiene interfaz grácica desde Windows mediante la herramienta SWAT o en "smb.conf"

# Permisos de red

A nivel local, Cada usuario puede compartir una carpeta con un tipo de usuario, grupo o bajo una serie de restricciones (permisos locales) 

- Permisos efectivos, nos lista permisos que se conceden al grupo o a los usuarios seleccionados.
- Los permisos que se propagan desde los elementos que administramos a las capas inferioes (Permisos heredados)

# Delegación de permisos

Añadir en grupo a un usuario

# Listas de control de acceso

Las lsitas de control de acceso o ACL (Accel control list) se usan para determinar permisos a usuarios que no son el propietario del recurso y grupos que no sean los propios.

- Lectura: r
- Escritura: w
- Ejecución: x

## Linux

- Owner
- Group
- Other

# Directivas de grupo

Las directivas de grupo son propiedades de Windows Server, nos dan la posibilidad de especificar un conjunto de reglas que pueden aplicarse de manera general a las cuentas de equipo y de usuario.

En windows podemos acceder a ellos mediante el comando 

```
gpedit.msc
```

Esto nos permitirá ver las directivas locales en un editor

```
gpedit.msc /gpcomputer: "nombredeequipo"
```
si queremos verlas en el AD

```
gpedit.msc /gpcomputer:"nombreequipo.dominio.com"
```

# Estructura del grupo de trabajo

- Grupo de trabajo: Agrupación de ordenadores en red, comparte recursos de software y hardware, ya que por lo común están en la misma localización, no existe servidor principal.

- Workgroup por defecto

# Estructura lógica y física de directortio activo

## Estructura lógica

- Objetos: Entendemos por objetos a usuarios, equipos o importaras.
- Unidades Organizativas: Objetos que contienen otros objetos con la idea de organizar de forma lógica la red.
- Dominios: Colecciones de objetos administrativos que comparten una BD en común.
- Árboles de dominio: Agrupaciones de dominios con una ordenación jerárquica.
- Bosque: Conjunto de uno o varios árboles de dominio.

![image](https://github.com/user-attachments/assets/9e9b3b95-c7f2-489f-a2e2-3b509f7efadc)

## Estructura física

- Controladores de dominio: Servidores que realizan funciones de almacenamiento y repliación. Se aseguran de la disponibilidad de AD
- Sitios del directorio activo: Grupos de equipos conectados que pertenen a un domiinio.
- Catálogo global: Información del dominio, creado con la idea de habilitar a otros controladores.
- Particiones de directorio activo: Información de la BDE de AD se almacenan las particiones.

Partición de dominio: Guarda la información de usuarios, grupos.
Partición de configuración: Guarda la información de configuración global.
Partición de esquema: Donde se definen las clases y atributos de los objetos
Partición de aplicación: Se utiliza a nivel DNS

# Replicación entre sites





