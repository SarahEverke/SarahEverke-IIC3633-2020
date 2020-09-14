# Crítica: *Combining Predictions for Accurate Recommender Systems*

Jahrer et. al proponen que la combinación lineal (*blending*) de algoritmos de filtrado colaborativo (CF) aumenta el rendimiento y supera a cualquier algoritmo de ese tipo. Como *input* de sus ensambles recibieron las recomendaciones de 18 modelos con diversos hiperparámentros de AFM, GE, KNN, SVD y RBM. Luego, presentan varios ensamblajes como regresión lineal, redes neuronales, *bagging*, etc. Los peores resultados fueron obtenidos con la regresión lineal y los mejores con *bagging* de redes neuronales, regresión polinomial y GBDT. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, considero que es positivo que señalaran en la Tabla 2 los hiperparámetros de cada algoritmo de filtrado colaborativo que utilizaron en los ensambles, ya que esto facilita la replicación de la estrategia diseñada. 

Segundo, es interesante que hayan ensambles como el de regresión lineal que indiquen cuánto aporta cada modelo de filtrado colaborativo en la predicción, ya que en la práctica podría ser costoso entrenar y mantener 18 modelos con diversos parámetros. Se podría elegir, por ejemplo, a los cinco modelos que más aporten y utilizar esos para predecir. 

Tercero, la estrategia de ensamblar modelos es muy atractiva ya que el ensamble que tiene peor resultado (regresión lineal) supera al algoritmo de CF con mejor rendimiento SVD-4. Por lo que, es una metodología que hay que tomar en consideración al desarrollar sistemas de recomendación.

Cuarto, al leer el texto pensé que la mejora de los ensambles se podría deber a que se memorizaban los datos, generando un overfitting. No obstante, investigué y en varios medios señalan que no se produce overfitting pero que no se sabía exactamente por qué. Una frase que me gustó fue:

> *This [boosting] doesn't seem to overfit. That is an experimental result for which the literature is confused respect to providing an explanation. So, this stuff has been tried in all sort of problems like handwriting recognition, understanding speech, all sort of stuff uses boosting, and unlike other methods for some reason, and yet imperfectly understood, it does not seem to overfit. [...] In conclusion, this is magic, you always want to use it and it will work with any classifier.* (Winston, 2014)



Finalmente, los autores muestran que el ensable de diversos modelos de CF incrementa el rendimiento. Sin embargo, faltaría evaluar cómo es el desempeño de los ensambles respecto a otras propiedades como novedad, diversidad, *serendipity*, etc. Este *paper* no se limita al área de sistemas recomendadores sino que también es aplicable en otras áreas de *machine Learning* como clasificación.

Referencias:

* Winston, P. (2014). *17. Learning: Boosting (lecture of AI in the MIT)* . Recuperado de https://www.youtube.com/watch?v=UHBmv7qCey4#t=48m38s