## Crítica: *Item-Based Collaborative Filtering Recommendation Algorithms*

El *paper* describe dos metodologías de filtrado colaborativo. Primero, explica que los algoritmos *memory-based* utilizan toda la base de datos.Se basan en encontarar a los usuarios que sean más parecedios al usuario activo y según las preferencias de estos se genera la recomendación. 
Segundo, los algoritmos *model-based* 

Los autores comenentaron en la sección 3.1.3 que la similud ajustada del coseno era mejor una mejor métrica que *cosine-based similarity* porque consideraba las diferencias en las escalas de calificación entre los usuarios. Esto me pareció interesante porque en las pruebas que realizaron se muestra que la similitud ajustada del coseno tuvo un mejor desempeño.

No obstante no me pareció adecuado que no explicasen por qué sólo consideraron los usuarios que habían calificado más de 20 películas en su set de datos. ¿Qué sucede con los usuarios que no cumplen con ese criterio?

Tampoco explican por qué utilizan el *rating* que le dan los usuarios a los ítemes para calcular la similitud entre estos. Tal vez, podrían haber considerado otros factores como las descripciones de estos. 


