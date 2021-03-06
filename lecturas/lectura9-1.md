# Crítica: *Multi-armed recommender system bandit ensembles*

Cañamares et. al analizan el rendimiento de incorporar *multi-armed bandits* en el diseño de sistemas de recomendación dinámicos que seleccionan lo mejor entre varios algoritmos según el desempeño anterior de cada candidato. A continuación, comentaré aspectos que consideré interesantes y las dudas que tuve luego de leer el *paper*.

Primero, considero interesante que se refieran al proceso de filtrado como cíclico, ya que así el proceso le entrega la posibilidad a los ensambles de observar y aprender en cada iteración. A diferencia de un paradigma de aprendizaje *offline* donde dado un volumen de datos se entrena un modelo, en este proceso cíclico se permite que configuración del ensamble mejore progresivamente. 

Segundo, en este proceso cíclico se está utilizando *reinforcement learning*, área de la inteligencia artificial inspirada en psicología conductiva, ya que las acciones que realiza el agente en un entorno son interpretadas como una recompensa, que luego retroalimenta al *bandit*. El comportamiento del agente es modificado en cada iteración según la recompensa. Con *reinforcement learning* surge el desafío de aprender los intereses del usuario y simultáneamente explotarlos para realizar las recomendaciones mientras opera el sistema (Parra, 2019).

Tercero, se utilizó el *dataset* de MoviLens que entrega información explícita de los gustos del usuario. Esto permite que el premio sea 1 si al usuario le agradó la recomendación y 0 en otro caso. Sin embargo, no explican cómo fijar los premio cuando se utiliza información implícita. Por ejemplo, si se utilizan las veces que un usuario vio una película se podría asignar el premio como 1 si el usuario ya vio la película y 0 en otro caso. No obstante, valorarla como 0 puede ser erróneo porque no sabemos si al usuario efectivamente le disgusta una película que no ha visto. 

Referencias:

* Parra, D. (2019). *Aprendizaje Reforzado para Sistemas de Recomendación*. Recuperado de http://dparra.sitios.ing.uc.cl/classes/recsys-2019-2/aprendizajereforzado_recsys.pdf
