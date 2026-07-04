# Proyecto-Oled
Proyecto de PROGRAMACION AVANZADA

En el siguiente link es para pasar de imagen a codigo (esta pagina pertenece a otro creador, yo solo utilizo su pagina para facilitar la creacion de imagen a codigo):
https://javl.github.io/image2cpp/

El siguente link es la APP para conectar son el codigo(Código del ESP32 para la APP): https://drive.google.com/file/d/167dn-2H1FV-rvWf6sbOiXiVNudzZyz39/view?usp=drive_link

El siguiente Link es para Abrir la web para el codigo(Código del ESP32 para la WEB) consejo descargalo luego dale doble clic a ese archivo y se te abrira la web : https://drive.google.com/file/d/1cfFH0-UAaZwPro6RMphaPpI49pbM5bpJ/view?usp=drive_link

# Proyecto-Oled atrabes de la WEB

Resumen del Proyecto
Este proyecto consiste en el desarrollo de una interfaz de control remoto basada en tecnología IoT (Internet of Things), diseñada para gestionar visualmente un módulo de pantalla OLED de 128x64 píxeles mediante un microcontrolador ESP32-38P. El sistema permite a los usuarios interactuar con la pantalla de forma remota a través de una interfaz web, facilitando la publicación de mensajes de texto, el despliegue de imágenes personalizadas en formato mapa de bits y la gestión del estado del dispositivo en tiempo real.

Funcionalidades Clave:

Comunicación en Tiempo Real: Interacción remota sin necesidad de que el usuario esté en la misma red local que el dispositivo.

Protocolo de Comandos Simplificado:

Modo Texto: Renderizado dinámico de mensajes en la pantalla OLED.

Modo Gráfico: Conversión de cadenas hexadecimales en mapas de bits para la visualización de logotipos o iconos de 128x64 píxeles.

Control de Estado: Capacidad de limpieza remota del dispositivo para asegurar una visualización limpia.

Optimización de Recursos: Implementación de consultas no bloqueantes mediante millis() para garantizar que el ESP32 mantenga su estabilidad operativa y no se sature durante el proceso de conexión.

Aplicaciones Prácticas
Notificaciones Inteligentes: Ideal para escritorios inteligentes donde se requiera visualizar recordatorios.

Displays Informativos Remotos: Útil para mostrar estados de sensores, mensajes de bienvenida o señalética digital en entornos de oficina o estudio.



# Informe Técnico: Sistema de Control de Pantalla OLED mediante APP (ESP32)
1. Introducción
El proyecto consiste en un sistema embebido basado en un microcontrolador ESP32 que actúa como un servidor web inalámbrico (punto de acceso), permitiendo a cualquier dispositivo móvil conectarse y controlar visualmente una pantalla OLED de forma remota. El sistema utiliza protocolos de comunicación inalámbrica para recibir comandos de dibujo y renderizarlos en tiempo real.

2. Arquitectura del Sistema
El sistema se divide en tres capas fundamentales:

Capa de Conectividad (Wi-Fi): El ESP32 opera en modo Access Point, creando una red local propia. Esto permite que el teléfono se conecte directamente al dispositivo sin necesidad de un router externo.

Capa de Servidor (HTTP): Se implementa un servidor web ligero que escucha peticiones a través del protocolo HTTP. Los comandos de la aplicación móvil (dibujar puntos o cargar imágenes) llegan como peticiones web que el microcontrolador procesa de forma asíncrona.

Capa de Visualización (I2C): La comunicación con la pantalla OLED se realiza mediante el bus I2C, garantizando una transferencia de datos fluida entre el microcontrolador y el control de la pantalla.
