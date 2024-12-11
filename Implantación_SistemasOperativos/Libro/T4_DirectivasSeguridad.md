# Directivas de seguridad y auditorías

## Requisitos de seguridad del sitema y de los datos

Normas que deben cumplir la seguridad

- Disponibilidad: Información debe estar mas que disponible si no que debe existi algún mecanismo por el cual podamos recuperar
- Integridad: Información que ha sido generada, transmitida, recibida y procesada no ha sido alterada en ningún momento.
- Confidencialidad: Información solo debe ser manejada por aquellos que necesitan pconocer para desarrollar el trabajo.

Requisitos del administrador

- Segmentación de funciones: No acumular excesivos permisos en pocos usuarios.
- Accesos y privilegios: Mantener una politica de privilegios mínimos y accesos cerrados por defecto
- Formación: Culturalizar a las empresas.
- Auditorias: Periodicamente por parte de un tercero.

## Derechos de usuario

Permisos y derechos

- Permisos: Aplican a los recuros (ficheros, carpetas, archivos, etc.) hacen referencia a las restricciones qu pueden tener a la hora de ser ejecutados (autorizar o denegar)
- Derechos: Se aplican a los usuarios y determina que acciones pueden hacer dentro del sistema.

- Directivas de seguridad local
- Directivas de seguridad de dominio
- Directivas de seguridad del controlador de dominio

## Directivas de seguridad Local

Conjunto de reglas que se han de utilizar para la modificación de la configuración de seguridad de un sistema informático, siempre y cuando este sistema no tenga instalada una distribución de WIndows Server. O tampoco Active Directory.

Al no actuar como controlador de dominio, el equipo deberña configurar de manera aislada.

```
secpol.msc

Panel de control / Sistema y seguridad / Herramientas administrativas
```

Configuración:

- Orientadas al registro de eventos de seguridad
- Encargasdas en especificar los grupos o usuarios que pueden o no iniciar sesión
- Relativas a la seguridad, definiendo nombres.

## Orden de aplicación de las directivas

Ordens que deben seguir

![image](https://github.com/user-attachments/assets/25df5cd5-5e86-4896-ad75-c53ac418ad0f)

Podemos aislar cada tipo de directiva

- Directivas de seguridad local
- Directivas de usuario local
- Directiva de grupo del sitio
- Directiva de grupo del dominio.
- Directiva de grupo de la UO (Unidad organizativa)
- Directiva de grupo del controlador de dominio.

## Conjunto resultante de las directivas

Se le conoce como RSop (Resultant Set of Policy) permite elaborar informes sobre los distintos parámetros y valores de las directivas de grupo (GPO) que se han aplicado a un usuario o grupo de usuarios. 

Acceder a ella:

```
Windows + R
rsop.msc
gpresult /Scope User /v
```

![image](https://github.com/user-attachments/assets/6b33687d-1b0a-44a3-9b85-a31b5efa268e)

## Opciones avanzadas en la aplicación de directivas

Acceder a editor

```
Windows + R
gpedit.msc
gpupdate /force
```

![image](https://github.com/user-attachments/assets/1d6e58c3-bc52-4288-95f0-f9f734ffc8c5)

![image](https://github.com/user-attachments/assets/c88a5d92-973b-4d49-ae69-998a41d5cee3)

## Registros del sistema operativo

Se guardan datos como:

- Ajustes del sistema
- Dispostiivos de hardware presentes
- Preferencias y configuraciones propias del usuario
- Información y configuración del sistmma operativo
- Tipos de documentos que una aplicación puede genrar
- Instrucciones y rutas de carpetas de aplicaciones
- Etc.

Accedemos a una ventana y veremos categorías

- Root
- Usuario actual
- Máquina
- Usuarios
- Configuración

## Objetivos de la auditoría

Es una de las herramientas más útiles que se pueden manejar para tener controlada la integridad del sistema.

## Ámbito de la auditoría. Aspectos auditables

Cada auditoría dependerá de qué certificación o qué aspectos necesita la empresa que se va auditar.

A quién va realizada:

- Auditorías internas
- Auditorías externas

Metodología:

- Auditorias basadas en el cumplimiento o algún estándar
- Auditorías técnicas, basadan en revisión de los sistemas informáticos, equipos y bases de datos

Objetivo:

- Auditoría sobre aplicaciones y software

Metodologías:

- SAST: Analiza el código fuente de las apliaciones en busca de vulnerabilidades
- DAST: En directo mientras se usan las aplicaciones, para evaluar tráfico y uso de escenario real.

Objetivo: 

- Control de accesos: Dispositivos tecnológicos físicos que velan por la seguridad.
- Auditoría fonrense: Cuándo ha habido una incidencia como pérdida o hackero
- Hacking ético: Centrada en medir el nivel de seguridad

## Mecanismos de auditoría: Alarmas y acciones correctivas

1 - Toma de contacto con el sistema
2 - Análisis de recursos y transacciones
3 - Determinación del alcance del riesgo
4 - Análisis y examen de controles
5 - Informe de auditoría
6 - Seguimiento de las recomendaciones

Acciones 

- Acción Preventiva : Previene
- Acción Correctiva: Arregla una incidencia ya hecho

## Información de registro de auditoría

Cuales han sido os pasos para llegar hasta la incidencia o no. Registro de acciones.

## Técnicas y herramientas de auditoría

Herramientas, distribuciones, etc.

Linux, ARCH Linux

- Análisis de vulnerabilidades
- Análisis de aplicaciones web
- Evaluación de bases de datos
- Evaluación de robustez de contraseñas
- Pruebas de seguridad wireless/bluetooth
- Captura de tramas y análisis de encriptación
- Ingeniería Inversa

Programsa que podemos destacar:

- Dradis Framework: Permite almacenar y compartir información relacionada con los resultados de una prueba de penetración
- MagicTree: Software de penetración y productividad de hacking ético
- Faraday: Programa de catalogo como IPTE y permite indexar, distribuir y analizar los datos generador durante una auditoría de seguridad

## Informes de auditoría

Estructura del informe

- Título
- Índice general
- Memoria : Descripción en forma clasa y concisa del informe, con soluciones.
- Anexos: Documentos o justificaciones

Portada:

- Número del documento
- Título del informe
- Tipo de documento
- Organismo
- Identificación y datos profesionales
- Fecha y lugar

![image](https://github.com/user-attachments/assets/487b8191-2143-48af-8e65-b48d26700333)

![image](https://github.com/user-attachments/assets/9fff7058-6329-4b2f-993d-8e1dc161dfee)



