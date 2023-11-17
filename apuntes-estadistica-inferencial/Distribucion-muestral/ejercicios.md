# Prácticas

## EJERCICIO 1: Distribución muestral de medias con VARIANZA CONOCIDA (población)

**PROBLEMA 1:**

El [*valor nominal de la resistencia*](/apuntes-estadistica-inferencial/lista-definiciones.md/#valor-nominal) de una lámina de un
metal compuesto es de 8500 psi. Por estudios pasados se
conoce que la *desviación estándar* de esta resistencia es 1950 psi. Se tiene una muestra de 100 láminas. ¿Cuál es la probabilidad de que la media de esa muestra:

a) Sea mayor a 8900 psi?

b) Sea menor a 8000 psi?

| **DATOS DEL PROBLEMA:**     |
| --------------------------- |
| &mu;=8500                   |
| &sigma;=1950 **(conocida)** |
| n=100                       |

**Variable:** X resistencia de una lámina

**SOLUCIÓN 1.A:**

a. Media mayor que 8900 $(\tilde{x}>8900)$

$$ P(\tilde{x}>8900) = 1 - P(\tilde{x}>8900) $$

**Estandarización:**

- Recordando que

$$ Z = \frac{\tilde{X}-\mu}{\frac{\sigma}{\sqrt{n}}} \sim N(0,1) $$

- Donde &mu; = 0 y &sigma; = 1 para la distribución normal estándar

**Estandarizando:**

$$ 1-P(Z\le\frac{8900-8500}{\frac{1950}{\sqrt{100}}}) $$

- Obtenemos el valor para buscar en la tabla normal estándar (Z):

$$ 1-P(Z\le2.05) $$

$$ \therefore P(\tilde{x}>8900) = 1 - 0.97982 = 0.02018 $$

**SOLUCIÓN 1.B:**

b. Media menor que 8000 ($\tilde{x}<8000$)

$$ P(\tilde{x}<8000) $$

$$ P(Z<\frac{8000-8500}{\frac{1950}{\sqrt{100}}}) $$

$$ P(Z<-2.56) $$

- Usando la tabla normal estándar:

$$ P(Z<-2.56) = 0.0054 $$

## EJERCICIO 2: Distribución mustral de medias con VARIANZA DESCONOCIDA (población)

**PROBLEMA 1:**

Una máquina produce piezas con un tamaño que se ajusta a una [*distribución normal*](/apuntes-estadistica-inferencial/distribucion-muestral.md) cuyo *valor medio* es de 14 cm.

¿Cuál es la probabilidad de que la media de una muestra de tamaño 20 sea menor que 14.58 cm., sabiendo que la varianza muestral ha sido de 9 cm² ?

| Datos del problema               |
| -------------------------------- |
| &mu;=14cm                        |
| S² = 9cm² (&sigma;² desconodida) |
| n=20                             |

**Variable:** X tamaño de una pieza

### SOLUCIÓN 2

Si: $X \sim N(\mu, ??) \rightarrow \tilde{X} \sim N(\mu, \frac{S}{\sqrt{n}})$

- Donde &mu; = 14 y S = 3

Entonces: $\tilde{X} \sim N(14, \frac{3}{\sqrt{20}})$

> Como &sigma;² es desconocida y n < 30, se usa la distribución T-Student

**Piden:**

$$ P(\tilde{x}<14.58) $$

**Recordando que:**

$$ T = \frac{\tilde{X}-\mu}{\frac{S}{\sqrt{n}}} \sim T_{n-1} $$

**Estandarizando:**

$$ P(T_{n-1}<\frac{14.58-14}{\frac{3}{\sqrt{20}}}) $$

**Ojo 👀:**

$$ Z = \frac{\tilde{X}-\mu}{\frac{\sigma}{\sqrt{n}}} \sim N(0,1) $$

**Estandarizando:**

$$ P(T_{19}<1.63) $$

- Usando la tabla T-Student:

$$ P(T_{19}<8646) \cong  0.80 $$

## EJERCICIO 3: Distribución de la diferencia de dos medias muestrales con varianza poblacional conocida (muestra)

**PROBLEMA 1:**

Se tiene la siguiente información de una determinada empresa:

Salario medio hombres $= 129 000 ptas., \sigma 2=2 500$

Salario medio mujeres $= 128 621 ptas., \sigma 2=3 000$

Si tomamos una muestra aleatoria de 36 hombres y 49 mujeres ¿cuál es la *probabilidad de que el salario medio de los hombres sea al menos 400 ptas. mavor al de las mujeres*?

**Datos del problema:**

**Población:**
| Hombres          | Mujeres          |
| ---------------- | ---------------- |
| &mu;1 = 129000$  | &mu;2 = 128621$  |
| &sigma;1 = 2500$ | &sigma;2 = 3000$ |

**Datos de la muestra:**

| Hombres | Mujeres |
| ------- | ------- |
| n1 = 36 | n2 = 49 |

**SOLUCIÓN:**

$X_1$: Salario de hombres

$X_2$: Salario de mujeres

**Se deduce:**

$$ \tilde{X}_{1} - \tilde{X}_{2} \sim N(\mu_{1} - \mu_{2}, \sqrt{\frac{\sigma_1^2}{n_1}+\frac{\sigma_2^2}{n_2}}) $$

**PIDEN:** $P(\tilde{X}_1-\tilde{X}_2) \ge 400$

**Estandarización:**
$$ Z_c = \frac{(\tilde{X}_1-\tilde{X}_2)-(\mu_1-\mu_2)}{\sqrt{\frac{\sigma_1^2}{n_1}+\frac{\sigma_2^2}{n_2}}} \sim N(0,1)$$

**Reemplazando:**

$$ P(Z\ge\frac{400-(129000-128621)}{\sqrt{\frac{2500}{36}+\frac{3000}{49}}})$$

$$ P(Z\ge\frac{400-379}{\sqrt{\frac{57625}{441}}}) $$

$$ P(Z\ge\frac{21}{11.43105132}) $$

$$ P(Z\ge1.84) = 1-P(Z<1.84)$$

- Usando la tabla normal estándar:

$$ P(Z<1.84) = 0.96712 $$

- Reemplazando

$$ P(Z\ge1.84)=1-P(Z<1.84)=1-0.96712 = 0.03288 $$

- La probabilidad de que el salario medio de los hombres sea al menos 400 ptas. mayor al de las mujeres será de 3.3%

**PROBLEMA 2:**

Los cinescopios para la televisión del fabricante A tiene una duración media de 6.5 años y una desviación estándar de 0.9 años, mientras que los del fabricante B tienen una duración media de 6.0 años y una desviación estándar de 0.8 años.

¿Cuál es la probabilidad de que una muestra aleatoria de 25 cinescopios del fabricante A tenga una duración media que sea al menos de un año más que la duración media de una muestra de 26 cinescopios del fabricante B?

**Datos del problema:**

Pasamos las desviaciones estándar a varianzas:

$$ \sigma_1^2 = 0.9^2 = 0.81 $$

$$ \sigma_2^2 = 0.8^2 = 0.64 $$

**Población:**

| Fabricante A                    | Fabricante B                    |
| ------------------------------- | ------------------------------- |
| &mu;1 = 6.5                     | &mu;2 = 6.0                     |
| &sigma;²1 = 0.81 **(conocida)** | &sigma;²2 = 0.64 **(conocida)** |

**Muestra:**

| Fabricante A | Fabricante B |
| ------------ | ------------ |
| n1 = 25      | n2 = 26      |

**SOLUCIÓN:**

$X_1$: Duración de los cinescopios del fabricante A

$X_2$: Duración de los cinescopios del fabricante B

**Se deduce:**

$$ \tilde{X}_{1} - \tilde{X}_{2} \sim N(\mu_{1} - \mu_{2}, \sqrt{\frac{\sigma_1^2}{n_1}+\frac{\sigma_2^2}{n_2}}) $$

**PIDEN:** $P(\tilde{X}_1-\tilde{X}_2) \ge 1$

**Estandarización:**

$$ Z_c = \frac{(\tilde{X}_1-\tilde{X}_2)-(\mu_1-\mu_2)}{\sqrt{\frac{\sigma_1^2}{n_1}+\frac{\sigma_2^2}{n_2}}} \sim N(0,1)$$

**Reemplazando:**

$$ P(Z\ge\frac{1-(6.5-6.0)}{\sqrt{\frac{0.81}{25}+\frac{0.64}{26}}})$$

$$ P(Z\ge\frac{1-0.5}{\sqrt{\frac{0.81}{25}+\frac{0.64}{26}}})$$

$$ P(Z\ge\frac{0.5}{\sqrt\frac{1853}{32500}})$$

$$ P(Z\ge\frac{0.5}{0.2387789451})$$

$$ P(Z\ge2.093) $$

$$ 1-P(Z<2.09) $$

- Usando la tabla normal estándar:

$$ P(Z<2.09) = 0.98169 $$

- Reemplazando

$$ P(Z\ge2.09)=1-P(Z<2.09)=1-0.98169 = 0.01831 $$

## EJERCICIO 4: Distribución de la diferencia de dos medias muestrales con VARIANZA POBLACIONAL DESCONOCIDA (muestra)

**PROBLEMA 1:** $\sigma^2_1=\sigma^2_2=\sigma^2$

Se realiza una investigación sobre la calidad del aire en Av. Abancay y Wilson. Un indicador de la calidad es el número de partículas en suspensión por $m^3$ de aire, que se asume siguen distribuciones Normales independientes de media 62.037 en Av. Abancay, 61.022 en Av. Wilson.

En la primera Avenida se realizan 12 mediciones, obteniéndose una varianza de 8.44 y en la segunda 15 mediciones, con una varianza de 9.44.

Obtener la probabilidad de que la media muestral de Av. Abancay sea como mínimo tres unidades mayor a la media muestral de Av. Wilson. [**Considere homogeneidad de varianzas.**](/apuntes-estadistica-inferencial/distribucion-muestral.md/#caso-a-⚠-las-varianzas-poblacionales-son-desconocidas-pero-iguales)

**Datos del problema:**

**Población:**

| Av. Abancay    | Av. Wilson     |
| -------------- | -------------- |
| &mu;1 = 62.037 | &mu;2 = 61.022 |

**Muestra:**

| Av. Abancay | Av. Wilson |
| ----------- | ---------- |
| n1 = 12     | n2 = 15    |
| S²1 = 8.44  | S²2 = 9.44 |

**SOLUCIÓN:**

$X_1$: Número de partículas en suspensión por $m^3$ de aire en Av. Abancay

$X_2$: Número de partículas en suspensión por $m^3$ de aire en Av. Wilson

- Piden calcular:

$$ P(\tilde{X}_1-\tilde{X}_2 > 3 )= ?$$

- La probabilidad de que la media muestral de Av. Abancay sea como mínimo tres unidades superior a la media muestral de Av. Wilson.

**PIDEN:**

$$ P(\tilde{X}_1-\tilde{X}_2 > 3)$$

**Correccion de T-Student:** Estandarización

$$ T=\frac{(\tilde{X}_1-\tilde{X}_2)-(\mu_1-\mu_2)}{\sqrt{S_p^2\cdot(\frac{1}{n_1}+\frac{1}{n_2})}} \sim t_{n_1+n_{2-2}} $$

- Donde $S_p^2$ es la varianza conjunta de las muestras

$$ S_p^2 = \frac{(n_1-1)\cdot S_1^2+(n_2-1)\cdot S_2^2}{n_1+n_2-2} $$

**Reemplazando:**

$$ S_p^2 = \frac{(12-1)\cdot 8.44+(15-1)\cdot 9.44}{12+15-2} $$

$$ S_p^2 = \frac{92.84+132.16}{25} $$

$$ S_p^2 = \frac{225}{25} $$

$$ S_p^2 = 9 $$

**Estandarizando:**

$$ P(\tilde{X}_1-\tilde{X}_2 > 3) \rightarrow P(t_{n_1+n_{2-2}}>\frac{3-(62.037-61.22)}{\sqrt{(9)(\frac{1}{12}+\frac{1}{15})}})$$

$$ \rightarrow P(t_{12+15-2}>\frac{1.985}{\sqrt{(9)(\frac{3}{20})}} $$

$$ \rightarrow P(t_{12+13}>\frac{1.985}{\sqrt{1.35}}) $$

$$ \rightarrow P(t_{25}>1.708) $$

$$ 1-P(t_{25}\le1.708) $$

- Usando la tabla T-Student:

$$ P(t_{25}\le1.708) = 0.950 $$

- Reemplazando

$$ P(t_{25}>1.708)=1-P(t_{25}\le1.708)=1-0.950 = 0.050 $$

**PROBLEMA 2:** $\sigma^2_1 \neq \sigma^2_2$

Un equipo de psicólogos está investigando si existen o no diferencias entre dos métodos de relajación para reducir la ansiedad. Para lo cual se seleccionan dos muestras de tamaño 10 cada una, a las que se les aplico el método **X** e **Y** respectivamente. Obteniéndose que las varianzas muéstrales son de 3.7 y 4.2 puntos respectivamente. Suponiendo que las puntuaciones de ansiedad de ambas poblaciones siguen distribuciones muéstrales con medias poblacionales de 90 y 87.3 puntos respectivamente y que [**las varianzas poblacionales son desconocidas pero se sabe que son diferentes**](/apuntes-estadistica-inferencial/distribucion-muestral.md/#caso-b-⚠-las-varianzas-poblacionales-son-desconocidas-y-diferentes). Hallar la probabilidad de la media muestral de puntuación del método **X** sea como mínimo 6 unidades mayor que el método **Y**.

**Datos del problema:**

**Población:**

| Método X   | Método Y     |
| ---------- | ------------ |
| &mu;1 = 90 | &mu;2 = 87.3 |

**Muestra:**

| Método X  | Método Y  |
| --------- | --------- |
| n1 = 10   | n2 = 10   |
| S²1 = 3.7 | S²2 = 4.2 |

**SOLUCIÓN:**

$X_1$: Puntuación de ansiedad del método X

$X_2$: Puntuación de ansiedad del método Y

**PIDEN:**

$$ P(\tilde{X}_1-\tilde{X}_2 > 6)$$

**Corrección de T-Student:** Estandarización

$$ T=\frac{(\tilde{X}_1-\tilde{X}_2)-(\mu_1-\mu_2)}{\sqrt{\frac{S_1^2}{n_1}+\frac{S_2^2}{n_2}}} \sim t_{v} $$

- Donde $v$ es el grado de libertad

$$ v = \frac{(\frac{S_1^2}{n_1}+\frac{S_2^2}{n_2})^2}{\frac{(\frac{S_1^2}{n_1})^2}{n_1-1}+\frac{(\frac{S_2^2}{n_2})^2}{n_2-1}} $$

**Reemplazando:**

$$ v = \frac{(\frac{3.7}{10}+\frac{4.2}{10})^2}{\frac{(\frac{3.7}{10})^2}{10-1}+\frac{(\frac{4.2}{10})^2}{10-1}} $$

$$ v = \frac{(\frac{79}{100})^2}{\frac{0.1369}{9}+\frac{0.1764}{9}} $$

$$ v = \frac{0.6241}{\frac{3133}{90000}} $$

$$ v = 17.92818385 \approx 18 $$

**Estandarizando:**

$$ P(\tilde{X}_1-\tilde{X}_2 > 6) \rightarrow P(t_{18}>\frac{6-(90-87.3)}{\sqrt{\frac{3.7}{10}+\frac{4.2}{10}}}) $$

$$ \rightarrow P(t_{18}>\frac{6-2.7}{\sqrt{0.37+0.42}}) $$

$$ \rightarrow P(t_{18}>\frac{3.3}{0.8888194417}) $$

$$ \rightarrow P(t_{18}>3.712790073) $$

$$ 1-P(t_{18}\le3.71) $$

- Usando la tabla T-Student:

$$ P(t_{18}\le3.71) = 0.995 $$

- Reemplazando

$$ P(t_{18}>3.71)=1-P(t_{18}\le3.71)=1-0.995 = 0.005 $$

## EJERCICIO 5: Distribución Muestral de la proporción

**PROBLEMA 1:**

Una máquina fabrica piezas para autos. En su producción habitual, se fabrica 3 piezas defectuosas de cada 100 piezas. Un cliente recibe una caja de 500 piezas procedentes de la fábrica. Calcular la probabilidad de que haya más de un 5% de piezas defectuosas en la caja.

| Datos del problema |
| ------------------ |
| &pi; = 0.03        |
| n = 500            |

**SOLUCIÓN:**

**Estandarización:**

$$ Z=\frac{p-\pi}{\sqrt{\frac{\pi\cdot(1-\pi)}{n}}} $$

- Donde:
- $P$ es la proporción de piezas defectuosas en la población y $n$ es el tamaño de la muestra

**Estandarizando:**

$$ P(P>0.05) \rightarrow P(Z>\frac{0.05-0.03}{\sqrt{\frac{0.03(1-0.03)}{500}}}) $$

$$ \rightarrow P(Z>\frac{0.02}{\sqrt{\frac{0.03(0.97)}{500}}}) $$

$$ \rightarrow P(Z>\frac{0.02}{\sqrt{\frac{0.0291}{500}}}) $$

$$ \rightarrow P(Z>\frac{0.02}{0.007628892449}) $$

$$ \rightarrow P(Z>2.621612526) $$

$$ 1-P(Z\le2.62) $$

- Usando la tabla normal estándar:

$$ P(Z\le2.62) = 0.996 $$

- Reemplazando

$$ P(Z>2.62)=1-P(Z\le2.62)=1-0.996 = 0.004 $$
