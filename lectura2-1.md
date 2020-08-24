## Crítica: *Collaborative Filtering for Implicit Feedback Datasets*

Los autores Hu et al. proponen una metodología de filtrado colaborativo que utiliza *feedback* implícito, es decir, información que representa indirectamente la opinión del usuario. Para esto implementaron un modelo de SVD con dos nuevas variables que representan la preferencia de un usario por un ítem y la confianza en ese valor. A continuación, comentaré aspectos que consideré interesantes y las dudas que tuve luego de leer el texto.

Consideré que utilizar como variable cuántas veces un usuario ha visto un *show* tenía sentido. Sin embargo, creo que habría sido interesante que también utilizara otras variables como los patrones de búsqueda de un usuario y que comparase los resultados de cada una. Esto permitiría investigar cuáles son los comportamientos implícitos más relevantes en la recomendación de ítems. 

Siento que es muy útil que la metodología pueda ser calculada en tiempo lineal de acuerdo al tamaño del input ya que permitiría que el método puede escalar a medida que crece el set de datos. También es un factor positivo que entregue explicaciones de las recomendaciones. Así la plataforma puede mostrárselas al usuario y generar un vínculo de confianza. Por ejemplo, cuando yo uso Netflix me agrada que la plataforma me indique por qué me recomienda un sección de películas (más populares, por qué viste *The Crown*, Comedias). Esto me ayuda a filtrarlas. 

Me habría gustado que usara más de una base de datos para comprobar sus resultados y que ya fuese conocida como MovieLens o Netflix para mostrar que los resultados son robustos en distintas plataformas. 

Entiendo que no pueda utilizar las mismas métricas que se usan en metodologías con *feedback* explicíto porque se desconoce qué    programas no le gustan al usuario. No obstante, los autores no explican bien cuáles son las ventajas de usar *rank* como métrica frente a otras alternativas. 



