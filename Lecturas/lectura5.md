## Context-Aware Recommender Systems
#### Adomavicius, G., Mobasher, B., Ricci, F. and Tuzhilin, A. (2011)
###### Comentario por: Diego Cartagena Herrera

El paper describe un área de recomendación en la que no solo interesa entregar un ranking para pares de valores <usuario, item>, sino que recalca la importancia de que esta recomendación se realice dentro de un contexto, entregando rankings para tripletas <usuario, item, contexto>, de forma que permitan realizar recomendaciones más inteligentes.

La definición de contexto no está clara, sin embargo en el artículo se mencionan dos puntos de vista:

1. Representativo: como forma de información.
2. Interaccional: de forma dinámica, donde el contexto depende de la actividad, y el contexto influencia la actividad.

Se definen los factores contextuales, los cuales pueden ser observables, parcialmente observables o implícitos. Además, estos pueden cambiar a medida que el tiempo avanza, por lo que podemos clasificarlos como estáticos y dinámicos.

Algo muy interesante que plantea el autor es cómo el usuario puede entregar un cierto feedback con respecto al contexto, para así poder mejorar su perfil de usuario, o simplemente para mejorar los factores contextuales. Sin embargo, me parece que es algo poco efectivo debido a que la cantidad de usuarios que dan feedback es muy bajo.

Por otro lado, algo muy positivo de los CARS es la posibilidad de que puedan ser aplicados sobre sistemas de recomendación tradicionales. En un principio al leer el artículo, me dió la impresión de que este nuevo paradigma de recomendar en un contexto dado iba a ser un sistema completamente distinto a los que hemos estudiado, sin embargo, la posibilidad de integrar este sistema en distintas etapas de la recomendación (contextual prefiltering o contextual postfiltering) es un avance muy grande, ya que deja abiertas muchas puertas para experimentar realizando distintos ensambles.

Algo que me causó mucha impresión es cómo se obtienen estos factores contextuales. Me parece muy importante recalcar que los usuarios a veces tienen muy poca noción de la cantidad de información que es extraída con su teléfono móvil, o por simplemente ingresar a un sitio web. Si bien no viene al tema del artículo, sería interesante saber cómo esta información es utilizada, y transparentar de cierta forma el uso que se hace de estos datos.

Me parece que la forma en que el artículo está escrito permite entender muy bien cuál es el enfoque de este sistema de recomendación, me gustó mucho que mostrará ejemplos reales de su uso en diversas áreas (gastronomía, viajes, shopping) y creo que genera la motivación suficiente para adentrarse a investigar mucho más en esta área.
