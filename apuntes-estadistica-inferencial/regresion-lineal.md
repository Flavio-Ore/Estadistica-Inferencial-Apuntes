# Regresión Lineal

La comprensión de un resorte depende la fuerza que se le aplique a aquel según los valores del siguiente cuadro:

| Fuerza (Newton) | Compresión (cm) |
| --------------- | --------------- |
| 1               | 2               |
| 0               | 1               |
| 2               | 2               |
| 3               | 2               |
| 4               | 3               |

1. Halle el coeficiente de correlación y determinación
2. Interprete cada uno de ellos

**SOLUCIÓN:**

- Variables de Interés:

  - $X$: Fuerza (Newton)
  - $Y$: Compresión (cm)

**Paso 1: Calcular la pendiente (m) y la intersección (b):**

<--! Agrega los dólares para que esté representada matemáticamente:-->
$$ m = \frac{(5 \times 23) - (10 \times 10)}{(5 \times 14) - 10^2} = \frac{115 - 100}{70 - 100} = \frac{15}{-30} = -0.5 $$

$$ b = \frac{1}{5} \times (23 - (-0.5 \times 14)) = \frac{1}{5} \times (23 - (-7)) = \frac{1}{5} \times 30 = 6 $$

Por lo tanto, la ecuación de regresión lineal es $y = -0.5x + 3$.

**Paso 2: Calcular el coeficiente de correlación (r):**

$$ r = \frac{5 \times 23 - 10 \times 10}{\sqrt{(5 \times 14 - 10^2)(5 \times 23 - 10^2)}} = \frac{115 - 100}{\sqrt{(70 - 100)(115 - 100)}} = \frac{15}{\sqrt{(-30)(15)}} = \frac{15}{\sqrt{-450}} = \frac{15}{-21.21} = -0.707 $$

**Paso 3: Calcular el coeficiente de determinación (r²):**

$$ r^2 = (-0.707)^2 = 0.5 $$

Por lo tanto, el coeficiente de correlación ($r$) es aproximadamente $0.122$ y el coeficiente de determinación ($r^2$) es aproximadamente $0.015$. Esto significa que aproximadamente el $1.5%$ de la variabilidad en la compresión puede ser explicada por la variabilidad en la fuerza aplicada. En términos simples, el modelo de regresión lineal no explica mucho de la variabilidad en los datos. Esto podría sugerir que hay otros factores que afectan la compresión que no están siendo tenidos en cuenta en este modelo.
