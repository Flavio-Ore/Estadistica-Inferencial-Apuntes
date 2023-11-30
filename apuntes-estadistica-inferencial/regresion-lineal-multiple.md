# Regresión Lineal Múltiple

El objetivo básico del Análisis de Regresión Lineal Múltiple es el de construir un modelo que permita predecir o estimar el valor de una variable Y, en base a un conjunto de variables XI, k

- A la variable Y se le llama variable dependiente, y es la que se quiere estimar o predecir.
- Las variables XI, son las variables independientes o variables predictoras.

$$ Y_i = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + ... + \beta_k X_k + \epsilon_i $$

Supuestos:

- Los residuos tienen media 0. La varianza de los residuos no depende de (homocedasticidad)
- Los residuos son normales.
- Los residuos son aleatorios.
- Las variables XI, h, etc. no están linealmente correlacionadas entre sí

El modelo poblacional de regresión lineal múltiple, independientes, es el siguiente:
Donde:
con
k
variables

- Son Parámetros desconocidos, llamados coeficientes de regresión.
** i = (0,1,2,3,...,k) Son los errores del modelo, y se suponen independientes y
2
normalmente distribuidos con media 0 y varianza

- PIXI + P2X2+...+PkXk

Estos coeficientes son calculados a partir del **método de los mínimos cuadrados**.

Resolución de Regresión Lineal Múltiple: Notación Matricial Para determinar la ecuación de regresión lineal múltiple muestral, debemos primero identificar la variable dependiente V luego las variables independientes, una vez identificados, formaremos nuestro sistema de matrices para cada uno de ellos, formando el siguiente sistema de ecuación de regresión múltiple, y ubicándolos de esta forma:

$$ Y_i =  \beta_k X_{ik} + \epsilon_i $$

Quedando el sistema de Matrices definida de la siguiente manera:
Donde:

- $Y_i$: Es la matriz de la variable Dependiente
- $X_{ik}$: Es la matriz de la variable Independiente
- $\beta_k$: Es la matriz de los coeficientes de regresión
- $\epsilon_i$: Es la matriz de los errores de estimación

$$
\left[\begin{array}{cc}
0.8944272 & 0.4472136\\
-0.4472136 & -0.8944272
\end{array}\right]
\left(\begin{array}{cc}
10 & 0\\
0 & 5
\end{array}\right)
$$

Para hallar el valor de cada uno de los coeficientes regresores B, resolveremos las siguientes operaciones matriciales:

$$ \beta = (X^TX)^{-1}X^TY $$

**Donde:**

- $X^T$: Es la matriz transpuesta de la variable Independiente
- $(X^TX)^{-1}$: Es la matriz resultante de la multiplicación de la matriz de la variable Independiente por su transpuesta
- $\beta$: Es la matriz de los coeficientes de regresión

## Coeficiente de regresión en el caso de dos variables independientes: Sistema de ecuaciones

1. $$ \sum{Y} = n\beta_0 + \beta_1 \sum{X_1} + \beta_2 \sum{X_2} $$

2. $$ \sum{X_1Y} = \beta_0 \sum{X_1} + \beta_1 \sum{X_1^2} + \beta_2 \sum{X_1X_2} $$

3. $$ \sum{X_2Y} = \beta_0 \sum{X_2} + \beta_1 \sum{X_1X_2} + \beta_2 \sum{X_2^2} $$
