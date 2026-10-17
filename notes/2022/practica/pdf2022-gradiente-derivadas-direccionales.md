# Trabajo práctico: Gradiente y derivadas direccionales

> Fuente: `2022 [Intensivo]/Derivadas Direccionales y Gradiente.pdf`. Archivo de
> 2022; sin año impreso. Procedencia y controles en
> [cobertura PDF 2022](../../../resources/2022/pdf2022-cobertura.md).

1. Definir la derivada de la función $z=f(x,y)$ en la dirección
   $\vec u=\cos\theta\vec i+\mathop{\mathrm{sen}}\nolimits \theta\vec j$.
1. Con sus propias palabras dar una descripción geométrica de la derivada
   direccional de $z=f(x,y)$.
1. Redactar un párrafo que describa la derivada direccional de la función $f$ en
   la dirección de
   $\vec u=\cos\theta\vec i+\mathop{\mathrm{sen}}\nolimits \theta\vec j$ cuando
   a) $\theta=0°$ b) $\theta=90°$.
1. Definir el gradiente de una función de dos variables.
1. Defina derivada direccional utilizando el gradiente.
1. Describir la relación del gradiente con las curvas de nivel de una superficie
   dada por $z=f(x,y)$.
1. Hallar la derivada de $f(x,y)=x^2\mathop{\mathrm{sen}}\nolimits 2y$ en el
   punto $(1,\pi/2)$, en la dirección $v=3i-4j$.
1. Halle la derivada de $f(x,y)=x^2+y^2$ en la dirección de $\theta=\frac\pi4$.
1. La temperatura en el punto $(x,y)$ de una placa metálica es
   $T=\frac{x}{x^2+y^2}$. Hallar la dirección de mayor incremento de calor en el
   punto $(3,4)$.
1. Hallar los valores de $a$, $b$ y $c$ tales que la derivada direccional de
   $f(x,y,z)=axy^2+byz+cz^2x^3$ en $(1,2,-1)$ sea máxima, igual a 64, y ocurra
   en dirección paralela al eje $z$.

**Temperatura:** La temperatura en el punto $(x,y)$ de una placa metálica se
modela mediante $T(x,y)=400e^{-(x^2+y)/2}$, $x\geq0$, $y\geq0$.

a) Utilizar un sistema computacional para representar gráficamente la función de
la distribución de la temperatura.

b) Hallar las direcciones sobre la placa, en el punto $(3,5)$, en las que no hay
cambio de calor.

c) Hallar la dirección de mayor incremento de calor en el punto $(3,5)$.

**11.** Siendo

$$
f(x,y)=\begin{cases}
\dfrac{x^3+2y^3+xy(1+2x+y)}{x^2+y^2},&(x,y)\ne(0,0),\\
0,&(x,y)=(0,0)
\end{cases}
$$

verifique que si
$\vec v=(\frac1{\sqrt2},\frac1{\sqrt2})\Rightarrow f'(\bar0,\vec v)\ne\overrightarrow{\nabla f}(\bar0)\cdot\vec v$.

**12.** Si $\ln(xz)-yz+x-1=0$ define a $z=f(x,y)$; obtenga las direcciones de
las derivadas máxima, mínima y nula de en $(1,0)$.

**13.** Dada $f(x,y,z)=4x^3-5y^2z$ calcule la derivada direccional de $f$ en
$(1,2,2)$ en la dirección de la normal exterior a $x^2+y^2+2z^2=6$ en $(2,0,1)$.

**14.** Hallar los valores de $a$, $b$ y $c$ tales que la derivada direccional
de $f(x,y,z)=axy^2+byz+cz^2x^3$ en $(1,2,-1)$ sea máxima igual a 64, y ocurra en
dirección paralela al eje $z$.

Nota de transcripción: la segunda página está en blanco. Se conserva la
repetición de los puntos 10 y 14 y «nula de en» del punto 12.
