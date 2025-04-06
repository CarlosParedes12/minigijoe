Este proyecto combina el uso de la cámara web con las bibliotecas OpenCV, MediaPipe 
y NumPy la lectura de movimientos con nuestra mano la cual permitira ya sea el movimiento
de una pelota o el dibujo a mano alzada desde la pantalla. 
El sistema detecta la mano utilizando MediaPipe y rastrea los puntos clave de los 
dedos, en especial la punta del dedo indice y del pulgar. Se utiliza el momento en el que se
detecta una union entre el indice y el pulgar para el dibujo o bien el movimiento de la 
pelota.

Cuando el usuario junta el índice y el pulgar, el sistema comienza a dibujar una
línea roja que sigue la trayectoria del dedo por la pantalla. Si se separan, el dibujo se
detiene. Además del dibujo, se incorpora un objeto circular azul que se puede 
mover con el mismo gesto de agarre. Si se detecta este gesto cerca del objeto, este empieza
a seguir la mano y se detiene cuando el gesto desaparece. Todo se muestra en una ventana
a pantalla completa, haciendo que la experiencia sea visualmente inmersiva y fácil 
de usar sin contacto físico.
