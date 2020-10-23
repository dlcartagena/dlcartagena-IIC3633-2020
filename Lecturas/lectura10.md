## Deep learning based recommender system: A survey and new perspectives.
#### Zhang, S., Yao, L., Sun, A., & Tay, Y. (2019)
###### Comentario por: Diego Cartagena Herrera

El paper introduce al lector en el área de recomendación basada en redes neuronales profundas. Al comienzo se enfatiza que es un área nueva que está "de moda" debido a los grandes avances y buenos resultados que las redes neuronales profundas han tenido.

En la sección 2 se revisan ciertos conceptos que serán utilizados en las siguientes secciones del paper. Me parece que la sección 2.1, donde se revisan las diferentes técnicas de Deep Learning, es demasiado general para la complejidad que se presenta en la sección 3. Si bien esto no es un paper enfocado en técnicas de Deep Learning, creo que para alguien que está adentrándose en el área (y con un mínimo conocimiento de conceptos) puede ser un poco abrumador.

Luego los autores justifican el uso de Deep Learning para la tarea de recomendación, donde los prinicipales argumentos para su uso son:

1. Cuando existe una gran cantidad de datos complejos.
2. Cuando los items son imágenes, videos o texto.
3. Porque los modelos 'state of the art' pueden ser extendidos al uso de redes.

Por otro lado, los autores señalan la existencia de limitaciones en la interpretabilidad (las redes tienden a ser cajas negras), requerimiento de datos (para que las redes aproximen funciones requieren de una gran cantidad de datos) y la gran cantidad de hiperparámetros que hay que tunear.

Me parece un punto muy importante la interpretabilidad de las recomendaciones, ya que como usuario el saber por qué me recomendaron un determinado item es de gran valor y otorga mayor credibilidad a las recomendaciones.

En la sección 3 se detallan varios modelos basados en Deep Learning, los cuales fueron clasificados por la técnica de Deep Learning utilizada.

1. MLP

Se detalla una extensión del modelo CF usando redes neuronales (Neural Collaborative Filtering). En esta se entrega a la capa de input los perfiles de usuario y features de cada item, se generan factores latentes en la embedding layer y luego pasa por las capas de CF, para finalmente en la capa de output devolver el score.

Otra extensión de modelo es Deep Factorization Machine, sin embargo no me quedó muy claro el funcionamiento de este modelo.

2. Autoencoder Neural Network

Los autoencoders son utilizados de formas: para aprender representaciones de baja dimensión, o para rellenar los espacios en blanco de la matriz de interacción.

Fue una gran confusión cuando hablan de CF usando ANN, ya que creí que este había sido clasificado como un modelo que utilizaba MLP.

3. CNN

Utilizado frecuentemente para datos multimedia y texto. Se utilizan para aprender representaciones de features a partir de estos datos. Se menciona que CF puede ser ampliado utilizando CNN y que se pueden utilizar grafos para estructurar esta nueva información.

En conclusión, me parece que la orientación del paper es introducir a esta área de recomendación, pero que la forma en que lo hace debe estar mucho mejor hilada, de forma que la lectura no sea tan dura y lleve a que el lector se desinterese por esta interesante área.
