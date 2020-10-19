# Crítica: *Zhang, S., Yao, L., Sun, A., & Tay, Y. (2019). Deep learning based recommender system: A survey and new perspectives.*

El objetivo del texto es presentar una revisión bibliográfica de los avances en los sistemas de recomendación basados en *deep learning*. En la sección 2 muestran una visión general sobre los sistemas de recomendación y las técnicas de *deep learning*. Luego, en la sección 3 introducen las categorías de *deep learning* e indica las investigaciones que están en el estado del arte. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, los autores señalan al inicio del texto que:

> Recommender systems are an intuitive line of defense against cosumer over-choise.

Considero que esto es interesante porque se expone que tener demasiadas opciones puede ser perjucial para el usuario. Es más, Scheibehenne (2008) indica que cuando hay muchas opciones disponibles, los consumidores pueden sentirse ansiosos, desconectados e incluso pueden deprimirse. Por lo que, los sistemas recomendadores son un beneficio al usuario, ya que le muestran una selección menor de ítems a los consumidores.

Segundo, en la sección 3.2 los autores indican que en CML, MLP se utiliza para aprender representaciones de ítems como textos, imágenes o *tags* sin la necesidad de realizar *feature engineering*. Por ejemplo, mediante *feature engineering* se determinaron características como LBP o las 7 métricas de atractivo visual, que fueron desarrolladas por expertos en esa área. En cambio, con *deep learning* se puede utilizar una red como *AlexNet* para obterner descritores de imágenes. Esto es más rápido, ya que no requiere crear nuevas características en caso de que las actuales (como LBP) no sean suficientes. No obstante, se desconoce con qué criterio MLP representó a los ítems.

Referencias:
* Scheibehenne, B. (2008). The effect of having too much choice.

