El *paper* de Pazzani et. al explica que el filtrado basado en contenido puede recibir tres tipos de datos. 

Luego, explican las diversas metologías existentes que utilizan contenido para recomendar ítems a los usuarios. 

Primero, Pazzani et. al señalan que los datos son categorizados en:
* estructurados
* desestructurados
* semi-estructurados

Luego, explican que muchos sistemas recomendadores crean una representación estrcuturada de la información que no lo es. Considero que este paso es fundamental ya que la calidad de la representación tiene un impacto directo en la recomendación. Según treehousetechgroup (2019) un texto desestructurado puede ser procesado de acuerdo a diversos modelos:
* Tokenization
* Stemming
* Lemmanization
* Topic modeling

Segundo, en el *paper* se centra en el análisis de texto. No obstante, hay otros formatos en que se presenta el contenido como imágenes, videos, etc. Por ejemplo, supongamos que una plataforma le quiere recomedar imágenes a un usuario de acuerdo a las imágenes que él ha subido al sitio. Entonces, se podrían extraer características a sus imágenes como LBP, HoG, Gabor etc. y recomendar otras que posean propiedades similares. 


Tercero, los autores indican que:
> Eventhough the naïve Bayes assumption of class-conditional attribute independence is clearly violated in the context, naïve Bayes per-forms very well. 

Esto me pareció interesante porque suena contradictorio que un método funcione bien cuando uno de sus principales supuestos no se cumple. 

Cuarto, podrían haber mostrado cuáles son las métricas de que habitualmente se utilizan para medir el rendimiento de los algoritmos basados en contenido. Claramente no se pueden usar RMSE.
Los más convenientes serían 

Finalmente, el *paper* narra


https://treehousetechgroup.com/how-to-analyze-and-process-unstructured-data/