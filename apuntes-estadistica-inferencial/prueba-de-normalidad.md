# Prueba de normalidad

Para conseguir si la distribución de datos se ajusta a una distribución normal teórica.

## 1. Prueba de Kolmogorov-Smirnov

1. $H_{0}$: Los datos siguen una [D.N.E](/lista-definiciones.md/#41-tabla-distribución-normal-estandarizada-tabla-z)
2. $H_{1}$: Los datos [**NO** siguen una D.N.E](/lista-definiciones.md/#fórmula-de-proceso-de-estandarización-🔋), no tienen [curva normal](/lista-definiciones.md/#curva-normal)

## 2. Errores conocidos

$$ \alpha = \{0,01; 0,05; 0,1\}$$

## 3. Estadístico de Prueba

Arsenal matemático para determinar si los datos tienen [curva normal](/lista-definiciones.md/#curva-normal) o **NO**.

$$ D = \displaystyle \sup_{1 \le i \le n}|\hat{F}_{n}(x_{i}) - F_0(x_{i})| $$

Donde:

- **$Xi$**: Es el i-ésimo valor observado en la muestra (Cuyos valores se han ordenado previamente de mayor menor)
- **$F_{n}(x_{i})$**: Es un estimador de la probabilidad de observar valores menores o iguales a $x_{i}$
- **$F_{o}(x_{i})$**: Es la probabilidad de observar valores menores o iguales que $x_{i}$ cuando $H_{0}$ es cierta

Así pues $D$ es la mayor diferencia absoluta entre la frecuencia acumulada observada $F_{o} (x_{i})$ y la frecuencia acumulada teórica $F_{o}(x_{i})$ obtenina a partir de la probabilidad que se especifica como Hipótesis Nula.

Para efectos prácticos:

$$ D^{+} = \max_{1 \le i \le n}\{ \frac{i}{n} - F_{0}(x_{i}) \}$$

$$D^{-} = \max_{1 \le i \le n}\{ F_{0}(x_{i}) - \frac{i - 1}{n} \}$$

Por tanto, a partir de estos valores $D = \max \{D^+, D^-\}$

## Por tanto el criterio para rechazar o aceptar la prueba de hipótesis es la siguiente

Si $D \le D_{\alpha} \rightArrow$ Aceptar $H_{0}$

Si $D > D_{\alpha} \rArr Rechazar H_{0}$

Donde $D_{a} = \frac{C_{\alpha}}{k(n)}$

$C_{\alpha}$ podrá tomar los siguientes valores:

| C&alpha; |       | &alpha; |       |
| -------- | ----- | ------- | ----- |
| Modelo   | 0,1   | 0,5     | 0,9   |
| General  | 1,224 | 1,358   | 1,628 |
| Normal   | 0,819 | 0,895   | 1,035 |

$K(n)$ podrá tomar los siguientes valores:

Normal:

$$ K(n) = \sqrt{n} - 0,01 + \frac{0,85}{\sqrt{n}}$$

### Ejemplo N.1

Se tienen los ingresos de un grupo de 10 ingenieros egresado de la UTP, los cuales se presentan a continucación (en miles):

`6,0; 2,3; 4,8; 5,6; 4,5; 3,4; 3,3; 1,9; 4,8; 4,5`

Probar que los sueldos se ajustan a una distribución normal con un nivel de significación de &alpha; = 0,05

**Solución:**

1. $H_{0}$: Los Sueldos siguen una [D.N.E](/apuntes-estadistica-inferencial/distribucion-muestral.md/#caso-1-población-con-distribución-normal)
2. $H_{1}$: Los Sueldos [**NO** siguen una D.N.E](/apuntes-estadistica-inferencial/distribucion-muestral.md/#caso-2-población-con-distribución-no-normal)

&alpha; = 0,05

$\tilde{x} = 4,1, S = 1,34$

A partir de la definición se construye la siguiente tabla: donde $\tilde{x} = 4,1, S = 1,34$

| Y   | Y-sorted | Orden | F   | Z      | Fo    | D+      | D-     |
| --- | -------- | ----- | --- | ------ | ----- | ------- | ------ |
| 6,0 | 1,9      | 1     | 0,1 | -1,628 | 0,051 | 0,049   | 0,051  |
| 2,3 | 2,3      | 2     | 0,2 | -1,332 | 0,091 | 0,109   | -0,009 |
| 4,8 | 3,3      | 3     | 0,3 | -0,592 | 0,276 | 0,024   | 0,076  |
| 5,6 | 3,4      | 4     | 0,4 | -0,518 | 0,302 | 0,098   | 0,002  |
| 4,5 | 4,5      | 5     | 0,5 | 0,296  | 0,616 | -0,116* | 0,216* |
| 3,4 | 4,5      | 6     | 0,6 | 0,296  | 0,616 | -0,016  | 0,116  |
| 3,3 | 4,8      | 7     | 0,7 | 0,518  | 0,698 | -0,002  | 0,098  |
| 1,9 | 4,8      | 8     | 0,8 | 0,518  | 0,698 | -0,102  | -0,002 |
| 4,8 | 5,6      | 9     | 0,9 | 1,11   | 0,867 | -0,033  | 0,067  |
| 4,5 | 6,0      | 10    | 1,0 | 1,406  | 0,920 | -0,080  | 0,020  |

> Si $D \le D_{\alpha}$, entonces se **acepta** $H_{0}$
>
> Si $D > D_{\alpha}$, entonces se **rechaza** $H_{0}$

Los cálculos para la primera fila será:

$$ Z = \frac{Y_{1}-x}{D} = \frac{1,9 - 4,1}{1,34} = -1,628 $$

- Buscar en la tabla el valor de -1,6 en la columna de la izquierda y 0,02 en la fila superior
- El valor de la tabla es 0,051

$$ Fo = P(Z =- 1,628) = 0,051 $$

$$ D_{1}^+ = 0,1-0,051 = 0,049 $$

$$ D_{1}^- = 0,051 - 0 = 0,051 $$

- El resultado del máximo valor en **valor absoluto** de la tabla, entre la fila de los D+ y D- es respectivamente |-0.116| y |0,216|. ❗
- Usando valor absoluto, se obtiene que el valor máximo es 0,216

$$ D = \max \{D^+, D^-\} = \max \{0,049, 0,051\} = 0,216 $$

- Véase [Criterio para rechazar o aceptar la prueba de hipótesis](#por-tanto-el-criterio-para-rechazar-o-aceptar-la-prueba-de-hipótesis-es-la-siguiente)

$$ D_{a} = \frac{0,895}{\sqrt{10}-0,01+\frac{0,85}{\sqrt{10}}} = \frac{0,895}{3,42} = 0,262 $$

**Conclusión:**

Como $D < D\alpha$, se puede concluir que los sueldos de los ingenieros de la UTP se ajustan a una [distribución Normal](/apuntes-estadistica-inferencial/lista-definiciones.md/#41-tabla-distribución-normal-estandarizada-tabla-z).

Es decir que aceptamos la hipótesis nula [$H_{0}$](#por-tanto-el-criterio-para-rechazar-o-aceptar-la-prueba-de-hipótesis-es-la-siguiente), es decir que tiene una [distribución normal](/apuntes-estadistica-inferencial/lista-definiciones.md/#41-tabla-distribución-normal-estandarizada-tabla-z)
