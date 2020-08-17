## Crítica: *Netflix Update: Try This at Home*

Simon Funk explica en una entrada de su *blog* cómo obtuvo el tercer lugar en un concurso de Netflix donde había que predecir cómo un usuario evaluaría una película según la base de datos proporcionada. Su estrategia se basa en la descomposición de valores singulares (SVD) para determinar los valores faltantes. A continuación, comentaré aspectos que consideré interesantes y las dudas que tuve luego de leer la entrada del *blog*.

No me queda completamente claro por qué utilizó SVD. Podría haber señalado cuáles son sus ventajes frente a otras metodologías. 

Me pareció interesante que el autor considerase los casos 'borde' al calcular el *rating* promedio de cada película. Por ejemplo, si hay una película que en el set de entrenamiento sólo ha sido evaluada una vez con un 1, ¿es su *rating* promedio igual a 1? El autor ante esta pregunta asume que no. Para calcular el 'promedio mejorado' utiliza el promedio (Ra) y varianza (Va) de todos los promedios de los *ratings* de las películas con la varianza individual (Vb) de cada una. No obstante, no comprendí por qué él introduce un factor K = Va/Vb en el cálculo del nuevo promedio. Luego, señala que K = 25 funciona bien, pero me habría gustado que explicase cómo obtuvo ese resultado y que comparase el rendimiento de K = 25 versus K = Va/Vb. 

El autor indica que ya no están limitados a utilizar modelos lineales. Habría preferido que explicara más en detalle los motivos. Propone adaptar la función no lineal G a los datos y que el impacto de los valores negativos (películas bajo el promedio) fuese mayor que el de los positivos. Personalmente, me pareció que la propuesta de penalizar más los valores negativos tenía sentido. También, decide que sólo es favorable usar la opción no lineal en las primeras 20 características. ¿Pero, cuáles son los beneficios? ¿Mejora la predición? ¿Es más veloz?

