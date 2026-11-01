# Calculadora Basica
Proyecto simple en Java que realiza operaciones matematicas basicas: suma, resta, multiplicacion y division.

Calculadora GPT - Módulo de expansión inteligente ESP32
Descripción del proyecto
La Calculadora GPT es un módulo de expansión inteligente basado en ESP32, diseñado específicamente para las calculadoras TI-84 Plus Silver Edition y TI-84 Plus C Silver Edition.

Mediante modificaciones de hardware, este proyecto incorpora funciones inteligentes modernas a las calculadoras tradicionales, revitalizando estos dispositivos clásicos.

El proyecto utiliza un microcontrolador ESP32 como puente para conectar la calculadora a Internet, permitiendo implementar diversas funciones avanzadas, como conversaciones con asistentes de inteligencia artificial, descarga de programas en línea, visualización de imágenes y chat en tiempo real.

Estas funcionalidades amplían considerablemente las posibilidades de uso de la calculadora.
Características principales
1. Conexión a Internet
- Proporciona conectividad Wi-Fi a la calculadora mediante ESP32.
- Permite la transmisión inalámbrica de datos y la comunicación remota.
- Facilita el acceso en tiempo real a recursos y servicios de Internet.
2. Integración de un asistente de inteligencia artificial
- Integra un asistente GPT con capacidad para mantener conversaciones en lenguaje natural.
- Puede utilizarse para resolver problemas matemáticos, ofrecer apoyo académico y facilitar el aprendizaje.
- Proporciona una experiencia de interacción inteligente.
3. Descarga de programas en línea
- Permite explorar y descargar programas para la calculadora directamente desde Internet.
- Admite diferentes aplicaciones y videojuegos.
- Facilita la ampliación de las funcionalidades de la calculadora sin necesidad de utilizar una computadora.
4. Visualización de imágenes
- Permite visualizar imágenes en la pantalla de la calculadora.
- Puede utilizarse para demostraciones educativas o entretenimiento.
- Incluye adaptación de imágenes para su visualización en blanco y negro.
5. Chat en tiempo real
- Admite salas de conversación con múltiples usuarios.
- Permite enviar y recibir mensajes instantáneamente.
- Puede utilizarse para colaboración en equipo o interacción social.
6. Compatibilidad con cámara (opcional)
- Permite conectar un módulo de cámara externo.
- Admite la captura y el procesamiento de imágenes.
- Amplía las posibilidades de desarrollar aplicaciones relacionadas con visión artificial.
Arquitectura técnica
Calculadora (TI-84) <---> Módulo ESP32 <---> Servidor de Internet
                              |
                              |
                       Funciones locales


La arquitectura del sistema se organiza en cuatro capas:
- Capa de hardware: Microcontrolador ESP32 y placa PCB personalizada.
- Capa de comunicación: Intercambio de información mediante la interfaz de datos de la calculadora.
- Capa de servicios: Servidor backend desarrollado con Node.js.
- Capa de aplicación: Programas ejecutados en la calculadora y API del servidor.
Casos de uso
1. Educación y aprendizaje
- Asistencia mediante inteligencia artificial para resolver problemas y facilitar el aprendizaje.
- Acceso en línea a recursos educativos y programas.
- Aprendizaje colaborativo y trabajo en equipo.
2. Entretenimiento y expansión
- Descarga y ejecución de videojuegos.
- Visualización e intercambio de imágenes.
- Funcionalidades de chat e interacción social.
3. Desarrollo y depuración
- Transferencia remota de programas.
- Intercambio de datos en tiempo real.
- Compatibilidad con procesos de depuración inalámbrica.
Requisitos de hardware
Para implementar este proyecto se necesitan los siguientes componentes:
- Calculadora TI-84 Plus Silver Edition o TI-84 Plus C Silver Edition.
- Placa de desarrollo ESP32.
- Placa PCB personalizada (los archivos de diseño están incluidos en el proyecto).
- Herramientas básicas de soldadura.
Componentes de software
1. Software de la calculadora
Incluye los siguientes elementos:
- Programa de inicio (Launcher).
- Programas correspondientes a los diferentes módulos funcionales.
- Implementación del protocolo de comunicación.
2. Firmware del ESP32
Se encarga de las siguientes funciones:
- Administración de la conexión Wi-Fi.
- Procesamiento y transmisión de datos.
- Comunicación con las API del servidor.
3. Software del servidor
Incluye los siguientes componentes:
- Servicio backend desarrollado con Node.js.
- Integración con la API de GPT.
- Administración de la biblioteca de programas.
- Servicio de mensajería y chat.
Estructura del proyecto
Calculadora-GPT/
├── esp32/                # Código del firmware ESP32
│   └── esp32.ino         # Archivo principal del programa
│
├── server/               # Código del servidor
│   ├── index.mjs         # Punto de entrada del servidor
│   └── routes/           # Rutas de la API
│
├── pcb/                  # Archivos de diseño de PCB
│   └── *.kicad_pcb       # Archivos de diseño KiCad
│
├── programs/             # Programas para la calculadora
│
└── README.md             # Documentación del proyecto


Guía de inicio rápido
Paso 1. Preparación del hardware
Fabricar la placa de circuito impreso siguiendo los archivos de diseño PCB incluidos en el proyecto.
Paso 2. Instalación del firmware
Cargar el firmware correspondiente en la placa de desarrollo ESP32.
Paso 3. Implementación del servidor
Configurar y desplegar el servidor backend desarrollado con Node.js.
Paso 4. Instalación de los programas
Transferir el programa de inicio (Launcher) a la calculadora.
Paso 5. Conexión y funcionamiento
Conectar los componentes de hardware y ejecutar las funciones disponibles.
Guía de contribución
Las contribuciones de la comunidad son bienvenidas.

Puedes participar en el desarrollo del proyecto mediante las siguientes actividades:
- Reportar errores y proponer nuevas funcionalidades.
- Mejorar el código fuente y la documentación.
- Compartir experiencias de uso.
- Diseñar y desarrollar nuevos módulos funcionales.
