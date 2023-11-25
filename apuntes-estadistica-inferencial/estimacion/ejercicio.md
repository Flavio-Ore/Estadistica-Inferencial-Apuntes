# Prácticas

## EJERCICIO 1: Intervalo de confianza de la MEDIA con VARIANZA CONOCIDA

**PROBLEMA 1:**

Un fabricante produce focos que tienen un *promedio de vida de distribución normal* y una desviación estándar de 40 horas. Si una muestra de 30 focos tiene una vida promedio de 780 horas.

a) Encuentre el *intervalo de confianza* del 95% para la media de la población de todos los focos que produce la empresa.

b) Que tan grande se requiere que sea una muestra. Si se desea tener una confianza del 95% de la media poblacional, que esté dentro de las 10 horas del romedio real.

**Datos del problema:**

**Población:**

- $\mu = ?$
- &sigma; = 40 horas (CONOCIDO)

**Muestra:**

- $n = 30$
- $\bar{X} = 780$

**Nivel de Confianza:**

- $1 - \alpha = 0.95$
- $\alpha = 0.05$

**SOLUCIÓN:**

- $X$: variable aleatoria tiempo de vida de focos fabricados
- $X$: $N(\mu; \sigma^2)$

**Intervalo de Nivel de Confianza:**

$$ IC = \left(\bar{X} - Z_{1 - \alpha/2} \frac{\sigma}{\sqrt{n}} \le \mu \le \bar{X} + Z_{1 - \alpha/2} \frac{\sigma}{\sqrt{n}}\right) $$

**Reemplazando:**

$$ Z_{1 - \alpha/2} = Z_{1 - 0.05/2} = Z_{0.975}$$

$$ IC = \left(780 - Z_{0.975} \frac{40}{\sqrt{30}} \le \mu \le 780 + Z_{0.975} \frac{40}{\sqrt{30}}\right) $$

- Usando tabla Z

$$ Z_{0.975} = 1.96 $$

- Reemplazando

$$ IC = \left(780 - 1.96 \frac{40}{\sqrt{30}} \le \mu \le 780 + 1.96 \frac{40}{\sqrt{30}}\right) $$

$$ IC = (780 - 1.96 \cdot 7.302967433 \le \mu \le 780 + 1.96 \cdot 7.302967433) $$

$$ IC = \left(765.69 \le \mu \le 794.31\right) $$

**Respuesta:**

Con un nivel de Confianza del 95%, el tiempo de vida promedio de los focos está comprendido desde 765.69 horas hasta 794.31 horas.

**Cálculo del error:**

Adicionalmente podemos calcular el error y el tamaño de muestra que aproximadamente será la misma.

**Error:**

$$ e = Z_{1 - \alpha/2} \frac{\sigma}{\sqrt{n}} $$

$$ e = 1.96 \frac{40}{\sqrt{30}} $$

$$ e = 14.3138 $$

**Tamaño de muestra:**

$$ n \ge \left[\frac{Z_{1 - \alpha/2} \cdot \sigma}{e}\right]^2 $$

- Reemplazando

$$ n \ge \left[\frac{1.96 \cdot 40}{14.3138}\right]^2 $$

$$ (5.48)^2 $$

$$ n \ge 30.0001 $$

Se necesita una muestra de 30 focos para estimar la media de la población y tener un error máximo de 14 horas.

El error(e) es muchas veces dato del problema o es fijado por el investigador!!

**PROBLEMA 2:**

La empresa AUTOZIN produce partes de componentes cilíndricos para la industria automotriz que tienen un promedio de diámetro de 5 milímetros con una distribución normal y una desviación estándar de 0.1 milímetros. Para confirmar esto; se tomo una muestra de 25 partes seleccionadas al azar que muestra que el diámetro promedio es de 5.027 milímetros. Encuentre el intervalo de confianza del 95% para la media de la población de todas las partes de componentes cilíndricos que produce la empresa.

**Datos del problema:**

**Población:**

- $\mu = ?$
- &sigma; = 0.1 milímetros (CONOCIDO)

**Muestra:**

- $n = 25$
- $\bar{X} = 5.027$

**Nivel de Confianza:**

- $1 - \alpha = 0.95$
- $\alpha = 0.05$

**SOLUCIÓN:**

- $X$: variable aleatoria diámetro de partes de componentes cilíndricos
- $X$: $N(\mu; \sigma^2)$

**Intervalo de Confianza:**

$$ IC = \left(\bar{X} - Z_{1 - \alpha/2} \frac{\sigma}{\sqrt{n}} \le \mu \le \bar{X} + Z_{1 - \alpha/2} \frac{\sigma}{\sqrt{n}}\right) $$

- Hallando el valor de Z

$$ Z_{1 - \alpha/2} = Z_{1 - 0.05/2} = Z_{0.975}$$

- Usando tabla Z

$$ Z_{0.975} = 1.96 $$

**Reemplazando:**

$$ IC = \left(5.027 - 1.96 \frac{0.1}{\sqrt{25}} \le \mu \le 5.027 + 1.96 \frac{0.1}{\sqrt{25}}\right) $$

$$ IC = (5.027 - 1.96 \cdot 0.02 \le \mu \le 5.027 + 1.96 \cdot 0.02) $$

$$ IC = \left(4.9878 \le \mu \le 5.0662\right) $$

**Respuesta:**

Con un nivel de confianza del 95%, el diámetro promedio de las partes de componentes cilíndricos está comprendido desde 4.987 milímetros hasta 5.067 milímetros.

## EJERCICIO 2: Intervalo de confianza de la MEDIA con VARIANZA DESCONOCIDA

**PROBLEMA 1:**

Una compañía utiliza baterías en sus juegos electrónicos que según ellos duran un **promedio de 30 horas**, para confirmar esto se prueba 16 baterías siendo la media muestral de 27.5 horas y su desviación estándar S=5 horas. Encuentre un intervalo de confianza del 95% para la media. Suponga que la distribución de las duración de las baterías es aproximadamente normal.

**Datos del problema:**

Se aproxima a una curva normal. Cuando no es normal, se vienen otras técnicas...

**Población:**

- $\mu = 30$
- &sigma; = ? (DESCONOCIDO)
  
**Muestra:**

- $n = 16$
- $\bar{X} = 27.5$
- $S = 5$

**Nivel de Confianza:**

- $1 - \alpha = 0.95$
- $\alpha = 0.05$

**SOLUCIÓN:**

- $X$: V.A duración de la bateria

**Intervalo de Confianza:**

$$ IC=\left(\bar{X}-T_{1-\alpha/2, gl}\frac{S}{\sqrt{n}} \le \mu \le \bar{X}+T_{1-\alpha/2, gl}\frac{S}{\sqrt{n}}\right)$$

$$ IC=\left(\bar{X}-T_{1-\alpha/2, gl}\frac{S}{\sqrt{n}} \le \mu \le \bar{X}+T_{1-\alpha/2, gl}\frac{S}{\sqrt{n}}\right)$$

- Hallando el valor de T

$$ T_{1 - \alpha/2, gl} = T_{1 - 0.05/2, 15} = T_{0.975, 15}$$

- Usando tabla T

$$ T_{0.975, 15} = 2.1318 $$

**Reemplazando:**

$$ IC = \left(27.5 - 2.1318 \frac{5}{\sqrt{16}} \le \mu \le 27.5 + 2.1318 \frac{5}{\sqrt{16}}\right) $$

$$ IC = (27.5 - 2.1318 \cdot 1.25 \le \mu \le 27.5 + 2.1318 \cdot 1.25) $$

$$ IC = \left(24.84 \le \mu \le 30.16\right) $$

**Respuesta:**

Con un nivel de confianza del 95%, la duración promedio de las baterías está comprendido desde 24.84 horas hasta 30.16 horas.

## EJERCICIO 3: Intervalo de confianza para LA DIFERENCIA DE MEDIAS MUESTRALES  con VARIANZA POBLACIONAL CONOCIDA

**PROBLEMA 1:**

En un estudio para determinar el gasto medio mensual en arbitrios en las ciudades A y B con desviaciones estándar
de 15 y 10 soles respectivamente. Se toma una muestra al azar de 200 hogares de A arrojando un gasto medio de S/250. Una muestra al azar de 180 hogares de la ciudad B da una gasto medio de 235.

1. Determine un intervalo de confianza del 99 % para la diferencia del gasto medio en las ciudades A y B.
2. ¿Es diferente el gasto medio mensual en arbitrios en las ciudades A y B?

**Datos del problema:**

**Población:**

- A: $\sigma_1$ = 15 soles (CONOCIDO)
- B: $\sigma_2$ = 10 soles (CONOCIDO)

**Muestra:**

- A: $n_1 = 200$, $\bar{X}_1 = 250$
- B: $n_2 = 180$, $\bar{X}_2 = 235$

**Nivel Confianza:**

- $1 - \alpha = 0.99$
- $\alpha = 0.01$

**SOLUCIÓN:**

- $X_i$: Gasto medio mensual en arbitrios en las ciudades.

$$ IC_{(\mu_1-\mu_2)} = \left[\bar{X}_1-\bar{X}_2 \pm Z_{1-\alpha/2} \cdot \sqrt{\frac{\sigma_1^2}{n_1}+\frac{\sigma_2^2}{n_2}} \right] $$

- Donde Z:

$$ NC=1-\alpha=0.99 $$

$$ \alpha=0.01 $$

$$ Z_{1-\alpha/2}=Z_{0.995}=2.5758 $$

$$ IC_{(\mu_1-\mu_2)} = \left[250-235 \pm Z_{0.995} \cdot \sqrt{\frac{15^2}{200}+\frac{10^2}{180}} \right] $$

$$ 11.66 \le \mu_1-\mu_2 \le 18.34 $$

**Respuesta:**

Con un nivel de confianza del 99%, la diferencia del gasto medio mensual en arbitrios en las ciudades A y B está comprendido desde 11.66 soles hasta 18.34 soles.

- ¿Es diferente el gasto medio mensual en arbitrios en las ciudades A y B?

Responder a la pregunta ¿Es diferente el gasto medio mensual en arbitrios en las ciudades $A$ y $B$? implica responder si ¿ $A \neq B$? o también ¿$A - B \neq 0$? Si apreciamos el intervalo de confianza construido no puede ser cero.

$$ 11.66 \le \mu_1—\mu_2 \le 18.34 $$

- Si:

$$ IC = (+,+), P(+<\mu_1—\mu_1<+) = 1-\alpha \rightarrow \mu_A > \mu_B $$

**Respuesta:**

$\mu_1—\mu_2$ no puede ser cero, es decir, el gasto medio mensual en arbitrios en ambas ciudades es diferentes.

**PROBLEMA 2:**

Se llevan a cabo pruebas de resistencia a la tensión sobre diferentes clases de largueros de aluminio utilizados en la fabricación de alas de aeroplanos comerciales. De la experiencia pasada con el proceso de fabricación de largueros y del procedimiento de prueba los datos obtenidos aparecen en la tabla siguiente. Si $\mu_1$ y $\mu_2$ denotan los promedios verdaderos de las resistencias a la tensión para las clases de largueros, entonces se pide encontrarse un intervalo de confianza del 95% para la diferencia de las medias pl — 1-12

Resultados de la prueba de resistencia a la tensión para largueros de alumio.

| Clase del larguero | Tamaño de la muestra | Media muestral de la resistencia de tensión (kg/mm²) | Desviación estándar muestral de la resistencia a la tensión (kg/mm²) |
| ------------------ | -------------------- | ---------------------------------------------------- | -------------------------------------------------------------------- |
| 1                  | $n_1=10$             | $\bar{X}_1=87.6$                                     | $\sigma_1=1.0$                                                       |
| 2                  | $n_2=12$             | $\bar{X}_2=74.5$                                     | $\sigma_2=1.5$                                                       |

**Datos del problema:**

**Población:**

- 1. $\sigma_1$ = 1.0
- 2. $\sigma_2$ = 1.5

**Muestra:**

- 1. $n_1 = 10$, $\bar{X}_1 = 87.6$

- 2. $n_2 = 12$, $\bar{X}_2 = 74.5$

**Nivel Confianza:**

- $1 - \alpha = 0.95$
- $\alpha = 0.05$

**SOLUCIÓN a:**

- $X_i$: Resistencia a la tensión para largueros de alumio...

$$ IC_{(\mu_1-\mu_2)} = \left[\bar{X}_1-\bar{X}_2 \pm Z_{1-\alpha/2} \cdot \sqrt{\frac{\sigma_1^2}{n_1}+\frac{\sigma_2^2}{n_2}} \right] $$

- Donde Z: Reemplazando

$$ Z_{1-\alpha/2}=Z_{0.975}=1.96 $$

- Reemplazando

$$ IC_{(\mu_1-\mu_2)} = \left[87.6-74.5 \pm 1.96 \cdot \sqrt{\frac{1^2}{10}+\frac{1.5^2}{12}} \right] $$

$$ 12.05 \le \mu_1-\mu_2 \le 14.15 $$

**Respuesta:**

Con el 95% de confianza, la diferencia de las medias de resistencia a la tensión para las clases de largueros (1 y 2) está comprendido desde 12.05 kg/mm² hasta 14.15 kg/mm².

## EJERCICIO 4: Intervalo de confianza para la DIFERENCIA DE MEDIAS MUESTRALES con VARIANZAS POBLACIONALES DESCONOCIDAS PERO IGUALES

**PROBLEMA 1:**

En un proceso químico, se comparan dos catalizadores para verificar su efecto en el resultado de la reacción del proceso. Se preparó una muestra de 12 procesos utilizando el **catalizador 1** y una de 10 con el **catalizador 2**, en el primer caso se obtuvo un rendimiento promedio de 85 con una desviación estándar muestral de 4, mientras que el promedio para la segunda muestra fue 81 y la desviación estándar muestral de 5. Encuentre un intervalo de confianza del 90% para la diferencia entre las medias poblacionales, suponiendo que las poblacionesestán distribuidas aproximadamente en forma normal,con varianzas iguales.

**Datos del problema:**

**Población:**

- Catalizador 1: $\sigma_1$ = ? (DESCONOCIDO)

- Catalizador 2: $\sigma_2$ = ? (DESCONOCIDO)

**Muestra:**

- Catalizador 1: $n_1 = 12$, $\bar{X}_1 = 85$, $S_1 = 4$

- Catalizador 2: $n_2 = 10$, $\bar{X}_2 = 81$, $S_2 = 5$

**Nivel Confianza:**

- $1 - \alpha = 0.90$

- $\alpha = 0.10$

**SOLUCIÓN:**

- Sabemos que $\sigma_1^2 = \sigma_2^2$

- Teniendo la fórmula: Para el intervalo de confianza para esta situación

$$ IC: \left((\bar{X}_1-\bar{X}_2)-T_{1-\alpha/2, gl}\sqrt{S_p^2 \cdot \frac{1}{n_1}+\frac{1}{n_2}} \le \mu_1-\mu_2 \le (\bar{X}_1-\bar{X}_2)+T_{1-\alpha/2, gl}\sqrt{S_p^2 \cdot\frac{1}{n_1}+\frac{1}{n_2}}\right) $$

- Hallamos primero el valor de T-Student

$$ T_{1-\alpha/2, gl}$$

- Donde el grado de libertad es: $gl = n_1 + n_2 - 2$

$$ T_{1-\alpha/2, n_1+n_2-2} $$

$$ T_{1-0.10/2, 12+10-2} $$

$$ T_{1-0.05, 20} $$

$$ T_{0.95, 20} $$

- Usando tabla T

$$ T_{1-\alpha/2, gl} = 1.7291 $$

- Una vez tenemos el valor de T-Student, sigue hallar el valor de $S_p^2$ con la siguiente fórmula:

$$ S_p^2 = \frac{(n_1-1) \cdot S_1^2 + (n_2-1) \cdot S_2^2}{n_1+n_2-2} $$

- Reemplazamos:

$$ S_p^2 = \frac{(12-1) \cdot 4^2 + (10-1) \cdot 5^2}{12+10-2} $$

$$ S_p^2 = \frac{11 \cdot 16 + 9 \cdot 25}{20} $$

$$ S_p^2 = \frac{176 + 225}{20} $$

$$ S_p^2 = \frac{401}{20} $$

$$ S_p^2 = 20.05 $$

- Reemplazando en la fórmula de IC:

$$ IC: \left((85-81)-1.725\sqrt{20.05 \cdot \frac{1}{12}+\frac{1}{10}} \le \mu_1-\mu_2 \le (85-81)+1.725\sqrt{20.05 \cdot\frac{1}{12}+\frac{1}{10}}\right) $$

$$ IC: \left(4-1.725\sqrt{1.67} \le \mu_1-\mu_2 \le 4+1.725\sqrt{1.67}\right) $$

$$ IC: \left(0.69 \le \mu_1-\mu_2 \le 7.31\right) $$

**Respuesta:**

Con un nivel de confianza del 90%, la diferencia entre las medias poblacionales de los catalizadores 1 y 2 está comprendido desde 0.69 hasta 7.31.

$$ IC=(+, +), P(+<μ1−μ2<+) = 1−α→μ1>μ2 $$

**Nota:** tienen un redimiento diferente.

## EJERCICIO 5: Intervalo de confianza para la DIFERENCIA DE MEDIAS MUESTRALES con VARIANZAS POBLACIONALES DESCONOCIDAS PERO DIFERENTES

Se registraron los siguientes datos en días, que representan los tiempos de recuperació de pacientes tratados aleatoriamente con dos medicamentos para aliviarlos de grave infecciones en la vesícula:

**Medicamento 1:**

- $n_1 = 14$
- $\bar{X}_1 = 17$
- $S_1^2 = 1.5$

**Medicamento 2:**

- $n_2 = 14$
- $\bar{X}_2 = 19$
- $S_2^2 = 1.8$

Encuentre un intervalo de confianza del 99% para la diferencia $\mu_1-\mu_2$ en el tiempo promedio de recuperación para los medicamentos, suponiendo poblaciones normales con *varianzas diferentes*.

**Datos del problema:**

**Población:**

- Medicamento 1: $\sigma_1$ = ? (DESCONOCIDO)
- Medicamento 2: $\sigma_2$ = ? (DESCONOCIDO)

**Muestra:**

- Medicamento 1: $n_1 = 14$, $\bar{X}_1 = 17$, $S_1^2 = 1.5$
- Medicamento 2: $n_2 = 14$, $\bar{X}_2 = 19$, $S_2^2 = 1.8$

**Confianza:**

- $1 - \alpha = 0.99$
- $\alpha = 0.01$

**SOLUCIÓN:**

- $\sigma_1^2 \neq \sigma_2^2$
- Teniendo la fórmula del IC para varianzas diferentes y desconocidas:

$$ IC: \left((\bar{X}_1-\bar{X}_2)-T_{1-\alpha/2, v}\sqrt{\frac{S_1^2}{n_1}+\frac{S_2^2}{n_2}} \le \mu_1-\mu_2 \le (\bar{X}_1-\bar{X}_2)+T_{1-\alpha/2, v}\sqrt{\frac{S_1^2}{n_1}+\frac{S_2^2}{n_2}}\right) $$

- Hallamos primero el valor de T-Student

$$ T_{1-\alpha/2, v}$$

- Donde el grado de libertad es:

$$ v= \frac{\left(\frac{S_1^2}{n_1}+\frac{S_2^2}{n_2}\right)^2}{\frac{1}{n_1-1}\left(\frac{S_1^2}{n_1}\right)^2+\frac{1}{n_2-1}\left(\frac{S_2^2}{n_2}\right)^2} $$

- Reemplazando:

$$ v= \frac{\left(\frac{1.5}{14}+\frac{1.8}{14}\right)^2}{\frac{1}{14-1}\left(\frac{1.5}{14}\right)^2+\frac{1}{14-1}\left(\frac{1.8}{14}\right)^2} $$

$$ v=25.787 \cong 26 $$

- Tabla T

$$ T_{1-\alpha/2, v} = T_{0.995, 26} = 2.779 $$

- Ahora reemplazando en la fórmula de IC:

$$ IC: \left((17-19)-2.779\sqrt{\frac{1.5}{14}+\frac{1.8}{14}} \le \mu_1-\mu_2 \le (17-19)+2.779\sqrt{\frac{1.5}{14}+\frac{1.8}{14}}\right) $$

$$ 2-1.349 \le \mu_1-\mu_2 \le 2+1.015 $$

$$ 0.651 \le \mu_1-\mu_2 \le 3.349 $$

**Respuesta:**

Con nivel de confianza del 99% la verdadera diferencia del tiempo medio de recuperación para los medicamentos esta comprendido de 0.651 a 3.349

## EJERCICIO 6: Intervalo de confianza para la PROPORCIÓN

**PROBLEMA 1:**

Los compradores de última hora se quejan de que las tiendas por departamento de LIMA cierran muy temprano. En una muestra aleatoria de 600 compradores compulsivos de un centro comercial se encontró que 360 están a favor de un horario más amplio para las compras.

Calcule e interprete un intervalo del 95% de confianza para la proporción verdadera de compradores que están a favor de un horario más amplio para las compras.

**Datos del problema:**

**Población:**

- ¿?

**Muestra:**

- $n = 600$
- $X = 360$
- Proporción muestral: $\hat{p} = \frac{X}{n} = \frac{360}{600} = 0.6$
- $q=0,4$

**Nivel de Confianza:**

- $1 - \alpha = 0.95$
- $\alpha = 0.05$

Tabla: $Z_{1-0.05/2}=Z_{0.975}=1.96$

**SOLUCIÓN:**

- $X$: Compradores que están a favor de un horario más amplio para las compras.
- Teniendo la siguiente fórmula:

$$ p-Z_{1-\alpha/2}\sqrt{\frac{pq}{n}} \le \pi \le p+Z_{1-\alpha/2}\sqrt{\frac{pq}{n}} $$

- Reemplazando:

$$ 0.6-1.96\sqrt{\frac{0.6 \cdot 0.4}{600}} \le \pi \le 0.6+1.96\sqrt{\frac{0.6 \cdot 0.4}{600}} $$

$$ IC(\pi)=0,6 \plusmn 1,96 \cdot \sqrt{\frac{0.6 \cdot 0.4}{600}} $$

$$ 0,561 \le \pi \le 0,639 $$

**Respuesta:**

Con un 95% de confianza la verdadera proporción (porcentaje) de compradores que están a favor de un horario más amplio para las compras en el centro comercial, se encuentra entre 0.561 y 0.639 (56.1% y 63.9%).

## EJERCICIO 7: Intervalo de confianza para la DIFFERENCIA DE PROPORCIONES

Los compradores de ultima hora de los centros comerciales se quejan de que las tiendas por departamento de LIMA cierran muy temprano. En una muestra aleatoria de 600 compradores compulsivos del Centro Comercial La Rambla y del Centro Comercial Jockey Plaza se encontró que 360 están a favor de un horario más amplio para las compras y del Centro Comercial Jockey Plaza encontró que 240 están a favor de un horario mas amplio de compra.

Calcule e interprete un intervalo del 95% de confianzal para la diferencia de proporciones verdadera de compradores de los 2 centros comerciales que están a favor de un horario más amplio para las compras.

**Datos del problema:**

**Población:**

- ¿?

**Muestra:**

- $n_1 = 600$
- $X_1 = 360$
- $P_1 = \frac{X_1}{n_1} = \frac{360}{600} = 0.6$
- $P_2 = \frac{X_2}{n_2} = \frac{240}{600} = 0.4$

**Nivel de Confianza:**

- $1 - \alpha = 0.95$
- $\alpha = 0.05$
- Tabla: $Z_{1-0.05/2}=Z_{0.975}=1.96$

**SOLUCIÓN:**

- $X1$: Clientes a favor de amplio horario de CC La Rambla
- $X2$: Clientes a favor de amplio horario de CC Jockey Plaza

- Teniendo la siguiente fórmula:

$$ IC(p_1-p_2)=\left(p_1-p_2-Z_{1-\alpha/2}\sqrt{\frac{p_1q_1}{n_1}+\frac{p_2q_2}{n_2}} \le \pi \le p_1-p_2+Z_{1-\alpha/2}\sqrt{\frac{p_1q_1}{n_1}+\frac{p_2q_2}{n_2}}\right) $$

- Reemaplazamos usando la siguiente reducción:

$$ IC(\pi) = 0,6-0,4 \pm 1,96 \cdot \sqrt{\frac{0,6 \cdot 0,4}{600}+\frac{0,4 \cdot 0,6}{600}} $$

$$ IC(\pi) = (0,14; 0,25) $$

$$ 0,14  \le \pi \le 0,25 $$

**Respuesta:**

Con un 95% de confianza la verdadera proporción (porcentaje) de compradores que están a favor de un horario más amplio para las compras en el centro comercial, se encuentra entre 0.14 y 0.25 (14.4% y 25.5%).

## EJERCICIO 8: Intervalo de confianza Chi-Cuadrado

**PROBLEMA 1:**

Los siguientes datos representan las edades que tenían al momento de morir por enfermedad de una muestra de 20 personas de un pueblo:

`80, 87, 90, 61, 85, 73, 82, 84, 75, 85, 58, 70, 70, 78, 84, 95, 87, 77, 81, 52`

Hallar un intervalo de confianza del 95% para la varianza poblacional de la edad de merte.

**Datos del problema:**

**Población:**

- ¿?

**Muestra:**

- $n = 20$
- $S = 11.0506$

**Nivel de Confianza:**

- $1 - \alpha = 0.95$
- $\alpha = 0.05$

**SOLUCIÓN:**

- Teniendo la siguiente fórmula

$$ \frac{(n-1)S^2}{\chi_{1-\alpha/2, n-1}^2} \le \sigma^2 \le \frac{(n-1)S^2}{\chi_{\alpha/2, n-1}^2} $$

- Usando la tabla Chi-Cuadrado

$$ \chi_{1-\alpha/2, n-1}^2 = \chi_{0.975, 19}^2 = 32.8523 $$

$$ \chi_{\alpha/2, n-1}^2 = \chi_{0.025, 19}^2 = 8.9065 $$

- Reemplazando

$$ \frac{(20-1)11.0506^2}{32.8523} \le \sigma^2 \le \frac{(20-1)11.0506^2}{8.9065} $$

$$ 71.258 \le \sigma^2 \le 262.8406 $$

**Respuesta:**

Hay un 95% de confianza de que la varianza de las edades de todas las personas que mueren por enfermedad en el pueblo cae entre 71,258 y 262,8406
