## Multi-armed recommender system bandit ensembles.
#### Cañamares, R., Redondo, M., & Castells, P. (2019)
###### Comentario por: Diego Cartagena Herrera

El paper habla sobre los métodos de ensamble "bandit", donde el método (bandit) debe seleccionar un algoritmo de recomendación dentro del ensamble (arms) para generar recomendaciones.

Los autores proponen un método cíclico, donde mediante reinforcement learning el método va aprendiendo y mejorando la configuración del ensamble para cada usuario objetivo.

El proceso a seguir es el siguiente:

1. Se selecciona un algoritmo de ensamble para cada usuario (arm).
2. Se realiza una recomendación a cada usuario con el algoritmo escogido.
3. Se actualizan los algoritmos del ensamble.

De esta forma, el algoritmo escogido en una instancia va depender de las "armas" escogidas en las iteraciones previas. Esta forma de plantear me parece muy interesante, ya que si bien escoge un algoritmo basado en su rendimiento previo, nunca deja de lado completamente un algoritmo (A/B testing). Por otro lado, me llamó mucho la atención el bias que se genera eligiendo un algoritmo sobre otro en el comienzo, por lo que el diseño de este método debe ser realizado con mucha precaución y siempre considerando las características de nuestros datos.

Por otro lado, proponen dos formas de elegir el arma para cada usuario:

1. <img src="https://render.githubusercontent.com/render/math?math=\varepsilon">-greedy: se selecciona con probabilidad 1 - <img src="https://render.githubusercontent.com/render/math?math=\varepsilon"> al algoritmo con mayor recompensa promedio, y el resto de los algoritmos es escogido con probabilidad <img src="https://render.githubusercontent.com/render/math?math=\varepsilon"> uniformemente.

2. Thompson sampling: cada arma obtiene un valor <img src="https://render.githubusercontent.com/render/math?math=p_{a}"> a partir de la distribución Beta(<img src="https://render.githubusercontent.com/render/math?math=\alpha_{a}, \beta_{a}">), donde <img src="https://render.githubusercontent.com/render/math?math=\alpha_{a}, \beta_{a}"> corresponden a las recomendaciones exitosas y no exitosas respectivamente. Se escoge el arma con mayor
<img src="https://render.githubusercontent.com/render/math?math=p_{a}">.

Cada recomendación acertada otorga una recompensa igual a 1, y 0 en otro caso.

Dado que solo se realiza una sola recomendación por usuario, el costo computacional es muy bajo. Sería interesante realizar un método en el que se escogiera además otro algoritmo (no personalizado quizás) además del arma para cada iteración, de tal forma de que si la recomendación no es exitosa, exista un "plan B" que sí podría entregar una recomendación exitosa. Sin embargo no sé cómo podría esto afectar el aprendizaje de cada algoritmo en este método.

Me parece un método muy creativo y que los positivos resultados demuestran que el éxito puede lograrse reformulando de cierta forma los algoritmos ya existentes de recomendación.
