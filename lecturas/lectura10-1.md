# Crítica: *Zhang, S., Yao, L., Sun, A., & Tay, Y. (2019). Deep learning based recommender system: A survey and new perspectives.*

El objetivo del texto es presentar una revisión bibliográfica de los avances en los sistemas de recomendación basados en *deep learning*. En la sección 2 muestran una visión general sobre los sistemas de recomendación y las técnicas de *deep learning*. Luego, en la sección 3 introducen las categorías de *deep learning* e indica las investigaciones que están en el estado del arte. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, los autores señalan al inicio del texto que:

> Recommender systems are an intuitive line of defense against cosumer over-choise.

Considero que esto es interesante porque se expone que tener demasiadas opciones puede ser perjudicial para el usuario. Es más, Scheibehenne (2008) indica que cuando hay muchas opciones disponibles, los consumidores pueden sentirse ansiosos, desconectados e incluso pueden deprimirse. Por lo que, los sistemas recomendadores son beneficios para el usuario, ya que le muestran una selección menor y personalizada de ítems.

Segundo, en la sección 3.2 los autores indican que en CML, MLP se utiliza para aprender representaciones de ítems como textos, imágenes o *tags* sin la necesidad de realizar *feature engineering*. Por ejemplo, mediante *feature engineering* se determinaron características como LBP o las 7 métricas de atractivo visual, que fueron desarrolladas por expertos en esa área. En cambio, con *deep learning* se puede utilizar una red como *AlexNet* para obtener descriptores de imágenes. Esto es más rápido, ya que no requiere crear nuevas características en caso de que las actuales (como LBP) no sean suficientes. No obstante, se desconoce con qué criterio MLP representó a los ítems e impide que puedan ser interpretados los descriptores.

Tercero, en varios modelos utilizan la sigmoide como función de activación. Sin embargo, esta función sufre del *vanishing problem* que sucede cuando:
>  n hidden layers use an activation like the sigmoid function, n small derivatives are multiplied together. Thus, the gradient decreases exponentially as we propagate down to the initial layers (Wang, 2019).

Un pequeño gradiente significa que los pesos en la primera capa no se actualizarán efectivamente en cada iteración. Por lo que, se podrían probar otras funciones de activación como ReLU. 

Referencias:
* Scheibehenne, B. (2008). The effect of having too much choice.
* Wang, C. (2019). *The Vanishing Gradient Problem*. Recuperado de https://towardsdatascience.com/the-vanishing-gradient-problem-69bf08b15484
