# Crítica: *Carousel Personalization in Music Streaming Apps with Contextual Bandits*

Bendana et. al modelan la personalización de *swipeable carousels*, listas *rankeadas* de ítems como un problema de *multi-armed bandit*. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, como los *multi-armed bandit* son un tipo de problemas de *reinforcement learning* está presente el desafío de aprender los intereses del usuario y explotarlos simultaneamente. Los autores mencionan que dado a esto surge el *exploration-explotation dilemma*. Lin et. al lo explica como:

>  As an agent starts toaccumulate some knowledge about the environment, it seems plausible to exploit the current knowledge in order to improve the immediate payoffs. However, sticking to the currently best option may cause the agent to ignore some potentially better options that haven’t been explored yet. 

Además, menciona que se han estudiado algoritmos como *Recency-Based Exploration* y *Detect and Explore Algorithm* (DAE). 

Segundo, considero que es positivo que los autores se hayan preocupado del caso en que el usuario probablemente no vio todos los ítems del carrusel, ya que tomar en consideración está posibilidad es más realista. Para esto se basaron en el modelo de cascada y a los ítems que no son "vistos" le asignan una X. Sin embargo, me hubiese gustado que explicaran con más detalle cómo manejar esos datos. ¿Se deben seguir mostrando los ítems que están marcados con una X en la siguiente ronda hasta que el usuario los vea? ¿O cómo interpreta el agente la X? ¿No modifica su comportamiento?

Tercero, es interesante que la inclusión del modelo cascada mejora el rendimiento de los sistemas de recomendación, ya que esto indica que para cada sistema recomendador hay que analizar cómo procesar los datos que requiere. 

Por último, los *multi-armed bandit* son útiles para resolver problemas de recomendación. Los autores muestran en la Fig.2 rendimiento de esta estrategia depende de cómo se escogen los brazos del agente. No obstante, hubiese sido positivo que comparasen sus resultados con los algoritmos tradicionales de filtrado y ensambles de estos para ver las diferencias o semejanzas de sus comportamientos.

Referencias:

* Lin, K., Kansal, A., Lymberopoulos, D., & Zhao, F. (2010, June). Energy-accuracy trade-off for continuous mobile device location. In Proceedings of the 8th international conference on Mobile systems, applications, and services (pp. 285-298).
