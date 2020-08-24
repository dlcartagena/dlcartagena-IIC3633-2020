## BPR: Bayesian Personalized Ranking from Implicit Feedback
#### Rendle, S., Freudenthaler, C., Gantner, Z., & Schmidt-Thieme, L. (2009)
###### Comentario por: Diego Cartagena Herrera

Este paper propone un nuevo algoritmo de optimización basado en un análisis Bayesiano, el cual es aplicado a diferentes modelos ya existentes para realizar recomendaciones personalizadas.

Un punto muy interesante que destacan los autores es sobre la importancia de elegir el tipo de optimización adecuado. Ningún modelo mencionado en el paper realizaba una optimización de sus parámetros enfocada en el ranking, sino que estaba enfocada en predecir si un usuario elegiría cierto item o no.

Me llamó mucho la atención que la optimización se realizaba para un par de items (i,j) para un usuario determinado u. Esto me hizo mucho sentido a medida que avanzaba el paper, ya que lo que se quiere realizar a priori es rankear los items para un usuario determinado, por lo que es necesario determinar la preferencia de un item sobre otro.

En la sección 4.1.1 (Analogies to AUC optimization) los autores realizan una comparación entre su nuevo método BPR y el método de optimización AUC. Es necesaria realizar esta analogía? No le veo la relevancia realmente.

Por otro lado, en la sección 6 utilizan dos datasets diferentes: Rossmann dataset (10000 usuarios y 4000 items) y DVD rental de Netflix (10000 usuarios y 5000 items). Por qué en el de Netflix no hicieron el análisis sobre 4000 items? Creo que a pesar de que son solo 1000 items de diferencia, creo que agrega un sesgo que pudo haber sido evitado, ya que se pudo haber comparado sobre la misma cantidad de items.

Los resultados de este paper hablan por si solos, ya que cada vez que se utilizó BPR sobre un modelo los resultados fueron considerablemente superiores, lo cual es un indicio de que quizás el camino correcto sea mejorar los mecanismos de optimización, por sobre los modelos de recomendación.
