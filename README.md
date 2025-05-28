Project Shooter Python Start II
¡Bienvenido a "Project Shooter Python Start II"! Este es un juego simple de disparos espaciales desarrollado con Pygame. Tu objetivo es derribar naves enemigas y evitar los asteroides mientras intentas sobrevivir y alcanzar la victoria.

Características
Control de la nave espacial del jugador.
Enemigos que se mueven y reaparecen.
Sistema de puntuación por enemigos destruidos.
Contador de enemigos perdidos.
Sistema de recarga de balas.
Música de fondo y efectos de sonido.
Pantallas de "VICTORY" y "GAME OVER".
Requisitos
Asegúrate de tener Python 3.x instalado en tu sistema.

Este juego requiere la librería pygame. Puedes instalarla usando pip:

Bash

pip install pygame
Estructura de Archivos
Para que el juego funcione correctamente, debes tener los siguientes archivos en la misma carpeta que main.py:

.
├── main.py
├── space.ogg         # Música de fondo
├── fire.ogg          # Efecto de sonido de disparo
├── galaxy.jpg        # Imagen de fondo
├── rocket.png        # Imagen de la nave del jugador
├── ufo.png           # Imagen de la nave enemiga
├── asteroid.png      # Imagen del asteroide
└── bullet.png        # Imagen de la bala
Cómo Jugar
Guarda el código de main.py y todas las imágenes y archivos de sonido (listados arriba) en la misma carpeta.

Abre una terminal o línea de comandos.

Navega a la carpeta donde guardaste los archivos.

Ejecuta el juego usando el siguiente comando:

Bash

python main.py
Controles
Flecha Izquierda (←): Mueve la nave del jugador hacia la izquierda.
Flecha Derecha (→): Mueve la nave del jugador hacia la derecha.
Espacio (Spacebar): Dispara balas.
Objetivo del Juego
Destruye 20 naves enemigas para ganar.
Si 5 naves enemigas pasan la pantalla o tu nave choca con un enemigo/asteroide, es "GAME OVER".
Desarrollo
El juego está estructurado con las siguientes clases principales:

GameSprite: Una clase base para todos los elementos del juego (jugador, enemigos, balas, asteroides). Maneja la carga de imágenes, posicionamiento y redibujado.
Player: Hereda de GameSprite y añade la lógica de movimiento del jugador y el método de disparo.
Enemy: Hereda de GameSprite y maneja el movimiento de los enemigos, su reaparición y el seguimiento de los enemigos perdidos.
Bullet: Hereda de GameSprite y gestiona el movimiento de las balas y su desaparición una vez que salen de la pantalla.
El bucle principal del juego maneja la detección de eventos, la actualización del estado del juego (movimiento, colisiones), la recarga de balas y el renderizado en pantalla.

¡Diviértete jugando a "Project Shooter Python Start II"!
