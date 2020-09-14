El *paper* de Pazzani et. al explica que el filtrado basado en contenido puede recibir tres tipos de datos:
* estructurados, en que cada un número determinado de atributos y cada ítem es descrito por ellos. 
* desestructurados, en que no hay conjuntos definidos de atributos. 
* semiestructurados, una mezcla entre los anteriores
Luego, explican las diversas metodologías existentes que utilizan contenido para recomendar ítems a los usuarios. A continuación, comentaré aspectos que considero interesantes y las dudas que tuve luego de leer el texto.

Primero, señalan los autores que muchos sistemas recomendadores crean una representación estructurada de la información que no lo es. Considero que este paso es fundamental ya que la calidad de la representación tiene un impacto directo en la recomendación. Según treehousetechgroup (2019) un texto desestructurado puede ser procesado no solo de acuerdo a *stemming* sino que también estos modelos:
* *Tokenization*: separa el texto en oraciones y palabras. No toma en cuenta la puntuación.
* *Lemmanization*: se unifican los sinónimos y toma en consideración los contextos de las palabras. 
* *Topic modeling*: es una herramienta de minería de texto que ayuda a descubrir temas en el texto y *clusters* relacionados a distintos tópicos.

Segundo, en el *paper* se centra en el análisis de texto. No obstante, hay otros formatos en que se presenta el contenido como imágenes, videos, etc. Por ejemplo, supongamos que una plataforma le quiere recomendar imágenes a un usuario de acuerdo a las imágenes que él ha subido al sitio. Entonces, se podrían extraer características a sus imágenes como LBP, HoG, Gabor etc. y recomendar otras que posean propiedades similares. 


Tercero, los autores indican que:
> Eventhough the naïve Bayes assumption of class-conditional attribute independence is clearly violated in the context, naïve Bayes per-forms very well. 

Esto me pareció interesante porque suena contradictorio que un método funcione bien cuando uno de sus principales supuestos no se cumple. 

Cuarto, podrían haber mostrado cuáles son las métricas de que habitualmente se utilizan para medir el rendimiento de los algoritmos basados en contenido. Probablemente, no se usan las mismas que para el filtrado colaborativo con *feedback* explícito como RMSE porque estas usan *ratings*, información que no necesariamente se tiene. 

Finalmente, el *paper* explica los diversos formatos en que se presenta el documento e indica las metodologías que permiten separar en *clusters* el contenido y realizar recomendaciones según estos. 

Referencias:
* Treehousetechgroup. (2019). *How to Analyze and Process Unstructured Data*. Recuperado de https://treehousetechgroup.com/how-to-analyze-and-process-unstructured-data/
