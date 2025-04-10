<h1 align="center"> Administración de software de base </h1>

# ÍNDICE

- [Usuarios y Grupos](https://github.com/d4l1v3rd3/ASIR/blob/main/Implantación_SistemasOperativos/Libro/T1.2_Administracion_Softwarebase.md#administración-de-usuarios-y-grupos-locales)
- [Seguridad Contraseñas](https://github.com/d4l1v3rd3/ASIR/blob/main/Implantación_SistemasOperativos/Libro/T1.2_Administracion_Softwarebase.md#seguridad-de-contraseñas)
- [Configuración Protocolo TCP/IP](https://github.com/d4l1v3rd3/ASIR/blob/main/Implantación_SistemasOperativos/Libro/T1.2_Administracion_Softwarebase.md#configuración-del-protocolo-tpcip-en-un-cliente-de-red-direcciones-ip-máscaras-de-subred)
- [DNS](https://github.com/d4l1v3rd3/ASIR/blob/main/Implantación_SistemasOperativos/Libro/T1.2_Administracion_Softwarebase.md#configuración-de-la-resolución-de-nombres)

# Administración de usuarios y grupos locales

- Dentro de windows server existe una BD y conjunto de servicios que relacionan recursos del sistema con los usuarios = Active Directory

- En un servidor Windows existen cuentas ya preinstaladas y grupos de seguridad.

### Grupos AD:

- Grupos de seguridad: Asignación de permisos a los recursos compartidos.
- Grupos de distribución: Creación de listas de distribución para el corrreo.

### Caracterización: 

- Universal
- Global
- Local

# Usuarios y grupos predeterminados

## Usuarios

Cuentas o entidades de seguridad usadas para administrar y proteger el acceso y la ejecución de los recursos o de los archivos.

### Cuenta de administrador

- Primera cuenta que se crea. 
- Control total de los archivos, directorios.
- Puede crear otros usuarios, modificarlos o eliminarlos.
- La cuente no puede eliminarse o dehabilitarse
- Podemos cambiar el nombre "SID"

### Cuenta de invitado

- Deshabilitada por defecto
- Permite a usuarios poder iniciar sesión con permisos limitados

### Cuenta HelpAssistant

- Cuenta local que viene predeterminada
- Se usa para conectarse a otro equipo que ejecute Windows iniciandose por invitación.

## Grupos

- Administradores: Posee control total sobre el servidor.
- Operadores de copia de seguridad: Otorga la capacidad de hacer, recuperar y restaurar copias de seguridad.
- Operadores criptográficas: Permite realizar operacioes de cifrado/descifrado criptográfico.
- Ivitados: Perfil temporal que está activo mientra dure la sesión.
- Operadores de configuración de red: Orientado a que sus miembros puedan realizar modificaciones en la configuración TCP/IP.
- Usuarios del monitor de sistema: Monitoriza las variables del ssitema para evaluar el rendimiento del equipo.
- Usuarios del registro de rendimiento: Permisos de este grupo posibilitan la administración de los controladores de rendimiento, alertar y registros.
- Usuarios avanzados: Mismos permisos que el grupo "usuarios"
- Usuarios: Tareas de uso del sistema de forma normal.
- Usuarios de escritorio remoto: Usuarios pueden acceder servidor mediante terminal.
- Usuarios de COM distribuido: Este grupo puede iniciar, activar y usar objetos COM en un equipo.
- IIS_IUSRS: Publicación y administración de contenido de IIS

# Seguridad de cuentas de usuario

Toda la seguridad en las cuentas de usuario recae sobre aquel quelas configura, administra y gestiona, que en este caso será la cuentadel administrador del sistema.

- Uso de contraseñas
- Privilegios
- Permisos

# Seguridad de contraseñas

# Administración de perfiles locales de usuario

La cuenta de usuario guarda información de los archivos y carpetas a los que el dicho usaurio tiene acceso.

Tener varias cuentas permite compartir recursos desde el mismo equipo.

Usuarios únicos y cumplir una serie de reglas:

- No se admiten caracteres especiales como /, |, :, ;, =, <, >,*
- No se admiten espacios en blanco.
- Máximo de 20 caracteres entre letras y números, mayúsculas y minúsculas.

# Configuración del protocolo TPC/IP en un cliente de red. Direcciones IP máscaras de subred

La dirección IP es un código numérico asignado por el proveedor de servicios de internet (ISP)

![image](https://github.com/user-attachments/assets/412f9e75-8de1-4823-8296-401a55319926)

A nivel interno de una LAN, tenemos que diferenciar IP pública con local.

```
ipconfig /all
```

- IPV4 : 4dígitos de 8bits, por lo que puede generar 2 a la 23 direcciones únicas
- IPV6 : Se compone de 8 grupos de 4 dígitos hexadecimales, 2 a la 128

# Configuración de la resolución de nombres

DNS (Domain Name System) 

Base de datos que traduce los nombres de dominio a IP y viceversa.

Componentes:

- Cliente DNS: El que hace la petición
- Servidor DNS: Contesta la petición
- Zonas de autoridad: Servidores encargados de resolver un conjunto de dominios.

1 - El navegador pasa la dirección al cliente DNS
2 - Ese cliente DNS traduce l nombre a una IP
3 - Búscara primero la tabla caché de nuestro equipo
4 - Lanzará la consulta del servidor DNS de nuestro router
5 - Lanzará consulta a uns ervidor DNs fuera de la red

- OpenDNS: Control parental (208.67.222.222)
- Google DNS: Servidores más rapidos (8.8.8.8 8.8.4.4)
- Cloudfare: Ofrece certificado SSL compartido (1.1.1.1)
- Quad9: Oriendtado a la seguridad (9.9.9.9)
- Verisign Public DNS: Segurida de la conexión (64.6.65.6)
- DNS.Watch: Centrado en la velocidad (84.200.69.80)
- AlternateDNS: Filtra anuncion (198.101.242.72)


