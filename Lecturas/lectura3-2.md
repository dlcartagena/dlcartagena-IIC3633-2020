## Evaluating Recommendation Systems
#### Guy, S., & Gunawardana, A.. (2011)
###### Comentario por: Diego Cartagena Herrera

El paper habla sobre las distintas formas que existen de evaluar los sistemas recomendadores, de tal forma de poder seleccionar uno sobre otro. Existen 3 formas de evaluar un sistema recomendador:
1. Offline experiments: generalemente se utiliza un dataset, donde cada fila representa un usuario y el valor en cada columna para el usuario representa el rating que el usuario le dió a cierto item.
2. User Studies: se recluta a una cierta cantidad de personas para que interactúen con el sistema y realicen ciertas acciones. Adicionalmente, es posible hacer preguntas a estas personas antes, durante y después de utilizar el sistema.
3. Online evaluation: es la forma más real de evaluación (y la más costosa). Se busca evaluar el comportamiento del usuario a medida que utiliza los sistemas de recomendación, y cómo este puede ir cambiando dependiendo de diversos factores.

Luego, se realiza una descripción de los factores involucrados en los sistemas, y se describen diversas métricas que son adecuadas para supuestos planteados por los autores.

Debido a lo extensa de la lectura, es necesario estar muy concentrado para poder seguir el hilo de lo que plantean los autores. Me parece excelente el cómo se desarrolla el paper, yendo desde lo más general que serían las formas de evaluar un sistema, a lo más particular que es detallar cada factor involucrado en la evaluación y las métricas que se usan para medirlo.

Un tema muy interesante tratado es la preparación que debe tener el sistema para que un experimento sea exitoso. Cada uno de los tipos de evaluación tienen distintos costos, es por eso que iniciar con un Offline experiment es lo ideal para poder tunear los parámetros del sistema, de tal forma que cuando sea evaluado en un experimento con personas reales, este se comporte de tal forma que no disguste al usuario, ya que podría provocar un rechazo inmediato a utilizar el sistema.

Por otro lado, es muy interesante todas las variables que se deben considerar para evaluar un sistema recomendador. Incluso, es posible relacionar fuertemente el área de evaluación de un sistema con la psicología. Muchas de las hipótesis planteadas durante el paper se basan en el análisis del comportamiento humano. Es importante destacar la importancia de realizar hipótesis que se acerquen lo más posible al real pensamiento del usuario, ya que muchos factores como la confianza (Confidence), credibilidad (Trust), Serendipity, entre otras, tienen una relación directa con el comportamiento del usuario.

Me parece que es un paper muy completo, muy bien argumentado, y donde se explica muy bien las métricas que se pueden observar en muchos papers del área. Realmente es una guía que nos lleva a un mayor entendimiento de cómo medir un sistema, y nos entrega las herramientas para poder analizar la imagen completa antes de elegir un sistema por sobre otro.
