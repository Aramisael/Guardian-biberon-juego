# **🍼 MR.BIBERÓN 3.0: Guardián del Biberón**

¡Bienvenido al código fuente de MR.BIBERÓN 3.0, un juego arcade de supervivencia desarrollado en una sola página HTML\! El objetivo es simple: sobrevivir el mayor tiempo posible y conseguir la mayor puntuación atrapando biberones y esquivando peligros.

Este proyecto fue desarrollado íntegramente en el entorno de Canvas, utilizando **Vanilla JavaScript**, **HTML5**, **CSS (Tailwind)** y **Firebase Firestore** para la gestión de las puntuaciones altas.

## **🕹️ Cómo Jugar**

1. **Objetivo:** Atrapa los **🍼 Biberones** para aumentar tu puntuación y tu racha de aciertos. Evita las **💥 Explosiones** o perderás una vida (paquete).  
2. **Controles:**  
   * **Escritorio:** Flechas Izquierda/Derecha.  
   * **Móvil:** Desliza (Swipe) a la izquierda/derecha.  
3. **Vidas:** Tienes **3 📦 Paquetes** de vida. Al perder el último, se activa un "PEDIDO DE EXPLICACIÓN".

## **🚀 Características Clave**

### **Modo Don Hugo (Modo Dios)**

Al alcanzar una racha de **10 biberones** consecutivos, se activa el "Modo Don Hugo". Durante este tiempo, no pierdes vidas al chocar con explosiones y tu multiplicador de puntos aumenta hasta **x4**.

### **Sistema de Puntuación Alta**

El juego utiliza **Firebase Firestore** para almacenar las puntuaciones de los jugadores en una base de datos pública. Esto permite que los *betatesters* y otros usuarios compitan en el **"TOP 3 MAMADERAS"** en tiempo real.

### **Pedido de Explicación**

Cuando pierdes la última vida, el juego se detiene y te presenta un "PEDIDO DE EXPLICACIÓN ACTIVO" con una frase aleatoria. Debes ingresar un alias y pulsar **"✍️ Firmar y Registrar"** para guardar tu puntuación y finalizar la sesión.

## **⚙️ Estructura del Proyecto**

El juego está contenido en un **único archivo HTML** (mr\_biberon\_3\_0.html) que incluye:

* **HTML:** Estructura del juego y UI.  
* **CSS:** Estilizado mediante clases de **Tailwind CSS** y estilos personalizados (fuente 'Orbitron', efectos retro/glitch).  
* **JavaScript (Módulo):** Lógica del juego, manejo de colisiones, bucle de animación (requestAnimationFrame), y toda la integración con **Firebase v11.6.1**.

## **🛠️ Instalación y Ejecución**

Al ser un proyecto de un solo archivo, la instalación es trivial:

1. Clona o descarga este repositorio.  
2. Abre el archivo mr\_biberon\_3\_0.html en cualquier navegador web moderno.  
3. **Nota sobre Firebase:** En un entorno de desarrollo normal, necesitarías configurar un archivo de configuración de Firebase; sin embargo, en el entorno donde se desarrolló este código, las claves de configuración y autenticación inicial son inyectadas automáticamente.