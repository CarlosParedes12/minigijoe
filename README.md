Este programa combina el uso de la cámara web con las bibliotecas OpenCV, MediaPipe 
y NumPy para crear una experiencia interactiva que permite dibujar en la pantalla 
usando el dedo índice y también mover un objeto virtual mediante gestos con la mano. 
El sistema detecta la mano utilizando MediaPipe y rastrea los puntos clave de los 
dedos, en especial la punta del dedo índice y del pulgar. Cuando ambos están muy 
cerca, se interpreta como un gesto de agarre, 
que activa el modo de dibujo o el movimiento del objeto.

Cuando el usuario junta el índice y el pulgar, el sistema comienza a dibujar una
línea roja que sigue la trayectoria del dedo por la pantalla. Si se separan, el dibujo se
detiene. Además, hay dos botones virtuales en pantalla: uno para guardar el 
dibujo (que guarda la imagen como drawing.png con fondo blanco), y otro para borrar
lo dibujado. Si el dedo índice se posiciona sobre estas zonas, el programa lo
detecta como si fuera un clic real.

Además del dibujo, se incorpora un objeto circular azul virtual, que se puede 
mover con el mismo gesto de agarre. Si se detecta este gesto cerca del objeto, este empieza
a seguir la mano y se detiene cuando el gesto desaparece. Todo se muestra en una ventana
a pantalla completa, haciendo que la experiencia sea visualmente inmersiva y fácil 
de usar sin contacto físico.
