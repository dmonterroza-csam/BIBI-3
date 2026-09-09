# BIBI-3
# Guía de Documentación: Estructura Mínima para un README.md

Un archivo `README.md` es la pieza fundamental de documentación en cualquier repositorio de GitHub. Su función principal es actuar como la portada de presentación del proyecto, proporcionando contexto inmediato a desarrolladores, reclutadores o usuarios sobre qué hace la aplicación y cómo utilizarla.

---

## Secciones y Contenidos Mínimos

### 1. Título del Proyecto y Descripción Corta
* **Título:** BIBI - Food Delivery Bot
* **Descripción:** Carrito robot móvil y autónomo diseñado para la distribución y entrega optimizada de almuerzos en entornos locales.

---

### 2. Tecnologías y Herramientas Utilizadas
Para la arquitectura física, la gestión del hardware y la interfaz de usuario, se integró el siguiente ecosistema tecnológico:

* **Hardware y Componentes Electrónicos:**
  * **Unidad de Control:** ESP32 NodeMCU con conectividad Wi-Fi integrada.
  * **Sistema de Tracción:** Motores de corriente continua con controlador L298N y servos de alta precisión.
  * **Módulos de Proximidad:** Sensores de ultrasonido HC-SR04 y arreglos infrarrojos para seguimiento de trayectoria.
  * **Gestión de Energía:** Sistema de baterías Li-Ion de 12V con módulo regulador de tensión Step-Down LM2596.
  * **Interfaz de Control Físico:** Botón integrado para activación y conmutación manual de estados.

* **Firmware del Dispositivo:**
  * **C / C++ (Entorno Arduino / ESP-IDF):** Código optimizado para la gestión de interrupciones, lectura de telemetría, detección de pulsaciones de botón y control PWM de propulsión del carrito.

* **Panel de Control y Monitoreo (Frontend):**
  * **HTML5:** Estructuración modular para la interfaz de mando.
  * **CSS3:** Estilos adaptativos con diseño UI/UX enfocado en dispositivos móviles.
  * **JavaScript (ES6+):** Interacción asíncrona vía Fetch API y WebSockets para el envío inmediato de instrucciones.

* **Herramientas de Entorno:**
  * Git, GitHub, Visual Studio Code y Fritzing (para esquemáticos electrónicos).

---

### 3. Características Principales y Estructura del Proyecto

#### Características Principales
* **Activación por Botón e Interfaz Web:** Inicio de operaciones mediante botón físico en el carrito y dashboard en vivo para operar el desplazamiento mediante protocolo HTTP/Wi-Fi.
* **Modo de Evitación Automática:** Algoritmo de detección de colisiones e interrupción de ruta en presencia de obstáculos.
* **Panel de Métricas en Vivo:** Monitoreo constante de lecturas de proximidad y estado del enlace inalámbrico.
* **Diseño UI Adaptativo:** Interfaz accesible desde cualquier navegador móvil o de escritorio.

---

### 4. Instrucciones de Instalación y Configuración Local

Sigue esta guía para desplegar el firmware e iniciar la interfaz de gestión del carrito:

#### Requisitos Previos
* [Arduino IDE](https://www.arduino.cc/en/software) configurado con el soporte para tarjetas ESP32.
* Controladores de puerto serie **CP210x / CH340** instalados.
* Extensión **Live Server** en Visual Studio Code (o cualquier servidor web local).

#### Paso a Paso

1. **Clonar este repositorio:**
   ```bash
   git clone [https://github.com/tu-usuario/bibi-delivery-bot.git](https://github.com/tu-usuario/bibi-delivery-bot.git)
   cd bibi-delivery-bot

