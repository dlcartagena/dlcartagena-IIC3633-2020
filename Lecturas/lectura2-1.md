## Collaborative Filtering for Implicit Feedback Datasets
#### Diego Cartagena Herrera

Me pareció un paper muy interesante, dado que es un enfoque completamente contrario a lo que es Collaborative Filtering para Explicit Feedback. Otro punto a destacar es que está muy bien explicado las diferencias entre implicit y explicit feedback, deteniéndose en remarcar cada diferencia y ejemplificando muy bien.

Sin embargo, creo que en la sección 4 (Our Model) se pierde ese nivel de explicación detallada que tenía el paper en las secciones anteriores, específicamente en el cálculo del vector $x_{u}$, donde no queda muy claro cómo llega a esa factorización, o por qué calcula $Y^{T}Y$. Lo mismo para el cálculo de $y_{u}$.

En la sección del paper en que explican el experimento que realizaron mencionan que el vector de preferencia $\hat{p}_{ui} = y_{i}^{t}x_{u}$, siendo que antes lo habían definido como $\hat{p}_{ui} = x_{u}^{t} y_{i}$, lo  que puede llevar a confusiones, a pesar de que son lo mismo.

Por otro lado, mencionan que el periodo de training de 4 semanas fue elegido basado en un estudio expermiental, sin embargo no citan el estudio en ningún lado.
