# Teorema: Ecuación del plano tangente y recta normal

> Fuente: `2022 [Intensivo]/Plano tangente-Linealización.pdf`. Archivo de 2022;
> sin año impreso. Procedencia y controles en
> [cobertura PDF 2022](../../../resources/2022/pdf2022-cobertura.md).

Si $`F`$ es diferenciable en $`P_0(x_0,y_0,z_0)`$, entonces una **ecuación del
plano tangente** a la superficie dada por $`F(x,y,z)=0`$ en $`P_0`$ es

```math
F_x(x_0,y_0,z_0)(x-x_0)+F_y(x_0,y_0,z_0)(y-y_0)+F_z(x_0,y_0,z_0)(z-z_0)=0.
```

O bien en su expresión vectorial

```math
\nabla f(x_0,y_0,z_0)\cdot\overrightarrow{PP_0}=0
\quad\text{siendo }\overrightarrow{PP_0}\ (x-x_0,y-y_0,z-z_0).
```

Las ecuaciones paramétricas de la recta normal son

```math
\begin{cases}
x=x_0+F_x(x_0,y_0,z_0)t,\\
y=y_0+F_y(x_0,y_0,z_0)t,\\
z=z_0+F_z(x_0,y_0,z_0)t.
\end{cases}
```

**1.-** Hallar la ecuación del plano tangente y la recta normal a la superficie
en el punto dado:

a) $`z=25-x^2-y^2`$ en $`(3,1,15)`$.

b) $`z=\sqrt{x^2+y^2}`$ en $`(3,4,5)`$.

c) $`x^2+y^2+z^2=9`$ en $`(1,2,2)`$.

Grafique las superficies con un graficador y compruebe que los planos hallados
son tangentes en el punto dado.

**11-16** Explique por qué la función es diferenciable en el punto dado. Luego
determine la linealización $`L(x,y)`$ de la función en ese punto.

**11.** $`f(x,y)=1+x\ln(xy-5)`$, $`(2,3)`$.

**12.** $`f(x,y)=x^3y^4`$, $`(1,1)`$.

**13.** $`f(x,y)=\frac{x}{x+y}`$, $`(2,1)`$.

**14.** $`f(x,y)=\sqrt{x+e^{4y}}`$, $`(3,0)`$.

Nota de transcripción: el original alterna $`F`$ y $`f`$ y escribe
$`\overrightarrow{PP_0}`$ con componentes $`(x-x_0,y-y_0,z-z_0)`$; se conserva.
El encabezado dice 11-16, pero solamente incluye 11-14.
