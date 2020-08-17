## Crítica: *Netflix Update: Try This at Home*

Simon Funk explica en una entrada de su *blog* cómo obtuvo el tercer lugar en un concurso de Netflix donde había que predecir cómo un usuario evaluaría una película según la base de datos proporcionada. Según él 

No me queda completamente claro por qué utilizó SVD y cuáles son las vetanjas de esta metodología frente a otras 

Tampoco 

Me pareció interesante que el autor considerase los casos 'borde' al calcular el *rating* promedio de cada película. Por ejemplo, si hay una película que en el set de entrenamiento sólo ha sido evaluada una vez con un 1, ¿es su *rating* promedio igual a 1? El autor ante esta pregunta asume que no. Para calcular el 'promedio mejorado' utiliza el promedio (Ra) y varianza (Va) de todos los promedios de los *ratings* de las películas con la varianza individual (Vb) de cada una. No obstante, no comprendí por qué él introduce un factor $K = Va/Vb$ en el calculo del nuevo promedio. Luego, señala que $K = 25$ funciona bien, pero me habría gustado que explicase cómo obtuvo ese resultado o que comparase el rendimiento con $K = 25$ versus $K = Va/Vb$. 


