# Crítica: *See What You Want to See: Visual User-Driven Approach for Hybrid Recommendation*

Los autores se enfocan en la controlabilidad del usuario sobre el proceso de recomendación híbrida de charlas de conferencias. Para esto desarrollaron una interfaz que le permite a los usuarios combinar manualmente las recomendaciones de diversos modelos. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, es interesante que loa autores no se hayan enfocado en la evaluación de los sistemas de acuerdo a métricas matemáticas, ya que al preferir los estudios de usuario (*user studies*) pueden observar cómo interactúa con el sistema recomendador y recolectar información cuantitativa como el tiempo que utilizaron el sistema.

Segundo, es novedoso que el sistema permita que los usuarios interactúen directamente con él. Esto permite que el usuario modifique el sistema recomendador a su preferencia y que al participar directamente perciba que el mecanismo de recomendación es más transparente.

Tercero, considero que el diagrama de Venn fue una buena herramienta para mostrar los *papers* que han sido recomendados por cada método, ya que es una visualización simple de entender e intuitiva para el usuario.

Cuarto, siento que faltó que la interfaz explicase el orden de las recomendaciones. Por ejemplo, en la Figura 1, se ve que:
* en segundo lugar está un *paper* que fue recomendado por los filtros que tienen un peso igual a 0.4 cada uno. En cambio, en la tercera posición está un trabajo que fue seleccionado por recomendadores, cuyos pesos son 0.4 y 0.6.


Entonces, no queda claro cómo ordena a los *papers*, debido a que intuitivamente esperaba que estuviesen más arriba los textos que son recomendados por filtros a los que se les asignaron un mayor peso. 

Quinto, mencionan que con la interfaz los usuarios agregaron más textos a sus listas de favoritos (*bookmarked*). No obstante, esto no indica si efectivamente las recomendaciones fueron más útiles para los usuarios. 

Finalmente, los autores exploran cómo afecta la interacción humana en el proceso de filtrado al desarrollar una interfaz que les permite combinar manualmente las recomendaciones de diversos modelos.
