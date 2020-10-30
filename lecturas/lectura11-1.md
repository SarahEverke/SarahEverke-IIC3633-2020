# Crítica: *Zhang, S., Yao, L., Sun, A., & Tay, Y. (2019). Deep learning based recommender system: A survey and new perspectives.*

El objetivo del texto es presentar una revisión bibliográfica de los avances en los sistemas de recomendación basados en *deep learning*. En las secciones 3 y 4 presentan los desafíos y los problemas abiertos en el área, identifican las nuevas tendencias y posibles direcciones en las investigaciones futuras sobre generar recomendaciones con *deep learning*. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, es interesante que en *session-based recomendation without user identifier* se hayan obtenido resultados similares con GRU4Rec y un simple *approach* basado en vecindad. Esto muestra que los mecanismos que no están basados en *deep learning* también son competitivos y son una alternativa. Asimismo, señalan que un ensamble entre los modelos obtuvo un mejor rendimiento. Por lo que, hay que tener en consideración mezclar metodologías (vía regresión lineal, boosting, bagging, etc) con *deep learning* y de filtrado más clásico. 

Segundo, los autores desmienten que las recomendaciones con *deep learning* carecen completamente de explicabilidad. Especialmente, recalcan que los *attentional models* son interpretables en gran medida porque entregan *insights* de cómo están funcionando. Asimismo, según West (2019) el conocimiento de cada capa de la red se construye sobre el conocimiento de las anteriores. Por ejemplo, en la siguiente red de tres capas se ve que en cada una agrega y recombina el conocimiento de las aprendidas:

![](image-10-1.png)

Tercero, concuerdo con los autores en que en el área faltan criterios comunes al evaluar los modelos, ya que en los *papers* que he leído durante el curso utilizan diversos *baselines*, métricas de evaluación, no especifican los parámetros de los algoritmos o no especifican cómo dividieron los sets de testeo y entrenamiento. Claramente, es una tarea compleja ya que, por ejemplo, no todos los algoritmos pueden utilizar las mismas métricas (MAE) como en el caso de filtrado con información implícita o explícita.

Cuarto, me preocupa que los usuarios no puedan decidir que información pueden usar los programadores para desarrollar los sistemas recomendadores. En el texto mencionan que:

> However, the session or cookie mechanisms enables those systems to get user`s short term preferences.

Sin embargo, ¿hasta que punto se puede explotar la información privada de una persona para obtener una mejor recomendación? ¿Se debiese regular que datos pueden explotar los algoritmos?

Referencias:

* West, M. (2019). *An Introduction to Deep Learning*. Recuperado de 
https://www.bouvet.no/bouvet-deler/an-introduction-to-deep-learning
