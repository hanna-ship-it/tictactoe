Tic-Tac-Toe (3 en Raya) desarrollado en Java con JSP y Servlets, lo que significa que es una aplicación web que permite a los usuarios jugar en un entorno interactivo a través del navegador.

Estructura del Proyecto

GameBean.java: Contiene la lógica del juego y maneja el estado de la partida.
GameServlet.java: Controlador que gestiona las peticiones del usuario durante el juego.
EntryServlet.java: Controla la entrada del usuario y el inicio de la partida.
Cell.java y Line.java: Clases auxiliares utilizadas para manejar la lógica del tablero y verificar las combinaciones ganadoras.

Frontend (JSP y Archivos Web)

index.jsp: Página de inicio o lobby donde el usuario ingresa su nombre para comenzar la partida.
game.jsp: Interfaz del juego donde los jugadores interactúan con el tablero de 3 en raya.

Configuración y Recursos

webapp/WEB-INF/: Contiene la configuración del servidor.
webapp/img/: Carpeta destinada para almacenar las imágenes utilizadas en la aplicación.

Funcionamiento

El usuario accede a index.jsp, donde ingresa su nombre para iniciar la sesión.
Luego, EntryServlet.java recibe la solicitud y configura la sesión utilizando GameBean.

Posteriormente, game.jsp se encarga de mostrar el tablero del juego y actualizarlo según las acciones del jugador.

Finalmente, GameServlet.java procesa las jugadas realizadas por el usuario, actualiza el estado de la partida y verifica si existe un ganador o si el juego termina en empate.

Características del Juego
	•	Modo Clásico: Juego tradicional de 3 en raya, donde los jugadores deben alinear tres fichas iguales (horizontal, vertical o diagonal) para ganar.
	•	Interfaz en Español: Todos los textos del juego están adaptados al idioma español.
	•	Juego en Web: Implementado con JSP y Servlets, permitiendo jugar directamente desde un navegador.
