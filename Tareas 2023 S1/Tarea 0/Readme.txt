Nota Parte 1: 8
Nota Parte 2: 0
Nota final: 8

P1: 15/20 pts
P2: 0/20 pts
P3: 0/60 pts
Total: 15/100 pts
Descuentos:
-20 pts (se usa una solución no vectorizada en P1)
PUNTAJE FINAL: 0/100 pts

---

PREGUNTA 1: 15/20 pts

- 5/5 pts: Generar array con posiciones en x aleatorias entre 0 y 1.

- 5/5 pts: Generar array con posiciones en y aleatorias entre 0 y 1.

- 5/5 pts: Calcular r o r².
Nota: la solución está bien, pero también se pudo hacer:
d = x**2 + y**2
La suma directa también está implementada en NumPy como una operación vectorizada, no es necesario usar np.add.

- 0/5 pts: Contar puntos dentro del área.

En Python, los bucles for y las compresiones de listas (cosas como [i**2 for i in X]) son muy lentos. Por eso, lo ideal en estos casos (y lo que se solicita en el fondo en esta pregunta) es usar NumPy para reemplazarlos lo más que se pueda.
Se debe usar NumPy para reemplazar el bucle for por una operación vectorizada.
[OJO: POR CADA SOLUCIÓN NO VECTORIZADA SE DESCUENTAN 20 PTS.]

Ejemplos posibles son:
inside = np.sum(d < 1)
inside = np.count_nonzero(d < 1)
inside = d[d<1].size
inside = len(d[d<1])
La operación d < 1 toma el arreglo d y compara elemento por elemento cuáles son menores a 1, retornando un arreglo de Trues y Falses. np.count_nonzero cuenta cuántos elementos son True. np.sum hace algo similar, sumando todos los Trues para obtener un número final.

---

PREGUNTA 2: 0/20 pts
No realizada.
- 0/10 pts: Calcular pendiente para error exacto.
- 0/10 pts: Calcular pendiente para error aproximado.

---

PREGUNTA 3.1: 0/45 pts
No realizada.

- 0/5 pts: Generar ángulos aleatorios entre 2π y 11π/4.
- 0/5 pts: Generar alturas aleatorias entre 0 y 4.
- 0/10 pts: Evaluar los ángulos aleatorios en la función g(t).
- 0/10 pts: Comparar alturas aleatorias con los valores en la función g(t).
- 0/5 pts: Contar los puntos bajo la curva.
- 0/10 pts: Estimar el área bajo la curva dada la cantidad de puntos.

PREGUNTA 3.2: 0/10 pts
No realizada.

- 0/5 pts: Utilización adecuada de vectorización.
- 0/5 pts: Caluclar el error de aproximación utilizando el código de la pregunta 2.

PREGUNTA 3.3: 0/5 pts
No realizada.

- 0/5 pts: Calcular pendiente para error aproximado.