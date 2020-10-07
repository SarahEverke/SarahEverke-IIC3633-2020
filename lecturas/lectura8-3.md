# Crítica: *Inspectability and control in social recommenders*

Los autores estudian cómo el aumento de inspeccionabilidad y control en el proceso de recomendación afectan la experiencia del usuario. Para esto realizaron un estudio *online* sobre un recomendador de música en *Facebook* con las siguientes etapas:
1. Los usuarios pueden modificar ajustar los pesos de los ítems que les gustan y de la confianza que le tienen a los gustos de sus amigos. En caso de que el usuario sea asignado al grupo *"no control"* no realiza este paso.
2. Los participantes puede ver una lista de las recomendaciones o un grafo explicativo.
3. Los usuarios responden un cuestionario sobre su experiencia.


Tras, realizar el experimento los autores concluyeron que tanto la inspeccionabilidad como el control sobre las recomendaciones mejora la experiencia de los participantes. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, la forma en que Knijnenburg et al. le muestran la información a los usuarios es relevante, ya que los participantes que vieron el grafo explicativo lo inspeccionaron por más tiempo. Esto es interesante porque muestra que la manera en que se le entrega la información a un usuario afecta su comprensión del sistema. 

Segundo, en el *paper* basan las recomendaciones según los gustos musicales (dados por los *likes*) y los amigos en Facebook de un usuario. Por lo que, es sencillo comprender que si se modifican los pesos de sus gustos musicales o de la confianza de sus amigos las recomendaciones pueden variar. No obstante, en el caso de que se usase otro modelo como SVD, cuyos factores latentes no tienen necesariamente una "traducción", podría ser más complejo explicar qué características se están modificando. 

Finalmente, los autores muestran que al permitir que los usuarios puedan controlar los pesos genera que se perciba que la recomendación es de mejor calidad y una mayor satisfacción. Además, al presentar el grafo explicativo mejoró la experiencia del usuario. Por tanto, al diseñar un sistema recomendador hay que tomar en consideración cómo una persona va a interactuar con él y no sólo preocuparse de mejorar el rendimiento matemático.
