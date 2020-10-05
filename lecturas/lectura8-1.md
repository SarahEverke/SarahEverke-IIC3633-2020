# Crítica: *A user-centric evaluation framework for recommender systems*

Pu et. al proponen un marco de evaluación de sistemas recomendadores que se basa en las métricas de rendimiento-esfuerzo y el modelo de usuario-confianza. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, en las métricas de rendimiento-esfuerzo propuestas creo que es interesante que en ambas considerasen información cuantitativa y cualitativa. Al considerar tanto la opinión como el comportamiento del usuario se obtiene un mejor acercamiento a cómo el usuario valora el sistema en comparación de utilizar una métrica matemática. Aunque, probablemente utilizar esta metodología es más costoso en relación a usar métricas matemáticas, ya que involucra realizar casos de estudio con usuarios. 

Segundo, como miden a través de un cuestionario las variables subjetivas, es factible replicar el experimento y obtener datos que sean comparables. Sin embargo, esto es una limitación debido a que no pueden profundizar en la experiencia personal de cada usuario como lo haría por ejemplo una entrevista. 

Tercero, considero que faltó que hubiesen evaluado al menos un sistema recomendador con su propuesta. Especialmente, habría sido interesante comparar esta métrica con las métricas matemáticas, ya que se podría haber visto si existe una relación entre estas. 

Cuarto, no queda claro cómo combinar los valores subjetivos y objetivos de las métricas de precisión y esfuerzo. ¿Se ponderan con el mismo factor? ¿Se deben normalizar los valores antes de ser ponderados? 

Quinto, este método podría ser de gran ayuda para comparar resultados de algoritmos de recomendación que utilicen distintos tipos de datos, debido a que no es necesario que el *data set* que se estudie tenga sólo información explícita o implícita. Simplemente, para evaluar los resultados se recolectan datos según la interacción con el usuario como evaluando si hubo *switching task* (si un usuario escoje otro producto luego de revisar todos los ítems)

Finalmente, el *paper* es interesante porque propone un mecanismo de evaluación que toma en consideración información objetiva y subjetiva. Sin embargo, faltó señalar cómo interpretar el resultado final. ¿Se obtiene un único valor tras aplicar el modelo? ¿Mientras mayor sea implica que el usuario confía más en las recomendaciones?
  