## Content-based recommendation systems.
#### Pazzani, M. J., & Billsus, D. (2007)
###### Comentario por: Diego Cartagena Herrera

El paper habla sobre un tipo de recomendación basado en contenido, donde un item es recomendado dependiendo de la descripción de este, y de UN perfil que tiene el usuario, el cual es creado basado en sus preferencias.

En gran parte del paper se discute sobre los distintos métodos que existen para transformar información no estructurada (como texto) a una forma estructurada. Una de ellas es el stemming, cuyo objetivo es encontrar un término que refleje el significado de un grupo de palabras.

Me parece muy interesante el hecho de que si bien una palabra o término puede aparecer de forma repititiva, esto no significa que sea un término representativo para el contexto, ya que no es posible incluirlo. Otras posibles representaciones era considerar grupos de palabras como términos, de tal forma de entregarles valor a palabras que por si solas no tienen un real significado.

Algo muy rescatable del paper, es que introduce muy bien el tema, y es muy fácil de leer. Está muy bien estructurado, ya que toda la explicación de cómo estructurar información no estructurada es para entregar las herramientas para construir un perfil de usuario.

En la sección 10.3, se habla de un tradeoff existente entre el implicit y explicit feedback, lo cual me pareció muy relevante para la recomendación basada en contenido, ya que esta depende fuertemente de lo que al usuario le gusta y lo que no.

Luego se describen algoritmos para aprender una función que modele los intereses del usuario. Dentro de ellos se encuentran los Decision Trees y Nearest Neighbors, que si bien son muy simples, tienen un rendimiento igual o similar a algoritmos más complejos. Me parece que quizás pudieron haber profundizado un poco más en alguno de estos algoritmos, de tal forma de tener una referencia para comparar entre un algoritmo simple y otro complejo.

En la sección 10.6 se comienza a hablar del termino "queries" al hablar sobre el relevance feedback, sin embargo, no se aclara la definición de este hasta ya el final del paper en la sección 10.9, indicando que se trata del modelo del usuario.

Por otro lado, no queda clara la fórmula del Rocchio’s Algorithm, ya que si bien describen con palabras la función, nunca definen los <img src="https://render.githubusercontent.com/render/math?math=D_{i}"> en la fórmula (10.2), lo cual puede producir confusión en el lector.

Para concluir, el paper está bien estructurado, permite un entendimiento del tema principal que es la recomendación basada en contenido, y remarca la importancia de que la información a utilizar debe permitir diferenciar los intereses del usuario para realizar este tipo de recomendaciones.
