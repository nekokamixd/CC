Nota Parte 1: 10
Nota Parte 2: 88
Nota final: 98

P1: 5/5 pts
P2: 53/55 pts
P3: 30/30 pts
Total: 88/90 pts
Descuentos: Ninguno

NOTA FINAL T2 PARTE 2: 88/90 pts

——-

Pregunta 1: Implementar vector_to_room y graficar la 1° habitación con esa función y room_to_image (5/5 pts)

——-

Pregunta 2.1: Dividir DATASET en WALLS, ENEMIES y COINS, y mostrar las paredes de la 1° habitación con plt.imshow (5/5 pts)

Pregunta 2.2: Implementar PCA (18/20 pts)

En general bien, pero hay un error al usar np.linalg.svd, pues el parámetro full_matrices debía ser setteado a False, no a True. Esto, para no usar la SVD completa, sino la reducida, que era lo que se pedía.

Detalle sin descuento: no era necesario definir dim = np.shape(M) para luego hacer mu = mu[:dim[1]] y V = V[:dim[1], :m]. El arreglo mu ya era del largo correcto, y esa línea no tiene efecto. Para V solo bastaba hacer V = V[:, :m].

Pregunta 2.3: Realizar PCA de 32 componentes sobre WALLS y mostrar la 1° componente principal con plt.imshow (5/5 pts)

Ojo, que no es necesario trasponer V para obtener la 1° componente. La 1° columna se puede obtener así: V[:, 0]. El resultado también es un vector 1D que se puede convertir con vector_to_room. Pero el resultado está bien.

Pregunta 2.4: Implementar rebuild_ith_row y usarla para reconstruir las paredes de la 1° habitación con el PCA anterior, y mostrar el resultado con plt.imshow (20/20 pts)

Pregunta 2.5: Implementar binarize y aplicarla sobre la reconstrucción anterior (5/5 pts)

——-

Pregunta 3.1: Implementar interpolate_rows (10/10 pts)

Pregunta 3.2: Interpolar las paredes de las habitaciones de índice 0 y 16 con alpha = 0.5 (2/2 pts)

Pregunta 3.3: Implementar generate_new_room_row (15/15 pts)

Pregunta 3.4: Generar una nueva habitación a partir de las de índices 0 y 16, con 32 componentes principales y alpha = 0.5 (3/3 pts)