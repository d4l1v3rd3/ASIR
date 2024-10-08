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

