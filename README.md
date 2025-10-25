Este archivo SQL sirve para crear una pequeña base de datos local (usando PostgreSQL) que contiene una lista de palabras clave relacionadas con los temas académicos que aparecen en la lista de estudiantes.

#¿Para qué sirve esto?
Imagina que tienes una lista de estudiantes y cada uno está trabajando en un tema diferente: Matemáticas, Física, Biología, Historia, etc.
Este archivo prepara una tabla en la base de datos donde se guardan palabras importantes (llamadas "palabras clave") que ayudan a identificar o describir mejor cada uno de esos temas.

##Por ejemplo:

Para el tema "Matemáticas", palabras clave podrían ser: números, álgebra, geometría, cálculo.
Para "Biología – Zoología", podrían ser: animales, especies, hábitat, vertebrados.
Cada palabra en la base de datos también incluye:

Qué tan relacionada está con el tema (un porcentaje, como 90% si es muy representativa).
Sinónimos o palabras similares que también podrían usarse (por ejemplo, "computación" y "informática").
¿Por qué es útil?
Esta base de datos puede usarse después para:

Buscar automáticamente qué tema le corresponde a un texto nuevo, basado en las palabras que contiene.
Ayudar a clasificar trabajos, proyectos o preguntas según su contenido.
Hacer búsquedas más inteligentes en sistemas educativos o de gestión académica.
¿Qué hace exactamente el archivo SQL?
Crea una tabla llamada palabras_clave con las columnas:
palabra: la palabra clave en sí.
porcentaje_identidad: qué tan fuerte es su relación con un tema (del 0 al 100).
sinonimos: otras palabras similares, separadas por comas.
Llena esa tabla con al menos 15 palabras clave, cada una vinculada a uno de los temas de la lista original (Matemáticas, Física, Química, etc.).
