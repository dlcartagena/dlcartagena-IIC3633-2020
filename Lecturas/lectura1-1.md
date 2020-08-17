
## Item-Based Collaborative Filtering Recommendation Algorithms
##### Diego Cartagena Herrera
En el paper se expuso sobre los diferentes tipos de algoritmos de recomendación Collaborative Filtering, los cuales se separaban en dos tipos: memory-based (user-user) y model-based (item-item).

Durante gran parte del artículo se entregan los conocimientos básicos de este tipo de algoritmos, y cuales son las dificultades que se presentan en la práctica (escalabilidad y calidad de las recomendaciones), lo que lleva a que los autores propongan su propio algoritmo (model-based).

Si bien los resultados demuestran una gran mejora en cuánto a calidad de las recomendaciones y el tiempo de ejecución de estas, todo se basa en el supuesto de que el usuario haya realizado una cierta cantidad de ratings (en la sección 4.1 se especifica que se seleccionan solo usuarios con 20 o más ratings), lo cual genera un sesgo en el rendimiento del algoritmo. Creo que es necesario incluir este punto en la sección de discusión, ya que no siempre se podrá asegurar que el usuario al que se le hará la recomendación tenga una gran cantidad de ratings. Por otra parte, hubiese sido interesante que hicieran una comparación de la calidad de las recomendaciones a un usuario dependiendo de la cantidad de ratings realizados.


Otro punto importante a destacar es que en la sección de Conclusión en gran parte se resume el problema de recomendación en grandes sets de datos y se enfoca en que los sistemas recomendadores son importantes en e-Commerce, dejando en segundo plano lo más importante que es el algoritmo que los autores presentaron en este paper.

En conclusión, es un artículo que explica muy bien los sistemas de recomendación CF, gran parte del paper se centra en explicar en detalle el funcionamiento de estos, sin embargo, puede que en ciertos momentos se pierde el foco de lo que realmente es importante en el paper.
