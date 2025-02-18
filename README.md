# ProyectoUnity

## Preparación y Prototipado Inicial
Definir el alcance del MVP:

 - Lista de funcionalidades mínimas.

Encontrar un numero de objeto y traerlo a un lugar.
 - Esbozar un mapa o boceto del entorno del IES Haría que se recreará.

La aula pero las plataforma sera objetos de clase desordenado y sin gravedad.
 - Configuración del repositorio Git; Crear el repositorio y la estructura base del proyecto Unity.

Hecho
 - Primer commit con la configuración inicial.

Hecho
 - Prototipo básico:
Implementar el movimiento del jugador y la cámara en tercera persona en un entorno simple (por ejemplo, un plano).

## Problemas y soluciones

- Salto infinito

La acción de saltar se podía realizar sin límite y la idea era un solo salto. Se solucionó con poner etiquetas.

- Obtener objetivo y salir del nivel.

Ahora tenemos un player que se mueve, pero no puedes conseguir la llave para salir por la puerta al siguiente nivel. Se solucionó poniendo etiquetas, pero tenías que crear varias para cada acción (Salta, Recogida y Salida).

 - Las trampas

Las trampas no hacían nada y se arregló usando también etiquetas y añadiendo un sistema de vidas, que cada colisión con un objeto con la etiqueta 'trampa' quite una de vida y mueva al jugador al spawn.

- La puerta

La puerta o el final del nivel no hacía nada y lo cambiamos para que, cuando colisiones y hayas colisionado anteriormente con la llave, te lleve a la siguiente escena.

 - Cambio de escena

Para el cambio de escena se usa un sceneloder, pero eso se ajustaba en bild setting, el cual no salía. Para arreglarlo, hicimos una lista de coordenadas para que en vez de cambiar de escena , hagamos todos los niveles en la misma escena.

Más tarde, al intentar exportar la app, se encontró el ajuste de Build para pasar por escenas y se pudo cambiar todo para tener escenas distintas.

- Mapa sin tilemap

Al principio buscaba crear un nuevo tilemap, pero todos los videos son de descargar y, usando lo descargado, crear el mapa. Al final se pudo averiguar cómo hacerlo al descargar un tilemap ya creado de internet.

- Cambio de escena infinito

El proyecto tiene que parar para cambiar de escena y recoger el número de escena actual y añadir uno, pero en el último nivel no tendrá sentido. Se puso una pantalla de fin que te deja salir del juego y empezar de nuevo.
