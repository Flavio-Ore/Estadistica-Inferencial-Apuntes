# Metodología de Prueba de Hipótesis

Es la posible respuesta a un problema.

**Pongamos en duda lo siguiente: ¿Cerá cierto?**

- "Los niños que comen pescado azul durante seis meses mostrarán un coeficiente intelectual mayor que los que no lo hacen".
- "El consumo de tabaco en los primeros años de la adolescencia es cuatro veces más nocivo que en la adultez".
- "Los automóviles de la actualidad consumen 20% más de energía que los de hace veinte años".
- "No existe diferencia en los niveles de ansiedad entre niños con coeficientes intelectuales altos y aquellos que tienen coeficientes intelectuales bajos".

**HIPÓTESIS ESTADíSTlCA:**
La prueba de hipótesis comienza con una *suposición*, denominada hipótesis, que hacemos entorno a un  **parámetro** (&theta;) de la población,

Principalmente sobre:

- ✔ media (&mu;)
- ✔ varianza (&sigma;²)
- ✔ proporción (p)

**¡¡Es muy sencillo!!:**

Reunimos **datos muéstrales**, producimos **estadísticos** de la muestra y *con esta información decidimos la* **probabilidad** *que el* **parámetro supuesto** de la población sea correcto.

La hipótesis se prueban con **evidencias** en estadística una buena evidencia es una muestra estadística.

## Tipos de Hipótesis

### Hipótesis Nula ($H_0$)

Es la creencia a priori o lo que sucede actualmente, **no se rechaza** a menos que los datos muestrales prueben lo contrario.

Se mantiene el efecto. Emplea los signos igual, mayor o igual o menor o igual ($=, \le, \ge$)

### Hipótesis Alterna ($H_1$)

*Sospechamos* que hay un cambio que posiblemente sea cierto, por lo tanto es la hipótesis que espera **el investigador** sea cierto.

Si hay un cambio (hay efecto) entonces. Emplea los signos diferente, mayor o menor ($\neq, < ó >$).

**Nota:** Las hipótesis nula y alterna, se refieren ambas a la misma población(es), por lo tanto, si se rechaza la hipótesis nula, se acepta la hipótesis alterna. $\mu, \sigma^2, \pi$

### Observaciones

✔ La hipótesis nula es siempre la hipótesis que se prueba entonces:

✔ Un **estadístico de prueba** entonces:

1. Que la $H_0$ se rechace y la $H_1$ se acepte. $H_0: \theta =\theta_0$
2. No se rechace la $H_0$ en base a la evidencia. $H_0: \theta \neq \theta_0$

✔ **Aceptar** la hipótesis alterna alternativa *conducirá a cambios de opiniones o acciones*, ya que se está probando que si hay un efecto

**Nota:** Si la Hipótesis nula no se rechaza, no significa se acepte como válida (no hay evidencia).

**Ejemplo 1:**

Una empresa de Marketing Industrial está considerando la introducción de un nuevo plan de servicio para piezas hidráulicas, el plan será prese tad si se prefiere por mas del 40% de los clientes:

**Lenguaje Estadístico**:

$$ H_0 : \pi \le 40\% $$

$$ H_1 : \pi > 40\% \leftarrow \text{lo que el investigador espera} $$

Si se rechaza la Hipótesis nula $H_0$, se aceptará la alterna $H_1$ se introducirá el nuevo servicio si no se puede rechazar la hipótesis nula $H_0$, el nuevo plan de servicio no debería introducirse a menor que se obtenga una evidencia adicional

Esta prueba tiene una dirección (mayor 40%), por lo tanto es una prueba de una cola superior

**Ejemplo 2:**

Un ingeniero Industrial tiene como objetivo mejorar la calidad de sus frascos producidos, para ello el diámetro de la tapa de frascos en la producción de lotes debe tener una variabilidad que deben ajustarse. La medida aproximada que se ha mantenido siempre es 0.35 cm

**Lenguaje Estadístico**:

$$ H_0 : \sigma^2 = 0.35cm $$

$$ H_1 : \sigma^2 < 0.35cm (\text{mejorar la calidad}) $$

En estudios previos, se ha determinado que el nivel de colesterol de pacientes con problemas cardíacos es 220. Un cardiólogo piensa que en realidad el nivel es más alto.

**Lenguaje Estadístico**:

$$ H_0 : \mu \le 220 $$

$$ H_1 : \mu > 220 (\text{el nivel es más alto de colesterol}$$

**Ejemplo 3:**

Un proyecto de investigación pretende, entre sus objetivos, determinar si los datos presentan suficiente evidencia para indicar que **nivel medio de hematocrito en hombres nadadores es menor de 44,5%** en una muestra de 29 sujetos de esta población. Para cumplir este objetivo se debe probar con un nivel de significancia de 5%.

**Lenguaje Estadístico**:

$$ H_0 : \mu \ge 44.5 $$

$$ H_1 : \mu < 44.5 $$

## Tipos de Errores

Ninquna prueba de hipótesis es 100% cierta. Puesto que la prueba se basa en probabilidades, siempre existe la posibilidad de lleqar a una conclusión incorrecta. Cuando usted realiza una prueba de hipótesis, puede cometer dos tipos de error: tipo I y tipo II.

> [Fuente](www.minitab.com)

- $H_0: \text{No hay embarazo}: \text{En hombres es imposible, se vuelve error tipo 1 falso positivo}$
- $H_1: \text{No hay embarazo}: \text{Se observa claramente que la mujer está embarazada, se vuelve error tipo 2 falso negativo}$

### Error tipo I

**Rechazar una Hipótesis Nula cuando es cierta.**

$$ \alpha = P(\text{Error tipo I}) = P(\text{Rechazar } H_0 / H_0 \text{ es cierta}) $$

Si usted rechaza la hipótesis nula cuando es verdadera, comete un error de tipo I. La probabilidad de cometer un error de tipo I es &alpha;, que es el **nivel de significancia** que usted establece para su prueba de hipótesis. Un de 0.05 indica que usted está dispuesto a aceptar una probabilidad de 5% de estar equivocado al rechazar la hipótesis nula.

**Recuerda:**

- ✔ El nivel de confianza (1 - &alpha;) es 95% -> el nivel de significancia (&alpha;) es 5%.
- ✔ El nivel de confianza (1 - &alpha;) es 90% -> el nivel de significancia (&alpha;) es 10%.

### Error Tipo II

**Aceptar (no rechazar) una Hipótesis Nula cuando es falsa.**

$$ \beta = P(\text{Error tipo II}) = P(\text{No rechazar } H_0 / H_0 \text{ es falsa}) $$

Cuando la hipótesis nula es falsa y usted no la rechaza, comete un error de tipo II. La probabilidad de cometer un error de tipo II es &beta;.

### Potencia de prueba

Es igual a $1 - \beta$, es la probabilidad de rechazar la hipótesis nula cuando es falsa.

Al tomarse una decisión respecto a una hipótesis nula ($H_0$), se puede presentar **cuatro posibles casos** que determinan si la decisión tomada es correcta o incorrecta esto se presenta en la siguiente tabla:

|    Decisión    |    $H_0$ es verdadera    |     $H_0$ es falsa      |
| :------------: | :----------------------: | :---------------------: |
| Aceptar $H_0$  |    Decisión correcta     |      Error tipo II      |
|                | Probabilidad 1 - &alpha; |  Probabilidad = &beta;  |
| Rechazar $H_0$ |       Error tipo I       |    Decisión correcta    |
|                |  Probabilidad = &alpha;  | Probabilidad 1 - &beta; |

## Procedimiento para realizar una Prueba de Hipótesis

|      Prueba Bilateral       | Prueba Unilateral Inferior | Prueba Unilateral Superior |
| :-------------------------: | :------------------------: | :------------------------: |
|  $H_0: \theta = \theta_0$   | $H_0: \theta \ge \theta_0$ | $H_0: \theta \le \theta_0$ |
| $H_1: \theta \neq \theta_0$ |  $H_1: \theta < \theta_0$  |  $H_1: \theta > \theta_0$  |

1. Paso 1: Plantear la hipótesis (1 población, 2 poblaciones)
2. Paso 2: Fijar nivel de significación $\alpha = (0.05, 0.01, 0.10)$
3. Paso 3: Identificar el estadístico de prueba $Z, t, \chi^2, etc$
4. Paso 4: Formular una regla de decisión $\rightarrow$ Establecer la regla de decisión bajo las cuales se rechaza o no $H_0$
5. Paso 5: Decisión $\rightarrow$ Tomar decisión en base a la evidencia muestral
6. Paso 6: Conclusión $\rightarrow$ La conclusión se expresa en función del problema.

## Prueba de hipótesis para la MEDIA POBLACIONAL

### Paso 1

Planteamiento de la hipótesis.

![Prueba de hipotesis](/apuntes-estadistica-inferencial/prueba-de-hipotesis/graf-de-h0.png)

### Paso 2

Establecer el nivel de significancia ($\alpha$), el cual puede ser: $0.05, 0.01, 0.10, etc$

### Paso 3

Estadístico de prueba

$$ \mu_{hip}=\mu_0 $$

#### Caso 1: Varianza poblacional conocida

$$ Z_c = \frac{\bar{x} - \mu_{hip}}{\frac{\sigma}{\sqrt{n}}} $$

#### Caso 2: Varianza poblacional desconocida y tamaño de muestra pequeño ($n < 30$)

$$ T_c = \frac{\bar{x} - \mu_{hip}}{\frac{S}{\sqrt{n}}} $$

- Grados de libertad: $n - 1$

#### Caso 3: Si la varianza es desconocida y tamaño de muestra grande ($n \ge 30$), se puede utilizar la distribución normal estándar

$$ Z_c = \frac{\bar{x} - \mu_{hip}}{\frac{S}{\sqrt{n}}} $$

### Paso 4: Región de rechazo de $H_0$ ($RH_0$) y región de no rechazo de $H_0$ ($NRH_0$)

![Rechazo o aceptacion de hipotesis](/apuntes-estadistica-inferencial/prueba-de-hipotesis/zona-de-rechazo-h0.png)

Primero es bilateral, la sumatoria de las colas es igual a $\alpha$. Y la sumatoria total de todo el gráfico es igual a 1.

### Paso 5: Decisión Estadística

Con los datos de la muestra, hallar el valor del estadístico de prueba $Z$ o $T$ y compararlo con el valor crítico $Z_{cal}$ o $T_{cal}$.

- **Rechazar $H_0$**: Si $Z_{cal}$ o $T_{cal}$ se encuentra en la región de rechazo $RH_0$
- **No rechazar $H_0$**: Si $Z_{cal}$ o $T_{cal}$ se encuentra en la región de no rechazo $NRH_0$
