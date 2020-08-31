## Crítica: *Evaluating Recommendation Systems*

Los autores Shani y Gunawardana explican tres tipos de experimentos utilizados para evaluar sistemas recomendadores:
*  Las pruebas *offline* utilizan conjuntos de datos con información que relaciona a los usuarios con los ítems como *ratings*.  
*  Los estudios de usuarios (*user studies*) se caracterizan por involucrar a usuarios de prueba y solicitarles que interactúen con los sistemas recomendadores.
*  Las evaluciones *online* seleccionan aleatoriamente a una muestra de usuarios reales que utilicen los sistemas. 
Luego, explican diversas propiedades de los sistemas recomedadores como preferencia del usuario, precisión de la predicción, cobertura, robutez, etc. Para cada una explican cómo evaluarlas. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, fue interesante que los autores expongan dos metologías de evaluación que involucran interacción directa con los usuarios, ya que a lo largo del curso nos habíamos enfocado en pruebas *online*, que simulan el comportamiento de los usuarios mediante *sets* de datos. Con este nuevo enfoque se puede complementar el análisis. Por ejemplo, en los *user studies* no sólo se obtiene información cuantitativa sino que también cualitativa como sus opiniones, su comportamiento al interactuar con el sistema, etc.

Segundo, me habría gustado que profundizarán más en cómo evaluar los datos cualitativos. Por ejemplo, en un ramo Antro-Diseño (IDI2015) los analizan a través de la teoría fundamentada que 
> exige identificar categorías teóricas que son derivadas de los datos mediante la utilización de un método comparativo constante, recurriendo a la sensibilidad teórica del investigador (Mórales, 2015)
Este método era útil porque permitía examinar los datos según los temas o subtemas que eran recurrentes y con estos interpretar el fenómeno estudiado. 

Tercero, considero que uno no sólo debe preocuparse en que el sistema recomendador tenga la mejor precisión. Personalmente, creo que la diversidad de las recomendaciones es un factor esencial. Permite que los usuarios interactúen con contenidos distintos a los que normalmente prefieren. Por ejemplo, Twitter en 2019 fue acusado en varios medios de comunicación de amplificar la retórica política extremista porque le sugiere contenido más extremista a personas con esas tendencias (CNN, 2019). 

Finalmente, el texto de los autores es una buena guía para conocer las estrategias de evaluación de los sistemas recomendadores. Además, entrega métricas o sugiere cómo evaluarlos según sus propiedades como diversidad, utilidad, precisión de la predicción, cobertura, robutez, etc


Referencias:
* Páramo Morales, D. (2015). La teoría fundamentada (Grounded Theory), metodología cualitativa de investigación científica. Pensamiento & gestión, (39), 1-7.
* CNN. (2019). *How Twitter's algorithm is amplifying extreme political rhetoric*. Recuperado de https://edition.cnn.com/2019/03/22/tech/twitter-algorithm-political-rhetoric/index.html