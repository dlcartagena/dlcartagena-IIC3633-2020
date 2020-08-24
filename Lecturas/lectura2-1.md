## Collaborative Filtering for Implicit Feedback Datasets
#### Hu, Y., Koren, Y., & Volinsky, C. (2008)
###### Comentario por: Diego Cartagena Herrera

El paper a discutir desarrolla y contextualiza un algoritmo de recomendación Collaborative Filtering para Implicit Feedback, es decir, el usuario no entrega información sobre si le gustó o no un item determinado. El algoritmo se basa en analizar los comportamientos del usuario, y a través de estos poder obtener información que nos permita realizar recomendación de items.

Me pareció un paper muy interesante, dado que es un enfoque completamente contrario a lo que es Collaborative Filtering para Explicit Feedback. Otro punto a destacar es que está muy bien explicado las diferencias entre implicit y explicit feedback, deteniéndose en remarcar cada diferencia y ejemplificando muy bien.

Sin embargo, creo que en la sección 4 (Our Model) se pierde ese nivel de explicación detallada que tenía el paper en las secciones anteriores, específicamente en el cálculo del vector $x_{u}$, donde no queda muy claro cómo llega a esa factorización, o por qué calcula $Y^{T}Y$. Lo mismo para el cálculo de $y_{u}$.

En la sección 5 (Explaining Recommendations) explican cómo el algoritmo es capaz de entregar una explicación de la recomendación. El usuario es abstraído utilizando factores latentes, por lo que encontrar una relación transformando el modelo de factores latentes a un modelo lineal que le otorga un peso a la similaridad entre items desde el punto de vista del usuario es bastante impresionante. Sin embargo, en esta sección definen el vector de preferencia como $\hat{p}_{ui} = y_{i}^{t}x_{u}$, siendo que anteriormente había sido definido como $\hat{p}_{ui} = x_{u}^{t} y_{i}$, lo que puede llevar a confusiones.

Por otro lado, en la sección 6 (Experimental Study) mencionan que el período de training de 4 semanas fue elegido basado en un estudio expermiental, sin embargo no citan el estudio en ningún lado, pudiendo dejar en duda si las decisiones que tomaron para realizar el experimento fueron las mejores.

Para finalizar, me gustaría recalcar lo bien estructurado del paper. Fue un agrado que explicaran cada una de los puntos que mencionan, está muy bien contextualizado y los resultados del sistema implementado son excelentes comparado a los modelos Most Popular y Neighborhood based.
Punto aparte a destacar, es el primer modelo basado en descomposición de matrices que entrega una explicación a las recomendaciones. Excelente paper.
