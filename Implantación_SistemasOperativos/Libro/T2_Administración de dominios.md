<h1 align="center"> Administración de dominios </h1>

# Estructura cliente-servidor

Se basa en que un equipo pregunta una serie de datos (cliente) y otro le da la información (servidor). La información no tiene por qué estar en el servidor, puede ser una ruta o BD oportunas.

![image](https://github.com/user-attachments/assets/8000113f-e989-4bb6-9b5b-e1d424a8e31f)

Normalmente en una red se centralizan los datos para mejor optimización y prestación. A eso se le llama "sevidor de dedicado" (Sirve única y exclusivamente funciones de servidor)

## Planificación:

- Seguridad en la comunicaciones
- Cantidad de los recursos compartidos
- Jerarquía de permisos de acceso a la información
- Herramientas para acceder a la información, tanto para suadministración como consumo.
- Cantidad de nodos y elementos de la red y su perfil.

## Tipos de servidor:

- Servidor web
- Servidor de BD
- Servidor ficheros/ftp
- Servido de aplicaiones
- Servidor de impresión
- Servidor de DNS
- Servidor de correo/mensajería

# Protocolo LDAP

El protocolo LDAP (Lighweight Directory Access Protocol) posee una estructura cliente-servidor y se utiliza para acceder a servicios de directorios dentro del dominio.

## Funcionalidades:

- Credenciales de usuario: Pueden acceder a los recursos mediante credenciales del sistema.
- Administración centralizada: Centraliza y agrupa la gestión de administración, tanto de usuarios como permisos.
- Búsqueda de información: Funciona como índice referencaindo la información del resto de usuarios.
- Replicación: La BD puede ser replicada, dando la opción de configuración de servidores sincronizados.

En linux podemos instalar el paquete "OpenLDAP"

```
sudo apt-get install slapd ldap-utils
```

# Concepto de dominio, Subdominio. Requisitos

- Dominio: Grupo de ordenadores en un entorno de red administrador por un ordenador principal.
- Controlador de dominio: Ordenador principal encargado en gestionar cuentas, niveles de acceso, recursos, etc.
- Los integrantes del dominio no tienen porque estar en la misma red "física" pero los grupos de trabajo sí.
- Se puede iniciar sesión a cualquier máquina del dominio con las credenciales del mismo.
- En internet, un dominio es la parte principal de la dirección web.

![image](https://github.com/user-attachments/assets/0fbff590-2ec6-4c8f-834e-d305bf458357)

- El subdominio, es la parte que precede al dominio principal de la URL, separado por un punto.

![image](https://github.com/user-attachments/assets/1bef62e8-08d9-43ef-a525-c7f6d66fe605)

# Administración de cuentas

```
Server Manager - Local Server - Active Directory User and computers
```

- Usuario administrador
- Usuario invitado
- Usuario asistente de ayuda

# Contraseñas

Cada usuario tendra su credencial para el sistema. Han de cumplir con estándares de seguridad.

# Cuentas de usuarios y grupos

Las cuentas de los usuarios deben cumplir una serie de normas para que se consideren válidas. 

- El nombre de usuario tendrá una extensión máxima de 20 caracteres.
- Las contraseñas deben ter un mínimo de siete caracteres y combinar mayúscula, minúscula y números.

![image](https://github.com/user-attachments/assets/c3a824cd-adea-4b0f-b0e0-cf60f99485bf)

- No pueden existir nombres de dominio iguales.

# Perfiles móviles y obligatorios

Al ser perfiles locales, en windows sus archivos se guardan en: "C:\Usuarios\nombre"

Sin embargo, existen el "perfil móvil", independientemente de que equipo inicie tendrá ahi los accesos a sus archivos y aplicaciones.

# Carpetas personales

Podemos crear en el servidor un directorio general para cada usuario. 

```
Usuarios y equipos - carpeta particular
```

# Plantillas de usuario

Una plantilla de usuario se utiliza para adjudicar a varios usuarios al mismo tiempo.

Para formalizar una plantilla usaremos la herramienta de "usuarios y equipos" donde crearemos un usario al completo y marcaremos la casilla de desactivar la cuenta, para no tener el perfil activo.

Las variables de entorno forman un conjunto de valores que se ejecutan cada vez que el usuario inicia sesión y que tendrán efecto sobre ciertos comandos y procesos.

```
Administración de qeuipos - Administración de equipo - Propiedades - Opciones avanzados
```

# Administración de grupos

- El uso de grpo nos facilita la gestión de permisos y nos ahorra mucho tiempo de configuración de usuarios.

- Grupos de distribución: Crear listas de distribución de mensajería o e-mail
- Grupos de seguridad: Asignación de permisos a recuros compartidos.

Dentro de un grupo se puede anidar un subgroupo:

Atendiendo el ámbito, podemos diferenciar:

- Ámbito de grupo global: Puede contener usuarios, equipos y grupos globales de su propio dominio. Puede conceder derechos y permisos a los grupos de seguridad global.
- Ámbito de grupo local de dominio: Puede tener grupos universales, globales u otros grupos locales de dominio de su propio dominio. Solo puede otorgar permisos a grupos locales de dominio.
- Ámbito Universal: Puede contener usuarios, equipos, grupos universales y grupos globales de cualquier dominio del bosque.


