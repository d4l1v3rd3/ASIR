# Resolución de incidencias y asistencia técnica

## Interpretación, análisis y elaboración de documentación técnica

Si queremos elaborar una guía deberemos valorar una serie de cuestiones:

- Claridad y efectividad: Redacción clara y concisa posible.
- Usuario: Centrarse en el nivel técnico de comprensión del usuario
- Control de versiones: Especificar versión en documentación.
- Recursos gráficos: Incluir diagramas, dibujos, capturas etc.
- F.A.Q : Incluir una sección de preguntar frecuentes o errores
- Glosario: Definición de vocabulario técnico
- Índice de contenido

## Interpretación análisis y elaboración de manuales de instalacion y configuracion de sistemas

Nos centraremos en cómo desarrollar manuales o documentación sobre S.O y/o aplicaciones.

- Control de versiones
- Nivel de usuario
- Integración con terceros
- Grafismo
- Requisitos

## Instalaciones desatendidas

Si tenemos que realizar la misma instalación en multiples equipos. Es por ellos que hemos de configurar instalaciones desatendidas.

En linux:

```
sudo apt-get install system-config-kickstart
```

## Implementación de archivos de respuesta

Hemos de tener en cuenta también los llamados archivos de respuesta, son ficheros que contienen definiciones y valores de configuración usados durante el proceso de instalación

Estos archivos suelen ser .xml "Unattend.xml"

## Servidores de actualizaciones automáticas

![image](https://github.com/user-attachments/assets/737180b5-9162-45ee-8d3c-8f87b5af65bd)

Red de multitud de equipos y estos detectan al mismo tiempo una nueva actualización, todo descargaran al unisono, saturando la red y provocando perdida de datos.

Por ello, se usan mejores soluciones como un servidor de actualizaciones, un ordenador en el que se baja la actualización y después, ya por red local, al resto de los equipos de dominio "Windows Server Update Services (WSUS)"

## Partes de incidencias y protocolos de actuación

Incidencia : Evento o acción que supone un contratiempo en el deasrrolo normal de la productividad del usuario.

- Conocidads
- Desconocidas

### Documentación

- Clasificar incidencias
- Investigar y encontrar posibles diagnósticos y soluciones
- Resolución de la incidencia y restablecimiento del servicio
- Guardado de la incidencia en el registro o histórico
- Fecha y hora
- Equipo en el que se ha producido
- Software instalado en el equipo
- Requisitos de hardware del equipo

## Administración Remota

Poder tomar el control del ordenador del usuario para resolver una incidencia.

Windows incorporta la conexión a escritorio remoto (RDP) 

### Team VIewer

### AnyDesk


