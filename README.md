# Manejo de Pantalla y Teclado

El laboratorio implementa tres programas en ensamblador x86 con NASM que utilizan las interrupciones INT 21h e INT 10h para controlar la salida de texto en pantalla, la posición del cursor y los atributos de color en modo texto, ejecutados en DOSBox.


Programas:

post1.asm: Salida básica de texto con INT 21h / AH=09h. Imprime tres cadenas en pantalla.

post1b.asm: Control de cursor y color con INT 10h. Muestra "A" en amarillo sobre azul (fila 2) y "U7" en rojo claro sobre negro (fila 3), con limpieza previa de pantalla.

post1c.asm: Escritura de cadena en posición exacta. Recorre carácter por carácter el título "UNIDAD 7 - PANTALLA Y TECLADO" y lo imprime centrado en la fila 5 con color verde brillante.

Compilación y ejecución en DOSBox:

- nasm -f bin post1.asm -o post1.com
- post1.com

- Reemplazar post1 por post1b o post1c según el programa a ejecutar.
