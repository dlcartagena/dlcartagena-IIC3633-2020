## Performance of Recommender Algorithms on Top-N Recommendation Tasks
#### Cremonesi, P., Koren, Y., & Turrin, R. (2010)
###### Comentario por: Diego Cartagena Herrera

El paper realiza una comparación de distintos modelos en la tarea de recomendar una cantidad N de items, donde estos items debiesen ser los más atractivos para el usuario. Para realizar el testeo se utilizaron datasets de películas (MovieLens y Netflix), donde se separó cada dataset en un set de training M y otro set de testing T, el cuál solo contenía aquellas películas que obtuvieron el mejor rating (5 estrellas). De esta forma los autores determinaban como un éxito que dado un valor de N, el modelo rankeara entre 1 y N a la película.

Me parece que es un paper muy conciso, no se da muchas vueltas en introducir el tema, sino que describe el contexto de forma muy acotada, detalla el funcionamiento de cada modelo y luego muestra los resultados de su experimento.

Algo que me gustó mucho del experimento que realizaron, es que intentaron eliminar lo más posible el sesgo, eliminando aquellas recomendaciones que serían triviales (dado que eran películas que tenían muchos ratings, y por lo tanto las más populares), lo que le otorga gran generalización y mayor credibilidad a los resultados obtenidos. Además incluyen el experimento para el test set completo, lo que sirve para justificar de mejor manera la decisión tomada.
