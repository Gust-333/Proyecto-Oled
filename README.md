# Proyecto-Oled
Proyecto de PROGRAMACION AVANZADA

Para utilizar poder aprender a utilizar este prollecto ingrece a:
https://thingspeak.mathworks.com/channels/3416289 

En el siguiente link es para pasar de imagen a codigo (esta pagina pertenece a otro creador, yo solo utilizo su pagina para facilitar la creacion de imagen a codigo):
https://javl.github.io/image2cpp/

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
Notificaciones Inteligentes: Ideal para escritorios inteligentes donde se requiera visualizar recordatorios o mensajes rápidos de forma no intrusiva.

Displays Informativos Remotos: Útil para mostrar estados de sensores, mensajes de bienvenida o señalética digital en entornos de oficina o estudio.
