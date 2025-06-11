# 📊 Análisis de Algoritmos: Búsqueda Lineal vs Binaria

## 🎯 Objetivo

Demostrar comprensión de los conceptos fundamentales del análisis de algoritmos, la notación Big O, la complejidad temporal y espacial, y su aplicación práctica en Python mediante la comparación entre dos algoritmos de búsqueda: **lineal** y **binaria**.

---

## ⚙️ Algoritmos Implementados

### 🔍 Búsqueda Lineal (`O(n)`)
Recorre la lista secuencialmente hasta encontrar el objetivo. Su rendimiento depende directamente del tamaño de la lista y de la posición del valor buscado.

### 🔎 Búsqueda Binaria (`O(log n)`)
Funciona solo en listas ordenadas. Divide la lista a la mitad en cada paso, reduciendo drásticamente el número de comparaciones necesarias.

---

## 🧠 Notación Big O

La notación Big O permite describir el **crecimiento del tiempo de ejecución** en función del tamaño de la entrada:

- **O(n)**: crece linealmente → búsqueda lineal.
- **O(log n)**: crece logarítmicamente → búsqueda binaria.

---

## 🧪 Metodología

1. Se generaron listas ordenadas de tamaños `10⁴`, `10⁵` y `10⁶`.
2. Se realizaron búsquedas en tres escenarios:
   - **Mejor caso**: el objetivo está al inicio.
   - **Caso medio**: el objetivo está en el centro.
   - **Peor caso**: el objetivo está al final.
3. Se midió el tiempo de ejecución de cada algoritmo con el módulo `timeit`.
4. Se graficaron los resultados con `matplotlib` usando escala logarítmica en ambos ejes.

---

## 📈 Resultados Obtenidos

![Gráfico de comparación](comparacion_todos_los_casos.png)

### 🔍 Búsqueda Lineal (O(n))

- **Peor caso (línea roja):** tiempo crece linealmente; el objetivo está al final de la lista.
- **Caso medio (naranja):** tiempo medio; el objetivo está a mitad de lista.
- **Mejor caso (verde):** tiempo constante; el objetivo está al inicio.

> 📌 La búsqueda lineal es sensible a la posición del elemento y no escala bien con listas grandes.

### 🔎 Búsqueda Binaria (O(log n))

- Todas las líneas (verde, naranja, roja) son similares y cercanas al eje horizontal.
- Demuestra rendimiento constante sin importar la posición del objetivo.

> 📌 La búsqueda binaria es ideal para listas ordenadas, siendo muy rápida incluso en el peor caso.

---

## 📊 Comparación General

| Característica           | Búsqueda Lineal       | Búsqueda Binaria     |
|--------------------------|------------------------|-----------------------|
| Complejidad temporal     | O(n)                  | O(log n)              |
| Requiere orden previo    | ❌ No                 | ✅ Sí                 |
| Varía por posición       | ✅ Sí                | ❌ No                |
| Escalabilidad            | ❌ Mala               | ✅ Excelente          |

---

## 🖼 Capturas de Pantalla

### 🧾 Código en el editor
![Captura del código](captura_codigo.png)

### 📉 Salida y gráfica
![Gráfico generado](comparacion_todos_los_casos.png)

---

## ✅ Conclusiones

- La búsqueda binaria demuestra una gran eficiencia en cualquier caso siempre que la lista esté ordenada.
- La búsqueda lineal es fácil de implementar y útil en listas pequeñas o desordenadas, pero su rendimiento se degrada rápidamente con el tamaño.
- Las diferencias de rendimiento, mostradas en escalas logarítmicas, confirman las predicciones teóricas de la notación Big O.

---

## 👨‍💻 Autor

**[Claudio Andrés Díaz Vargas]**  
Análisis de Algoritmo y Notación Big O /
Módulo 2 - Clase N° 4
[Año: 2025]

---

