# Taller de IA: Creando un Videojuego con Gemini

Este repositorio contiene todos los archivos de recursos (*assets*) necesarios para crear un videojuego completo de estilo "Flappy Bird" utilizando HTML, CSS, y JavaScript con la ayuda de un modelo de IA como Google Gemini.

## Descripción del Proyecto

El objetivo es construir un juego funcional donde el jugador controla un pájaro animado que debe volar a través de una serie de tuberías verdes sin chocar. El juego incluye animaciones, efectos de sonido para cada acción y un sistema de puntuación visual basado en imágenes.

## Descripción de los Archivos de Recursos (`Assets`)

A continuación se detalla el propósito de cada archivo en este repositorio.

### Imágenes (PNG)

* **`background-day.png`**: La imagen de fondo principal para el escenario del juego.
* **`base.png`**: La imagen del suelo. Se desplazará por la parte inferior de la pantalla. El juego terminará si el pájaro la toca.
* **`pipe-green.png`**: La imagen para los obstáculos (las tuberías). Se usará tanto para la tubería inferior como para la superior (invertida).
* **`yellowbird-upflap.png`, `yellowbird-midflap.png`, `yellowbird-downflap.png`**: Son los tres fotogramas (frames) que componen la animación del aleteo del pájaro. El código deberá alternar entre estas tres imágenes para que el pájaro parezca que está volando.
* **`message.png`**: Una imagen de bienvenida o de instrucciones, como "Get Ready!", que se muestra al inicio del juego antes de que comience la acción.
* **`gameover.png`**: La imagen que se muestra en pantalla cuando la partida termina.
* **`0.png` a `9.png`**: Un conjunto de imágenes para cada dígito. Se usarán para dibujar la puntuación en la pantalla, en lugar de usar texto plano.

### Sonidos (OGG)

* **`wing.ogg`**: El efecto de sonido que se reproducirá cada vez que el pájaro aletee o salte.
* **`swoosh.ogg`**: Un sonido de transición, ideal para usar al iniciar el juego o en los menús.
* **`point.ogg`**: El efecto de sonido que se reproducirá cada vez que el jugador gane un punto al pasar entre las tuberías.
* **`hit.ogg`**: El efecto de sonido del impacto, que se reproducirá justo cuando el pájaro choque contra una tubería o el suelo.
* **`die.ogg`**: Un efecto de sonido que se reproduce justo después del impacto (`hit.ogg`), cuando el pájaro cae y la partida termina.

Actúa como un programador experto en desarrollo de videojuegos web. Tu tarea es crear un juego funcional y completo estilo "Flappy Bird" usando HTML, CSS y JavaScript.

Utiliza la siguiente lista de archivos de recursos (assets) que están alojados en GitHub. Es crucial que uses estas URLs exactas en el código para cargar todas las imágenes y los sonidos.

**Assets del Juego:**
- Fondo: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/background-day.png`
- Suelo/Base: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/base.png`
- Tubería: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/pipe-green.png`
- Pájaro (frame 1): `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/yellowbird-upflap.png`
- Pájaro (frame 2): `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/yellowbird-midflap.png`
- Pájaro (frame 3): `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/yellowbird-downflap.png`
- Mensaje de inicio: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/message.png`
- Fin del juego: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/gameover.png`
- Números para el score (del 0 al 9): `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/0.png` (y así sucesivamente hasta 9.png)

- Sonido de aleteo: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/wing.ogg`
- Sonido de punto: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/point.ogg`
- Sonido de choque: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/hit.ogg`
- Sonido de muerte: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/die.ogg`
- Sonido de transición: `https://raw.githubusercontent.com/morenoemanuel/AltrusaTallerAIParte2/main/swoosh.ogg`

**Requisitos Funcionales Detallados:**
1.  **Estado Inicial:** Al cargar, muestra la imagen `message.png`. El juego comienza con el primer clic o al presionar la barra espaciadora.
2.  **Animación del Pájaro:** El pájaro debe tener una animación de aleteo constante, ciclando entre los tres frames (`yellowbird-upflap`, `midflap`, `downflap`).
3.  **Control y Sonido:** El pájaro cae por gravedad. Al hacer clic o presionar la barra espaciadora, el pájaro debe saltar y se debe reproducir el sonido `wing.ogg`.
4.  **Movimiento de Escenario:** El fondo (`background-day.png`) y el suelo (`base.png`) deben moverse continuamente de derecha a izquierda.
5.  **Obstáculos:** Las tuberías (`pipe-green.png`) deben generarse a intervalos regulares desde la derecha y moverse hacia la izquierda.
6.  **Puntuación:** La puntuación debe mostrarse en pantalla usando las imágenes de los números (de `0.png` a `9.png`). Cada vez que el pájaro pase un par de tuberías, la puntuación aumenta en 1 y se reproduce el sonido `point.ogg`.
7.  **Colisión y Fin de Juego:** El juego termina si el pájaro choca con una tubería o con el suelo (`base.png`). Al chocar, se debe reproducir primero el sonido `hit.ogg` y luego `die.ogg`. El juego se detiene y se muestra la imagen `gameover.png`.

**Formato de la Respuesta:**
Proporciona el código en tres bloques separados y claramente etiquetados para los archivos `index.html`, `style.css`, y `script.js`. Añade comentarios en el código JavaScript para explicar las partes clave como la animación del pájaro, el sistema de puntuación con imágenes y la lógica de los estados del juego.
