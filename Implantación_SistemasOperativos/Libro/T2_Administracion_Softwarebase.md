<h1 align="center"> Administración de software de base </h1>

# Administración de usuarios y grupos locales

Dentro de windows server existe una BD y conjunto de servicios que relacionan recursos del sistema con los usuarios = Active Directory

En un servidor Windows existen cuentas ya preinstaladas y grupos de seguridad.

Grupos AD:

- Grupos de seguridad: Asignación de permisos a los recursos compartidos.
- Grupos de distribución: Creación de listas de distribución para el corrreo.

Los grupos se caracterízan porque definen un ámbito de actuación:

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


