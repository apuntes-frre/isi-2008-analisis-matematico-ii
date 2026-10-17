# Derivada direccional y gradiente para funciones de tres variables

Fuente: `Gradiente.pdf`, páginas 1–3.
[Procedencia](../../../resources/2016/fuentes.md).

Sea $`f(x,y,z)`$ una función con derivadas parciales de primer orden continuas.
La derivada direccional en dirección de un vector unitario $`u=ai+bj+ck`$ está
dada por

```math
D_u f(x,y,z)=af_x(x,y,z)+bf_y(x,y,z)+cf_z(x,y,z)
```

**El gradiente de $`f`$ se define como:**

```math
\nabla f(x,y,z)=f_x(x,y,z)\boldsymbol i+f_y(x,y,z)\boldsymbol j+f_z(x,y,z)\boldsymbol k
```

**Las propiedades del gradiente son:**

1. $`D_u f(x,y,z)=\nabla f(x,y,z)\cdot\boldsymbol u`$
1. Si $`\nabla f(x,y,z)=0`$ entonces $`D_u f(x,y,z)=0`$ para todo
   $`\boldsymbol u`$
1. La dirección del máximo incremento de $`f`$ está dada por
   $`\nabla f(x,y,z)`$. El valor máximo de $`D_u f(x,y,z)`$ es
   $`\|\nabla f(x,y,z)\|`$
1. La dirección del mínimo incremento de $`f`$ está dada por
   $`-\nabla f(x,y,z)`$. El valor máximo de $`D_u f(x,y,z)`$ es
   $`-\|\nabla f(x,y,z)\|`$

## Teorema: El gradiente es normal a las curvas de nivel

Si $`f`$ es diferenciable en $`(x_0,y_0)`$ y $`\nabla f(x_0,y_0)\ne0`$, entonces
$`\nabla f(x_0,y_0)`$ es normal a la curva de nivel que pasa por $`(x_0,y_0)`$

**Nota:** Se puede generalizar para funciones de tres variables. Bajo la
hipótesis adecuadas, $`\nabla f(x_0,y_0,z_0)`$ es normal a la superficie de
nivel a través de $`(x_0,y_0,z_0)`$.

1. Dada la función $`f(x,y)=y-\mathop{\mathrm{sen}}\nolimits x`$

   a. Dibujar una curva de nivel que corresponde a $`c=0`$

   b. Hallar el gradiente de dicha función, en el punto $`(\frac\pi2,1)`$.

   c. Dibujar el vector gradiente en el mismo gráfico que ha dibujado la curva
   de nivel **Observe si se cumple el teorema anterior.**

1. Hallar el gradiente de la función en el punto dado:

   a. $`f(x,y)=2xe^{y/x}`$ en $`(2,0)`$

   b. $`w(x,y,z)=x\mathop{\mathrm{tg}}\nolimits (y+z)`$ en $`(4,3,-1)`$

1. Hallar $`D_u f(3,2)`$, donde
   $`\boldsymbol u=\frac{\boldsymbol v}{\|\boldsymbol v\|}`$, $`v=-3i-4j`$

## Definición de plano tangente y recta normal

Sea $`F`$ diferenciable en un punto $`P(x_0,y_0,z_0)`$ de la superficie $`S`$
dada por $`F(x,y,z)=0`$ tal que $`\nabla f(x_0,y_0,z_0)\ne0`$

1. Al plano que pasa por $`P`$ y es normal a $`\nabla f(x_0,y_0,z_0)`$ se lo
   llama **plano tangente a $`S`$ en $`P`$.**
1. A la recta que pasa por $`P`$ y tiene dirección de $`\nabla f(x_0,y_0,z_0)`$
   se la **llama recta normal a $`S`$ en $`P`$.**

## Teorema: Ecuación del plano tangente y recta normal

Si $`F`$ es diferenciable en $`P_0(x_0,y_0,z_0)`$, entonces una **ecuación del
plano tangente** a la superficie dada por $`F(x,y,z)=0`$ en $`P_0`$ es

```math
F_x(x_0,y_0,z_0)(x-x_0)+F_y(x_0,y_0,z_0)(y-y_0)+F_z(x_0,y_0,z_0)(z-z_0)=0
```

O bien en su expresión vectorial

```math
\nabla f(x_0,y_0,z_0)\cdot\overrightarrow{PP_0}=0
```

siendo $`\overrightarrow{PP_0}(x-x_0,y-y_0,z-z_0)`$

Las ecuaciones paramétricas de la recta normal son

```math
\begin{cases}
x=x_0+F_x(x_0,y_0,z_0)t\\
y=y_0+F_y(x_0,y_0,z_0)t\\
z=z_0+F_z(x_0,y_0,z_0)t
\end{cases}
```

1. Hallar la ecuación del plano tangente y la recta normal a la superficie en el
   punto dado:

   a) $`z=25-x^2-y^2`$ en $`(3,1,15)`$

   b) $`z=\sqrt{x^2+y^2}`$ en $`(3,4,5)`$

   c) $`x^2+y^2+z^2=9`$ en $`(1,2,2)`$

   Grafique las superficies con un graficador y compruebe que los planos
   hallados son tangentes en el punto dado.

1. **Investigación:** Considerar la función
   $`f(x,y)=\frac{4xy}{(x^2+1)(y^2+1)}`$ en los intervalos $`-2\le x\le2`$ y
   $`0\le y\le3`$

   a) Hallar un conjunto de ecuaciones paramétricas de la recta normal y una
   ecuación del plano tangente a la superficie en el punto $`(1,1,1)`$.

   b) Repetir el apartado a) para el punto $`(-1,2,-\frac45)`$

   c) Utilizar un graficador y representar gráficamente la superficie, las
   rectas normales y los planos tangentes encontrados.

   d) Utilizar la información analítica y gráfica para redactar una descripción
   breve de la superficie en los puntos indicados.

Nota de transcripción: se conserva «valor máximo» en la propiedad 4, las
variantes $`f/F`$ y la dirección/rotulación $`\overrightarrow{PP_0}`$ del
original. El ejercicio 3 de la primera página no especifica otra función.
