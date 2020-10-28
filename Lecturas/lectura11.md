## Deep learning based recommender system: A survey and new perspectives. (Desde 3.5)
#### Zhang, S., Yao, L., Sun, A., & Tay, Y. (2019)
###### Comentario por: Diego Cartagena Herrera

En la sección 3.5 se describen a grandes rasgos modelos de recomendación utilizando Recurrent Neural Networks (RNN), técnica que se adapta muy bien al uso de datos secuenciales. Se describen los avances en dos áreas de recomendación:

1. Session-based recommender sin identificación de usuario.

Me llama mucho la atención este enfoque en usuarios que no se han registrado, ya que es algo muy común en sitios de e-commerce que el usuario está recién conociendo, por lo que una buena recomendación tiene un impacto muy grande en el 'engagement' del cliente. En este caso, se busca obtener las preferencias del usuario en el corto plazo.

2. Sequential-based recommender con identificación de usuario.

Se describe la Recurrent Recommender Network (RRN), la cual permite modelar la evolución de los items y las preferencias del usuarios a través del tiempo.

3. Feature Representation Learning.

RNN es utilizado además para obtener representaciones latentes que permitan capturar la coevolución de usuarios e items.

En la sección 3.6 se describe el primer modelo de recomendación utilizando redes neuronales, Restricted Boltzmann Machine. En la versión con feedback explícito, el score de rating es representado con vectores one-hot encoding de la forma: [0,0,1,0,0]. Esto significa que el usuario le dió rating 3 a un item.

En la sección 3.7 se habla de Neural Attention recommendation. Esto permite capturar la información más relevante de los inputs. Los modelos Neural Attention pueden ser clasificados en vanilla attention y co-attention. Vanilla atention utiliza un vector de contexto para el aprendizaje, mientras que co-attention aprende pesos a partir de dos secuencias.

En la sección 3.8 hablan de Neural AutoRegressive based recommendation, sin embargo no me queda claro el funcionamiento de este, ya que es una alternativa al uso de RBM para CF. Dado que usa probabilidades condicionales quizá hubiese sido bueno mostrar la diferencia de resultados al ordenar los datos por timestamp y cuando no.

La sección 3.11 es una de las más interesantes, ya que nombra algunos trabajos que pueden ser clasificados como híbridos, ya que utilizan más de una arquitectura de redes neuronales. Cada una de estas arquitecturas tiene una tarea específica. Por lo general CNN son utilzadas para generar embeddings de datos no estructurados.

Creo que el área de recomendación utilizando Deep Learning no ha sido aún completamente explotado, y que a pesar de que existen avances muy grandes, siempre es posible innovar, ya que las redes neuronales son una herramienta muy poderosa que permitirá abrir el paso hacia mejores recomendaciones.
