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

**Confianza:**

- $1 - \alpha = 0.95$
- $\alpha = 0.05$

**SOLUCIÓN:**

- $X$: variable aleatoria tiempo de vida de focos fabricados
- $X$: $N(\mu; \sigma^2)$

**Intervalo de Confianza:**

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

Con un nivel de confianza del 95%, el tiempo de vida promedio de los focos está comprendido desde 765.69 horas hasta 794.31 horas.

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

**Confianza:**

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

**Confianza:**

- $1 - \alpha = 0.95$
- $\alpha = 0.05$

**SOLUCIÓN:**

- $X$: V.A duración de la bateria

**Intervalo de Confianza:**

$$ IC=\left(\bar{X}-T_{1-\alpha/2, gl}\frac{S}{\sqrt{n}} \le \mu \le \bar{X}+T_{1-\alpha/2, gl}\frac{S}{\sqrt{n}}\right)$$

**$$ IC=\left(\bar{X}-T_{1-\alpha/2, gl}\frac{S}{\sqrt{n}} \le \mu \le \bar{X}+T_{1-\alpha/2, gl}\frac{S}{\sqrt{n}}\right)$$

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
