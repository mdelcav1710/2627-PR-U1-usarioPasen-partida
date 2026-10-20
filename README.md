Desarrolla un programa que lea el número de aciertos y de errores obtenidos en un juego de preguntas.\ Cada acierto suma 3 puntos y cada error resta 1 punto.

Constantes

Declara a nivel de módulo las constantes correspondientes a los puntos por acierto y la penalización por error.

Crea también la constante VALORACION_PARTIDA, una tupla de tres posiciones con estos textos, en este orden:

("Sigue practicando", "Buen resultado", "Excelente")
Funciones que debes implementar

calcular_resultados(aciertos, errores): devuelve una tupla con el número total de preguntas respondidas y la puntuación obtenida, en ese orden.\
valorar_partida(puntuacion): devuelve un número entero que indica la posición del mensaje que se debe mostrar de VALORACION_PARTIDA:\
0 si la puntuación es inferior a 10.\
1 si está entre 10 y 19, ambos incluidos.\
2 si es de 20 o más.\
La función main() debe leer y convertir los dos datos a enteros.\

Si los aciertos o los errores son negativos, el programa debe mostrar únicamente este mensaje y finalizar, sin llamar a las funciones auxiliares:

ERROR - valores incorrectos\
Si ambos valores son válidos, main() llamará a las dos funciones, desempaquetará la tupla de resultados y utilizará el índice devuelto por valorar_partida() para acceder al mensaje correspondiente de VALORACION_PARTIDA.

Una partida con cero preguntas respondidas es válida.\ La puntuación final puede ser negativa.

Entrada y salida

Lee primero los aciertos y después los errores, en líneas separadas y sin imprimir mensajes para solicitar los datos.\ Puedes suponer que ambas entradas tienen un formato de número entero válido.

Con esta entrada:

6\
2\
La salida debe ser:

Preguntas respondidas: 8\
Puntuación: 16\
Valoración: Buen resultado