## Crítica: *Item-Based Collaborative Filtering Recommendation Algorithms*

El *paper* describe dos metodologías de filtrado colaborativo. Primero, explica que los algoritmos *memory-based* utilizan toda la base de datos.Se basan en encontarar a los usuarios que sean más parecedios al usuario activo y según las preferencias de estos se genera la recomendación. 
Segundo, los algritmos *model-based* consideran que el proceso de filtrado corresponde a calcular el valor esperado de una predicción del usuario según los *ratings* que le ha otorgado a otros objetos. 

Los autores comentaron en la sección 3.1.3 que la similud ajustada del coseno era una mejor métrica que *cosine-based similarity* porque consideraba las diferencias en las escalas de calificación entre los usuarios. Esto me pareció interesante porque en las pruebas que realizaron se muestra que la similitud ajustada del coseno tuvo un mejor desempeño.

También explican que en su metodología propuesta ellos sólo van a calcular los k ítemes más parecidos con k << n. Pero, me gustaría saber que sucede si los usuarios ingresan nuevas preferencias ya que esto podría modificar la lista de los objetos más similares. ¿Habría que volver a calcular los k objetos más cercanos cada vez que un usuario agrega un *rating* o esperar a que varios usuarios hayan añadido nuevos *ratings*?

No me pareció adecuado que no explicasen por qué sólo consideraron los usuarios que habían calificado más de 20 películas en su set de datos. ¿Qué sucede con los usuarios que no cumplen con ese criterio?

Tampoco indican por qué utilizan el *rating* que le dan los usuarios a los ítemes para calcular la similitud entre estos. Tal vez, podrían haber considerado otros factores como las descripciones de estos. 


