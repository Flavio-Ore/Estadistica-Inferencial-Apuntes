# Distribución Muestral

**Distribución**: Conjunto de datos la manera en la que están presentados varían según la distribución.

**Distribución muestral**: Datos de varias muestras de una población, mientras MÁS MUESTRAS, MÁS SEGURO QUE SERÁ DISTRIBUCIÓN NORMAL, confirmando la campana de Gauss.

SI ESTUDIO LA MEDIA (&mu;) DE LA POBLACIÓN: <a href="./lista-definiciones.md">Parámetro</a>[PARÁMETRO](#14-parámetro)

SI ESTUDIO LA MEDIA ($\tilde{x}$)DE LA MUESTRA: [ESTADÍSTICO o ESTIMADOR](#15-estadístico)

- Teoria del muestreo estudia las **RELACIONES** entre la **POBLACIÓN** y las **MUESTRAS** extraídas de la misma
- Permite **ESTIMAR** cantidades **DESCONOCIDAS** de la población como la media poblacional, la varianza,etc. frecuentemente llamadas **PARÁMETROS POBLACIONALES** a partir de las correspondientes cantidades muestrales como son la media, la varianza y otros **estadísticos muestrales** o brevemente llamados **estadísticos**.
- La teoría de muestreo es útil para determinar por ejemplo: el aplicar un nuevo suero para el tratamiento de una enfermedad, o decidir si un proceso de producción es mejor que otro. Estas deciciones envuelven a los llamados **ensayos e hipótesis de significación**.
- En general, a todo lo mencionado anteriormente se le conoce como **INFERENCIA ESTADÍSTICA**.
- De la población se extraen muestras de tamaño n, se calcula el estadístico de interés y se construye una distribución muestral de ese estadístico.
-La muestra puede tomar diferentes valores, pero el estadístico de interés es el mismo. Entonces es mejor hacer que varíen lo menos posible el tamaño de muestra.

```mermaid
flowchart RL

subgraph Población["Población (N) y &mu;"]
    población["
        🙍‍♂️🙍‍♂️...🙍‍♂️
    "]
end

subgraph muestran["Muestra n"]
    n_k("🙍‍♂️..🙍‍♂️")
end

subgraph distribucion["Distriución Muestral"]
    promediok["Promedio Muestral n"]
    DI["
        Son los promedios, proporciones, varianzas, etc. 
        de todas las muestras posibles de tamaño n 
        que se pueden obtener de una población
    "]
end 

n_k --> promediok -- "ESTIMA" --> Población --> n_k
```

*Véase también [Relación población-muestra](/lista-definiciones.md/#relación-población-muestra)*.

**e.g.** Tenemos a la población de 2500 empleados y varias de muestras cada una de 30.

- Población $N$

$N = 2500$

| Empleado | Salario |
| -------- | ------- |
| 1        | $       |
| 2        | $       |
| 3        | $       |
| ...      | ...     |
| 2500     | $       |

$\mu = \$1200$

- Muestra: $n_{1}$

$n_{1} = 30$

| Empleado | Salario |
| -------- | ------- |
| 1        | $       |
| 2        | $       |
| 3        | $       |
| ...      | ...     |
| 30       | $       |

$\tilde{x}_{1} = \$13334$

- Muestra: $n_{2}$

$n_{2} = 30$

| Empleado | Salario |
| -------- | ------- |
| 1        | $       |
| 2        | $       |
| 3        | $       |
| ...      | ...     |
| 30       | $       |

$\tilde{x}_{2} = \$11484$

- Muestra: $n_{3}$

$n_{k} = 30$

| Empleado | Salario |
| -------- | ------- |
| 1        | $       |
| 2        | $       |
| 3        | $       |
| ...      | ...     |
| 30       | $       |

$\tilde{x}_{k} = \$12500$

- Donde $k=500$
- Tabla de valores de 500 muestras, de tamaño $n=500$

| No. de muestras | Media muestral ($\tilde{x}$)  |
| --------------- | ----------------------------- |
| 1               | $\tilde{x}_{1}$ = $\$13354$   |
| 2               | $\tilde{x}_{2}$ = $\$11484$   |
| 3               | $\tilde{x}_{3}$ = $\$11138$   |
| ...             | ...                           |
| 500             | $\tilde{x}_{500}$ = $\$12500$ |

$$ \frac{\sum\tilde{x}_{i}}{500} \approx \mu  $$

Si en vez de 500 muestras tomamos todas las muestras posibles.

**Obtendríamos:** Valor estimado = media poblacional

$$ E(\tilde{x}) = \mu  $$

## Propiedades de la distribución muestral de la media muestral x̄

**Donde la media y la desviación estándar:**

🎪 La media (&mu;) y la [desviación típica](./lista-definiciones.md/#desviación-estándar) (&sigma;) de la **población**.

🏠 La media (&mu;$_{\tilde{x}}$) y la [desviación típica](./lista-definiciones.md/#desviación-estándar) (&sigma;$_{\tilde{x}}$) de la distribución **muestral**.

Casos según la distribución de la población: Donde $X$ son los datos.

### Distribución Estándar de la Muestra (n) y Población (N)

La población se aproxima a una distribución normal, la media muestral se distribuye normalmente para cualquier tamaño de muestra.

Muestra: $X \sim  n(\mu, \frac{\sigma}{\sqrt{n}})$

Población: $X \sim N(\mu, \sigma²)$

#### Caso 1: Población con Distribución **[NORMAL](./lista-definiciones.md/#curva-normal)**

$X \sim N(\mu, \sigma^2)$

Si la muestra aleatoria $X_{1}, ..., X_{n}$ Tiene distribución normal con **media &mu;** y **desviación típica &sigma;**:

Para cualquier tamaño de muestra ($n$):

La media muestral ($\tilde{x}$) también tiene una distribución normal con media $\mu_{\tilde{x}} = \mu$ y [desviación típica](./lista-definiciones.md/#desviación-estándar): $\sigma_{\tilde{x}} = \frac{\sigma}{\sqrt{n}}$

**Notación estadística** &rightarrow; Si: $X \sim n(\mu, \frac{\sigma}{\sqrt{n}}) \rightarrow X \sim N(\mu, \frac{\sigma}{\sqrt{n}})$

#### Caso 2: Población con distribución **NO NORMAL**

$X \sim ??(\mu, \sigma^2)$

**Teorema del [límite central](/lista-definiciones.md/#teorema-de-límite-central)**

Si la muestra seleccionada tiene un tamaño **MAYOR O IGUAL** a **30**, sea cual sea la forma de la distribución de la población **(SEA NORMAL O NO)**, las medias de todas las muestras seleccionadas de la población tendrán una distribución normal.

## Recapitulando 🔃

### a) Valor esperado

Para el muestreo aleatorio simple. Donde $E$ es el **valor esperado** $E(\tilde{x}) = \mu$

**e.g.** Sabemos que &mu; = \$12,2111, entonces E($\tilde{x}$) = \$12,2111

### b) Desviación Estándar

#### Población finita

$$ \sigma_{\tilde{x}} = \sqrt{\frac{N - n}{N - 1}} \cdot (\frac{\sigma^2}{n}) $$

#### Población infinita

Si no ❌ dan datos de la población, entonces se asume que es infinita. ✔

$$ \sigma_{\tilde{x}} = \frac{\sigma}{\sqrt{n}} $$

#### Curiosidad 👀❓

Si la población es finita pero la división entre la muestra y la población es menor o igual a 0,05; se usa la fómula de la [Población infinita](#población-infinita)

$$ \frac{n}{N} \le 0,05 $$

**e.g.** Sabemos que $\sigma = \$1,500$, entonces $\sigma_{\tilde{x}} = \$1,500$

$\sigma = 4480.42$
$N = 2500$
$n = 30$

$$ \frac{n}{N} = 30/2500 = 0,012 $$

$$ \sigma_{\tilde{x}} = \frac{4480.42}{\sqrt{30}} = 818.01 $$

**e.g.** Sabemos que $\sigma = \$1,500$, entonces $\sigma_{\tilde{x}} = \$1,500$

$\sigma = 4480.42$
$N = 2500$
$n = 30$

$$ \frac{n}{N} = 30/2500 = 0,012 $$

$$ \sigma_{\tilde{x}} = \frac{4480.42}{\sqrt{30}} = 818.01 $$

### c) Forma de la distribución (población &equiv; p)

#### Para una población desconocida

La distribución de la media de la muestra $\tilde{x}$ se puede aproximar con una distribución normal de probabilidades cuando el tamaño de la muestra es grande. Mayor o igual a 30.

$$ n \ge 30 $$

#### Para una [Población normal](./lista-definiciones.md/#población-normal), sin importar el tamaño de la muestra

La distribución muestral de $\tilde{x}$ es **[NORMAL](/lista-definiciones.md/#curva-normal)** para cualquier tamaño de la muestra.

![Tabla Normal](./Distribucion-muestral/tabla-normal.png)

### En resumen 🥣

Si $n \ge 30$, entonces $\tilde{x}$ se distribuye normalmente.

Si $n < 30$, entonces $\tilde{x}$ se distribuye normalmente *si la población es normal*

Si $n$ con una [M.A.S](/lista-definiciones.md/#311-muestreo-aleatorio-simple) de muestra mayor o igual a 30 y aplicando el [Teorema del Límite Central](/lista-definiciones.md/#teorema-de-límite-central), la distribución muestral de $\tilde{x}$ es normal con &mu; y &sigma;$_{\tilde{x}} = \frac{\sigma}{\sqrt{n}}$

Véase el ejemplo en [Teorema del Límite Central](/lista-definiciones.md/#teorema-de-límite-central)

![distribucion-muestral-de-x](/Lista-definiciones/distribucion-muestral.png)

Supóngase que son extraídas de una [Población Infinita](#población-infinita) todas las posibles [muestras](/lista-definiciones.md/#13-muestra) **sin reemplazo** de tamaño $n$.

**Si se denota:**

Vésase [distribución estándar](/distribucion-muestral.md/#distribución-estándar-de-la-muestra-n-y-población-n) de la [muestra](#la-media-μ-y-la-desviación-típica-σ-de-la-distribución-muestral) y [población](#la-media-μ-y-la-desviación-típica-σ-de-la-población)

- La [distribución muestral](#6-distribución-muestral) de las medias cumplen la siguiente igualdad:

- La media de la muestra va a ser igual a la media de la población cuando más muestras se tenga:

$$ \mu_{\tilde{x}} = \mu $$

- La desviación estándar de la muestra
- n = cantidad de elementos de la muestra

$$ \sigma_{\tilde{x}} = \frac{\sigma}{\sqrt{n}} $$

> [MARKDOWN BASIC SYNTAX GUIDE](https://www.markdownguide.org/basic-syntax/)
> [Mathematics in R Markdown](https://rpruim.github.io/s341/S19/from-class/MathinRmd.html)
> [How to markdown and document](https://hydro-informatics.com/documentation/documentation.html#markdown-editors-ides)
> [Extra Mathematics in Markdown](https://learninglab.gitlabpages.inria.fr/mooc-rr/mooc-rr-ressources/module1/ressources/introduction_to_markdown.html)
