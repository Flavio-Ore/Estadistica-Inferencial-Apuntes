# Estadística Inferencial 🧠

Inferir parámetros estadísticos de la población, a partir de los estadísticos de una muestra

## 0. Lista de definiciones

### Probabilidad de complemento

$$ P(A^c) = 1 - P(A) $$

Esta probabilidad se usa cuando se quiere calcular la probabilidad de que un evento no ocurra. Se calcula restando la probabilidad de que ocurra el evento a 1.

### Teorema del Límite Central

El teorema del límite central establece que, si se toman todas las muestras posibles de un tamaño $n$ de una población, la distribución de las medias muestrales será una distribución normal con una media igual a la media poblacional y una desviación estándar igual a la desviación estándar poblacional dividida por la raíz cuadrada del tamaño de la muestra.

## 1. Conceptos Básicos

### 1.1. Definición

Clasificación de la estadística teoría para **inferir o estimar** las leyes de una población, partiendo de un **análisis**.

### 1.2. Población

Conjunto de entes.

Unidades de observación, cuyas características observables se van a estudiar.

Se define en términos de su contenido, extensión y tiempo. Las medidas estadísticas que se obtienen se denominan **parámetros**.

### 1.3. Muestra

Es un subconjunto de la población seleccionada con el fin de obtener información acerca de la población de la que proviene.

La muestra debe ser **representativa** y **aleatoria**. Sus medidas estadísticas se denominan **estadísticos** o **estadígrafos**

### 1.4. Parámetro

Característica numérica que describe una variable observada en la **población**.

### 1.5. Estadístico

Característica numérica que describe una variable observada en la **muestra**.

### 1.6. Variable

Es una característica, cualidad de un objeto de estudio y tiende a medido.

### 1.7. Observación (datos)

Valores que toma la característica ([variable](#16-variable)) observada en cada elemento.

### 1.8. Unidad de análisis

Objeto indivisible que será estudiado sobre una población.

![Población->Muestra->Individuos->Variables](https://asesoriauniversitaria.com/wp-content/uploads/2022/03/img_1.png)

## Relación Población-Muestra

```mermaid
flowchart LR
    subgraph Población
    población("
        &mu;
        &sigma;²
        &pi;
        Parámetros
    ")
    end

    subgraph Muestra
    muestra("
        $\tilde{x}$
        S²
        &rho;
        Estadísticos
    ")
    end

    Población  -->  Estiman  -->  Muestra  -->  Población

```

### Para la población

- &mu; = Media o promedio poblacional
- &sigma;² = Varianza poblacional
- &sigma; = Desviación estándar poblacional
- &pi; = [Parámetro](#14-parámetro)

### Para la muestra

- $\tilde{x}$ = Media o promedio muestral
- S² = Varianza muestral
- S = Desviación estándar muestral
- &rho; = [Estadísticos](#15-estadístico)

### Nota: Si S² = 0, entonces todos los datos son iguales al promedio

## 2. Muestreo

Herramienta de la investigación científica, cuya función básica es **determinar qué parte de una población debe examinarse**, con la finalidad de hacer inferencias.

### 2.1 Muestreo Probabilístico (Aleatorio)

- Todos los elementos tienen la misma posibilidad de ser elegidos (probabilidad conocida y equitativa)
- Nos aseguran la representatividad de la muestra
- Se puede sacar conclusiones sobre la población (inferencia estadística)ro
- Alto costo de tiempo y dinero (criterios estadísticos)

### 2.2. Muestreo no Probabilístico (No Aleatorio)

- No todos los elementos tienen la misma posibilidad de ser elegidos
- Son muestras que seguramente **esconden sesgos** que sea lo más representativa posible
- No se puede sacar conclusiones (extrapolar) sobre la población (inferencia estadística)
- Bajo costo de tiempo y dinero (criterios no estadísticos)

## 3. Tipo de muestreo

### 3.1. Probabilístico

- Aleatorio simple
- Aleatorio sistemático
- Aleatorio estratificado
- Aleatorio por conglomerados

#### 3.1.1. Muestreo Aleatorio Simple

Todos los elementos de la población tienen la misma probabilidad de ser elegidos, es conocida y equitativa.

- Dificultad al elegir todos los números aleatorios si la población es muy grande, alto costo
- Necesita una lista completa de los elementos de la población (marco muestral)
- Es obligatorio un marco muestral

#### 3.1.2 Muestreo Sistemático

Se aplica cuando la población es bastante irregular respecto al carácter que se estudia y se desea que en la muestra se refleje toda est variabilidad.

- Fácil de seleccionar en campo o durante un operativo
- En el [MAS](#312-muestreo-sistemático) primero se calcula primero el tamaño de la muestra y luego se selecciona el intervalo de selección
- A veces se usa un intervalo

#### 3.1.3. Muestreo Estratificado

- Se estratifica la población según ciertas variables de interés
- Cada estrato homogéneos en su interior y diferentes entre sí en propiedades y tamaño
- Los estratos más grandes tienen mayor probabilidad de ser elegidos

#### 3.1.4. Muestreo por Conglomerados

Técnica que aprovecha la existencia de grupos o conglomerados naturales en la población. Este muestreo se utiliza cuando se trata de obtener una muestra al azar de una población que está dispersa geográficamente.

- Los conglomerados son homogéneos en su interior y diferentes entre sí en propiedades y tamaño
- Se seleccionan los conglomerados y luego se seleccionan los elementos de cada conglomerado
- Se usa cuando la población es muy grande y dispersa

### 3.2. No Probabilístico

- Por conveniencia o intencional
- Por cuota
- Bola de nieve
- Discrecional

#### 3.2.1 Muestreo por conveniencia

Comúnmente usada. Consiste en seleccionar una muestra de la población por el hecho de que sea accesible, implica un bajo coste operativo y bajo costo en el muestreo

**e.g.** Seleccionar a los primeros 100 estudiantes que lleguen a la universidad

#### 3.2.2 Muestreo por cuota

Es la versión **no probabilística** del muestreo estratificado.

##### Consiste en tres fases

1. Encontrar los grupos: Dividir la población en grupos o estratos según [variable](#16-variable) de interés
2. Fijar tamaño de las cuotas: Se fijan una "cuotas" que consisten en un número de individuos a encuestas para cada uno de estos grupos.
3. Seleccionar los individuos y comprobar las cuotas: Se buscan a los individuos (cuotas) de manera **no aleatoria**, puede ser por un muestreo por conveniencia.

#### 3.2.3 Muestreo por bola de nieve

Se localiza a algunos individuos, los cuales conducen a otros y estos a otros y así sucesivamente. Hasta conseguir que se **sature** la información.

##### Se emplea para poblaciones ocultas o de difícil acceso

#### 3.2.4 Muestreo discrecional

A criterio del investigador los elementos son elegidos sobre lo que él cree que puede aportar al estudio o investigación

## 4. Tablas estadísticas

### 4.1. Tabla Distribución Normal (Z positivo y negativo)

![Tabla Distribución Normal](https://i.ytimg.com/vi/C5btKRpblRQ/maxresdefault.jpg)

```mermaid
flowchart LR
    subgraph Normal
        var("
            &mu; = 0;
            &sigma; = 1;
            S = 1;
        ")
    end

Normal ==> Estándar
```

#### Problema a)

$P(Z \le -2,53)$

- Buscar en la tabla el valor de -2,5 en la columna de la izquierda y 0,03 en la fila superior
- El valor de la tabla es 0,0057

$$ P(Z \le -2,53) = 0,0057 $$

#### Problema b)

$P(Z \ge 1,32)$

- No puede ser mayor
- Usamos **probabilidad de complemento**

$$ 1 - P(Z \le 1,32) $$

- Buscar en la tabla el valor de 1,3 en la columna de la izquierda y 0,02 en la fila superior
- El valor de la tabla es 0,4032
- Luego se resta a 1
- El resultado es 0,5968

$$ P(Z \ge 1,32) = 0,5968 $$

#### Problema c)

$P(-2,53 \le 3,01)$

- Se dividen las probabilidades en dos

$$ P(Z \le 3,01) - P(Z \le -2,53) $$

- **La probabilidad mayor a Z pasó a restar**
- Buscar en la tabla el valor de 3,0 en la columna de la izquierda y 0,01 en la fila superior
- El valor de la tabla es 0,4987
- Buscar en la tabla el valor de -2,5 en la columna de la izquierda y 0,03 en la fila superior
- El valor de la tabla es 0,0057

$$ P(Z \le 3,01) - P(Z \le -2,53) $$
$$ 0,4987 - 0,0057 $$
$$ 0,4930 $$

#### Ejercicio $P(X < 6)$

##### Calcule la probabilidad de que X sea menor que 6

$$ \mu = 8 $$
$$ \sigma = 1,5 $$

### Fórmula de Proceso de Estandarización 🔋

$$ Z = \frac{X - \mu}{\sigma} $$

### Los valores de Z van de -3,99 a 3,99 ❗

- Aplican las mismas reglas de la tabla de distribución normal

$$ Z = \frac{6 - 8}{1,5} $$
$$ Z = \frac{-2}{1,5} $$
$$ Z = -1,33 $$

- Buscar en la tabla el valor de -1,3 en la columna de la izquierda y 0,03 en la fila superior
- El valor de la tabla es 0,0918
  $$ P(Z < 6) = 0,0918 $$

## 5. Cálculo de tamaño de muestra 🔋

Determinar el tamaño de la muestra que se va a seleccionar es un paso importante en cualquier estudio de investigación de mercados, se debe justificar convenientemente de acuerdo al planteamiento del problema, la población, los objetivos y el propósito del estudio.

**Se definen los siguientes factores:**

### a) Nivel de confianza (1 - &alpha;)

Probabilidad deseada de que el parámetro a estimar se encuentre dentro de un margen esperado , los valores estadísticos son:

#### Se elige nivel de confianza

```mermaid
flowchart LR
    subgraph NC["Nivel de confianza"]
        alpha("
            0,90 = 90%
            0,95 = 95%
            0,98 = 98%
        ")
    end

    subgraph Za["Z&alpha;"]
        z("
            1,64
            1,96
            2,33
        ")
    end

    NC --> Za
```

### b) Margen de error deseado (d)

Error en la estimación que como máximo se espera obtener

### c) Proporción estimada (p)

Proporción estimada del éxito de la variable que se desea medir

### 5.1. Cálculo del tamaño de muestra conociendo la población

$$ n = \frac{N \cdot Z\alpha \cdot p \cdot q}{d^2 \cdot (N - 1) + Z\alpha^2 \cdot p \cdot q}$$

### 5.2. Cálculo del tamaño de muestra sin conocer la población

$$ n = \frac{Z\alpha^2 \cdot p \cdot q}{d^2} $$

### 5.3. Cálculo del tamaño de muestra para una media cuando se conoce la población

$$ n = \frac{Z\alpha^2 \cdot \sigma^2 \cdot N}{E^2(N - 1) + Z\alpha^2 \cdot \sigma^2} $$

### 5.4. Cálculo del tamaño de muestra para una media cuando se desconoce la población

$$ n = \frac{Z\alpha^2 \cdot \sigma^2}{E^2} $$

#### Variables para el cálculo de tamaño de muestra

- N = Tamaño de la población
- Z&alpha; = Nivel de confianza
- p = Probabilidad de éxito
- q = Probabilidad de fracaso
- d = Error máximo permisible en la estimación (Margen de error)

## 6. Distribución Muestral

**Distribución**: Conjunto de datos la manera en la que están presentados varían

```mermaid
flowchart RL

subgraph Población["Población y &mu;"]
    población["
        🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️
    "]
end

subgraph muestran[Promedio muestral n]
    n_n("🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️...")
end

subgraph muestra1[Promedio muestral 1]
    n1("🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️")
end

subgraph muestra2[Promedio muestral 2]
    n2("🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️")
end

subgraph muestra3[Promedio muestral 3]
    n3("🙍‍♂️🙍‍♂️🙍‍♂️🙍‍♂️")
end

subgraph distribucion[Distribución de probabilidad de cualquier prpiedad de estas medias de la muestra]
    promedio1["Promedio Muestral 1"]
    promedio2["Promedio Muestral 2"]
    promedio3["Promedio Muestral 3"]
    promedion["Promedio Muestral n"]
end

Población --> n1
Población --> n2
Población --> n_n
Población --> n3

promedio1 -- estima --> Población
promedio2 -- estima --> Población
promedio3 -- estima --> Población
promedion -- estima --> Población

promedio1 <---  n1
promedio2 <---  n2
promedio3 <---  n3
promedion <---  n_n
```

Véase también [Relación población-muestra](#relación-población-muestra)

**e.g.** Tenemos a la población de 2500 empleados y varias de muestras cada una de 30.

### Población

#### $N = 2500$

| Empleado | Salario |
| -------- | ------- |
| 1        | $       |
| 2        | $       |
| 3        | $       |
| ...      | ...     |
| 2500     | $       |

$\mu = \$1200$

#### $n_{1} = 30$

| Empleado | Salario |
| -------- | ------- |
| 1        | $       |
| 2        | $       |
| 3        | $       |
| ...      | ...     |
| 30       | $       |

$\tilde{x}_{1} = \$13334$

#### $n_{2} = 30$

| Empleado | Salario |
| -------- | ------- |
| 1        | $       |
| 2        | $       |
| 3        | $       |
| ...      | ...     |
| 30       | $       |

$\tilde{x}_{2} = \$11484$

#### $n_{k} = 30$

| Empleado | Salario |
| -------- | ------- |
| 1        | $       |
| 2        | $       |
| 3        | $       |
| ...      | ...     |
| 30       | $       |

$\tilde{x}_{k} = \$12500$

Donde $k = 500$

### Distribución muestral de $\tilde{x}$

### a) Valor esperado

Para el muestreo aleatorio simple. Donde E es el valor esperado E($\tilde{x}$) = &mu;

**e.g.** Sabemos que &mu; = \$12,2111, entonces E($\tilde{x}$) = \$12,2111

### b) Desviación Estándar

#### Población finita

$$ \sigma\_{\tilde{x}} = \sqrt{\frac{N - n}{N - 1}} \cdot \frac{\sigma^2}{n} $$

#### Población infinita

$$ \sigma\_{\tilde{x}} = \frac{\sigma}{\sqrt{n}} $$

### Si la población finita pero $\frac{N - n}{N} \le 0,05$ se usa la fómula de la [Población infinita](#población-infinita)

**e.g.** Sabemos que $\sigma = \$1,500$, entonces $\sigma_{\tilde{x}} = \$1,500$

$\sigma = 4480.42$

$N = 2500$

$n = 30$

$\frac{n}{N} = 30/2500 = 0,012$

$$ \sigma\_{\tilde{x}} = \frac{4480.42}{\sqrt{30}} = 818.01 $$

### c) Forma de la distribución (población &cong; p)

#### Población desconocida

La distribución de la media de la muestra $\tilde{x}$ se puede aproximar con una distribución normal de probabilidades cuando el tamao de la muestra es grande

$$ n \ge 30 $$

#### Población normal

Ls distribución muestral de $\tilde{x}$ es normal para cualquier tamaño de la muestra.

![Tabla Normal](https://bookdown.org/aquintela/EBE/Figure/inter-confi.png)

### Si $n \ge 30$, entonces $\tilde{x}$ se distribuye normalmente

### Si $n < 30$, entonces $\tilde{x}$ se distribuye normalmente _si la población es normal_

### Si es un [M.A.S](#311-muestreo-aleatorio-simple) de $n \ge 30$ y aplicando el [Teorema del Límite Central](#teorema-del-límite-central), la distribución muestral de $\tilde{x}$ es normal con $\mu_{\tilde{x}} = \mu$ y $\sigma_{\tilde{x}} = \frac{\sigma}{\sqrt{n}}$

### La media $(\mu_{\tilde{x}})$ y la desviación estándar $(\sigma_{\tilde{x}})$ de la distribución muestral de $\tilde{x}$ son

$$ \mu*{\tilde{x}} = \mu $$
$$ \sigma*{\tilde{x}} = \frac{\sigma}{\sqrt{n}} $$

## 7. Prueba de normalidad

Para conseguir si la distribución de datos se ajusta a una distribución normal teórica.

### 7.1. Prueba de Kolmogorov-Smirnov

1. $H_{0}$: Los datos siguen una [D.N.E](#6-distribución-muestral)
2. $H_{1}$: Los datos **NO** siguen una [D.N.E](#6-distribución-muestral)

#### Errores conocidos (véase [Nivel de confianza](#se-elige-nivel-de-confianza))

$$ \alpha = \{0,01; 0,05; 0,1\}$$

#### Estadístico de Prueba

## Formulario

| Fórmula                   | Notación                                | Descripción                                               |
| ------------------------- | --------------------------------------- | --------------------------------------------------------- |
| Estandarización           | [Z - &mu; - &sigma;][f_estandarización] | Proceso de estandarización                                |
| Cálculo tamaño de muestra | [Z&alpha;][f_calculo_de_muestra]        | Nivel de confianza, margen de error y proporción estimada |

> [MARKDOWN BASIC SYNTAX GUIDE](https://www.markdownguide.org/basic-syntax/)

> [FÓRMULAS ESTADÍSTICAS](https://www.estadistica.net/Algoritmos2/pau.html)

[f_estandarización]: #fórmula-de-proceso-de-estandarización-🔋
[f_calculo_de_muestra]: #5-cálculo-de-tamaño-de-muestra-🔋
