Documentación del Juego "Batalla Naval"
Alejandro Mendoza, Valentina Ceron, Saray Rincon, Juan Felipe Castro
Descripción General
Este código implementa una versión simple del juego "Batalla Naval", en la que un jugador puede jugar contra la computadora o contra otro jugador. El juego se desarrolla en un tablero de 5x5, donde los jugadores deben colocar sus barcos y luego intentar hundir los barcos del oponente disparando a las posiciones en el tablero.
Estructura del Código
1. Creación de Tableros
crearTablero(tamano): Crea un tablero de tamaño tamano x tamano (en este caso 5x5) lleno de símbolos "~" que representan agua.
mostrarTableros(tableroDisparosJugador, tableroDisparosOponente): Muestra los tableros de disparos del jugador y del oponente.
2. Colocación de Barcos
colocarBarcos(tablero, barcos, jugador): Coloca los barcos en el tablero. El jugador elige la posición y la orientación, mientras que para la computadora, las posiciones son generadas aleatoriamente.
validarColocacion(tablero, fila, columna, tamano, orientacion): Valida si un barco puede colocarse en una posición específica del tablero.
colocarBarco(tablero, fila, columna, tamano, orientacion): Coloca un barco en el tablero en la posición validada.
3. Sistema de Combate
realizarDisparo(tableroOculto, tableroDisparos, fila, columna): Realiza un disparo en el tablero del oponente. Si impacta en un barco, marca "X"; si no, marca "O".
verificarVictoria(tableroOculto): Verifica si todos los barcos del oponente han sido hundidos.
4. Modos de Juego
jugarContraComputadora(): Permite al jugador jugar contra la computadora.
jugarDosJugadores(): Permite que dos jugadores jueguen entre sí, turnándose para disparar.
5. Menú y Flujo del Juego
mostrarMenu(): Muestra el menú principal con opciones para elegir el modo de juego.
iniciarJuego(): Controla el flujo principal del juego, permitiendo al jugador elegir el modo de juego y si desea jugar nuevamente.
Cómo Jugar
Inicio: Al iniciar el juego, se presenta un menú con tres opciones:
1. Juega contra la computadora: Jugarás una partida contra la computadora.
2. Dos Jugadores: Dos jugadores se turnarán para jugar en el mismo dispositivo.
3. Salir: Finaliza el juego.
Colocación de Barcos:
El jugador debe colocar sus barcos (un portaaviones de tamaño 3 y un submarino de tamaño 2) en el tablero ingresando las coordenadas de la fila y columna, así como la orientación (horizontal 'h' o vertical 'v').
La computadora colocará sus barcos automáticamente.
Disparos:
Los jugadores se turnan para disparar a una posición en el tablero del oponente, ingresando las coordenadas de fila y columna.
El tablero mostrará "X" si el disparo impacta en un barco, "O" si cae en el agua, y un mensaje si ya disparaste en esa posición.
Victoria:
El juego termina cuando un jugador hunde todos los barcos del oponente. Se declara un ganador y se pregunta si desea jugar de nuevo.
