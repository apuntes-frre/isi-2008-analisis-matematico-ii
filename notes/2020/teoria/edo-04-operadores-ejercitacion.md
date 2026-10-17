# Ecuaciones diferenciales ordinarias — Parte 4

> Fuente: `2020/15-EDO 2do Orden/Apunte Ecuaciones Diferenciales.pdf`. Apunte de
> las clases del Ing. Leopoldo S. de Urrutia. Universidad Tecnológica Nacional,
> Facultad Regional Resistencia. Sin año impreso. Desde el segundo tema de la
> página impresa 37 hasta 45 (PDF 39–47). Las expresiones se conservan,
> incluidas las erratas. Procedencia en
> [cobertura](../../../resources/2020/documentos-pdf-cobertura.md).

## Página 37 — Método Abreviado que comprende OPERADORES

En casi todos los casos que en la práctica se presentan, el método de los
coeficientes indeterminados, complementado por el de variación de parámetros,
bastan para resolver cualquier tipo de ecuación lineal a coeficientes
constantes. Hace algún tiempo los científicos tienen la necesidad creciente de
familiarizarse con los llamados “Métodos Operacionales” que simplifican
extremadamente las interpretaciones.

Consideremos una ecuación diferencial lineal $`\phi(D)y=f(x)`$ (1) en la que
$`\phi(D)`$ es el operador lineal polinómico de grado $`n`$, es decir:

```math
\phi(D)=a_0D^n+a_1D^{n-1}+a_2D^{n-2}+\cdots+a_{n-1}D+a_n
```

expresión en la que consideraremos $`a_0,a_1,a_2,\ldots,a_n`$ constantes dadas.

Si “despejamos” formalmente el valor de “$`y`$” en (1), tratando algebraicamente
a la ecuación, se tiene $`y=\frac1{\phi(D)}f(x)`$, en lo obtenido
$`\frac1{\phi(D)}`$ representa una operación que deberá efectuarse a $`f(x)`$.

## Página 38

La pregunta que necesita respuesta es: ¿Cuál es la naturaleza de esa operación?
Para tener una idea de la respuesta, analicemos una ecuación diferencial
sencilla $`y'=x`$ o $`Dy=x\Rightarrow y=\frac1D x`$; ¿qué significa esta
expresión?

Tendremos una guía si resolvemos la ecuación diferencial

```math
y'=x\quad\text{ó}\quad\frac{dy}{dx}=x
\Rightarrow dy=x\,dx\quad\therefore\quad y=\int x\,dx
```

por consiguiente es natural admitir, comparando con la expresión anterior, que

```math
\frac1D x=\int x\,dx\tag{2}
```

esto nos sugiere la siguiente interpretación: la operación de “multiplicar” una
función por $`1/D`$ corresponde a una “integración” de dicha función. Sería
natural entonces plantearnos otras preguntas, tales como: $`1/D^2`$ ¿representa
una doble integración?, si es así, la expresión $`1/D^n`$ corresponde a la
“enésima integración”.

Tratemos de aclarar estas incógnitas. Los operadores $`1/D,1/D^2,1/D^3,\ldots,
1/D^n`$ se llaman **operadores inversos**. Observemos otros operadores
$`(D-p)y=f(x)`$ donde $`p=`$ cte o $`y'-py=f(x)`$ despejando tenemos

```math
y=\frac1{D-p}f(x)
```

veamos como interpretarlo.

Si resolvemos la ecuación diferencial dada exactamente, obtenemos

```math
y=e^{px}\int e^{-px}f(x)\,dx
```

por lo tanto

```math
\frac1{D-p}f(x)=e^{px}\int e^{-px}f(x)\,dx
```

Advertimos en esta expresión que si $`p=0\land f(x)=x`$, se reproduce la vista
en el paso anterior (2).

Nos interesa también preguntarnos el significado de

```math
(D-p_1)(D-p_2)y=f(x)\tag{3}
```

donde $`p_1\land p_2`$ son constantes veamos que representa, sabemos que la
expresión:

```math
(D-p_2)y=y'-p_2y=\frac{dy}{dx}-p_2y
```

por lo tanto es admisible escribir:

## Página 39

```math
\begin{aligned}
(D-p_1)(D-p_2)y
&=\left(\frac d{dx}-p_1\right)\left(\frac{dy}{dx}-p_2y\right)\\
&=\frac d{dx}\left(\frac{dy}{dx}-p_2y\right)
-p_1\left(\frac{dy}{dx}-p_2y\right)\\
&=\frac{d^2y}{dx^2}-\frac{dy}{dx}(p_1+p_2)+yp_1p_2\\
&=[D^2-(p_1+p_2)D+p_1p_2]y
\end{aligned}
```

como vemos el operador $`(D-p_1)(D-p_2)`$ equivale a $`D^2-(p_1+p_2)D+p_1p_2`$,
de forma análoga, se puede establecer una equivalencia inversa. De todo lo visto
se deduce que los operadores se pueden multiplicar y factorizar como si fueran
cantidades algebraicas siempre que $`p_1,p_2,\ldots,p_n`$ sean constantes.

Podemos demostrar (basándonos en las propiedades de raíces o ceros de un
polinomio) que la factorización conveniente.

```math
a_0D^n+a_1D^{n-1}+a_2D^{n-2}+\cdots+a_{n-1}D+a_n
=a_0(D-p_1)(D-p_2)\cdots(D-p_n)
```

siempre que $`a_0,a_1,a_2,\ldots,a_n`$ sean constantes, por tanto también
$`p_1,p_2,\ldots,p_n`$. Además el orden de estos factores es indiferente, es
decir, los operadores obedecen a las leyes formales que se verifican para
cantidades algebraicas. Este hecho permite tratar la ecuación (3) de la misma
forma que la hemos tratado a las otras ecuaciones, o sea “despejando” tenemos.

```math
y=\frac1{(D-p_1)(D-p_2)}f(x)
```

aplicando la integración

```math
\begin{aligned}
y&=\frac1{D-p_1}\left[e^{p_2x}\int e^{-p_2x}f(x)\,dx\right]\\
&=e^{p_1x}\int e^{-p_1x}\left[e^{p_2x}\int e^{-p_2x}f(x)\,dx\right]dx
\end{aligned}
```

de manera análoga podemos escribir, generalizando

```math
\frac1{(D-p_1)(D-p_2)\cdots(D-p_n)}
=e^{-p_1x}\int e^{p_1x}e^{-p_2x}\int e^{p_2x}e^{-p_3x}\cdots
\int e^{p_nx}f(x)\,dx^n\tag{4}
```

basándonos en el cumplimiento de las reglas formales por parte de

## Página 40

los operadores, es posible practicar la descomposición en fracciones simples

```math
\frac1{(D-p_1)(D-p_2)\cdots(D-p_n)}
=\frac{A_1}{D-p_1}+\frac{A_2}{D-p_2}+\cdots+\frac{A_n}{D-p_n}
```

determinando adecuadamente $`A_1,A_2,\ldots,A_n`$, se verifica la identidad

```math
\frac1{(D-p_1)(D-p_2)\cdots(D-p_n)}f(x)
=\frac{A_1}{D-p_1}f(x)+\frac{A_2}{D-p_2}f(x)+\cdots+\frac{A_n}{D-p_n}f(x)
```

el segundo miembro se puede interpretar, según los conceptos ya vistos,

```math
A_1e^{-p_1x}\int e^{p_1x}f(x)\,dx
+A_2e^{-p_2x}\int e^{p_2x}f(x)\,dx+\cdots
+A_ne^{-p_nx}\int e^{p_nx}f(x)\,dx
```

que resulta una interpretación más sencilla de la expresión (4).

### Ejemplo 1

Resolver: $`(D^2+4D+4)y=x^3e^{-2x}`$.

podemos expresar $`(D^2+4D+4)=(D+2)^2`$.

```math
(D+2)^2y=x^3e^{-2x}\Rightarrow y=\frac1{(D+2)^2}(x^3e^{-2x})
```

```math
=\frac1{D+2}\cdot\frac1{D+2}(x^3e^{-2x})
```

```math
\begin{aligned}
y&=\frac1{D+2}\left[e^{-2x}\int e^{2x}(x^3e^{-2x})\,dx\right]\\
&=\frac1{D+2}\left(e^{-2x}\int x^3\,dx\right)\\
&=\frac1{D+2}(e^{-2x}x^4/4)\\
&=e^{-2x}\int e^{2x}\left(e^{-2x}\frac{x^4}4\right)dx\\
&=\frac{e^{-2x}}4\int x^4\,dx=\frac{x^5}{20}e^{-2x}
\end{aligned}
```

Solución:

```math
y=\frac{x^5}{20}e^{-2x}
```

## Página 41

es evidente lo breve del método, si lo comparamos con lo laborioso que
resultaría aplicar el Método de los coeficientes indeterminados, el hecho de no
ser generalizada su aplicación reside en que es necesario saber resolver
integrales.

### Ejemplo Nº 2

Hallar la solución particular de $`(D^2-D+1)y=x^3-3x^2+1`$.

Resolución: despejando tenemos $`y=\frac1{D^2-D+1}(x^3-3x^2+1)`$.

pero

```math
\frac1{D^2-D+1}=1+D-D^3-D^4+\cdots
```

reemplazando

```math
y=\frac1{D^2-D+1}(x^3-3x^2+1)
=(1+D-D^3-D^4\ldots)(x^3-3x^2+1)
```

```math
y=1(x^3-3x^2+1)+D(x^3-3x^2+1)-D^3-D^4(x^3-3x^2+1)-\cdots
```

```math
y=x^3-6x-5
```

### Ejemplo 3

Hállese la solución de $`(D^2-1)y=e^{-x}`$.

Resolución: sabemos que $`(D^2-1)=(D-1)(D+1)`$

despejando $`y`$ tenemos:

```math
y=\frac1{(D+1)(D-1)}(e^{-x})
=\left(\frac{1/2}{D-1}-\frac{1/2}{D+1}\right)e^{-x}
```

```math
y=\frac12e^x\int e^{-x}(e^{-x})\,dx
-\frac12e^{-x}\int e^x(e^{-x})\,dx
```

```math
y=C_1e^x+C_2e^{-x}-\frac14e^{-x}-\frac12xe^{-x}
```

```math
y=Ae^x+Be^{-x}-\frac12xe^{-x}
```

## Página 42 — Ejercicios Tipo, para resolver por el alumno

Verificar si cada una de las funciones dadas es solución de la ecuación
diferencial correspondiente, sometida a la condición indicada.

1\) $`y=e^{-x}+x-1`$; $`y'+y=x`$; $`y(0)=0`$.

2\) $`y=Ae^{5x}+Be^{-2x}-\frac{e^x}2`$; $`y''-3y'-10y=6e^x`$.

3\) $`s=8\cos3t+6\mathop{\mathrm{sen}}\nolimits 3t`$; $`\frac{d^2s}{dt^2}=-9s`$;
$`s=8\land\frac{ds}{dt}=18`$ en $`t=0`$.

4\) $`1+x^2y+4y=0`$; $`y''=2x(y')^2`$; $`y'(0)=0\land y'''(0)=1/8`$.

5\) $`y=Ax^3+Bx^{-4}-\frac{x^2}3`$; $`x^2y''+12xy'-12y=2x^2`$.

6\) $`y=C_1e^{-2x}+C_2e^x+C_3e^{3x}`$; $`y'''-2y''-5y'+6y=0`$.

### Resolver las siguientes ecuaciones diferenciales a Variable Separable

1\) $`(y^2-1)\,dx-(2y+xy)\,dy=0`$

2\) $`y\,dx+(x+xy)\,dy=0`$

3\) $`x\,dx+y\,dy=xy(x\,dy-y\,dx)`$

4\) $`\cos\theta\,dr-2r\mathop{\mathrm{sen}}\nolimits \theta\,d\theta=0`$

5\) $`2r\cos\theta\,dr-\mathop{\mathrm{tg}}\nolimits \theta\,d\theta=0`$

6\) $`dx+\sqrt{a^2-x^2}\,dy=0`$

7\) $`x\sqrt{1-y}\,dy-\sqrt{1-x^2}\,dy=0`$

8\) $`x\frac{dy}{dx}+y=y^2`$

9\) $`(1+x^2)\,dy+(1+y^2)\,dx=0`$

10\) $`\mathop{\mathrm{tg}}\nolimits x\frac{dy}{dx}-2y=a`$

11\) $`x\frac{dr}{dx}=\sqrt{a^4-r^4}`$

12\) $`e^y\left(\frac{dy}{dx}+1\right)=1`$

### Resolver las ecuaciones diferenciales exactas siguientes

1\) $`(x^2+y^2)\,dx+2xy\,dy=0`$

2\) $`y\,dx+(x+y)\,dy=0`$

## Página 43

3\) $`(3x^2+2xy-y^2)\,dx+(x^2-2xy-3y^2)\,dy=0`$

4\) $`y\,dx-(y+x)\,dy=0`$

5\) $`(2xe^y+y^2e^x+2x)\,dx+(x^2e^y+2ye^x)\,dy=0`$

6\) $`x\,dy-(x^2+y)\,dx=0`$

7\) $`y^2\,dx+x^2\,dy-2xy\,dy=0`$

8\) $`x\,dy+y\,dx=y^2\,dx`$

9\) $`y(3x-2y)\,dx=-x(x-2y)\,dy`$

10\) $`y(xy+1)\,dx=x\ln x+dy`$

11\) $`\cos\theta(1+2r\cos^2\theta)\,dr
+r\mathop{\mathrm{sen}}\nolimits \theta(1-r\cos^2\theta)\,d\theta=0`$

12\) $`e^x(x+1)\,dx+(ye^y-xe^x)\,dy=0`$

### Dada las ecuaciones diferenciales Lineales, hallar su integral general

1\) $`\frac{dy}{dx}-y=e^x`$

2\) $`x\frac{dy}{dx}+2y=3x`$

3\) $`y\,dx-(2x+2y^4)\,dy=0`$

4\) $`\mathop{\mathrm{tg}}\nolimits x\frac{dy}{dx}-2y=2a`$

5\) $`x^2\,dy=(1-3x-3xy)\,dx`$

6\) $`(y^3-y)\,dx+(xy^2+x-y^2+1)\,dy=0`$

7\) $`2\cos y\,dx-(x\mathop{\mathrm{sen}}\nolimits y-y^3)\,dy=0`$

8\) $`(y^2-xy)\,dx+x^2\,dy=0`$

9\) $`y\,dy=(y^3-x)\,dx`$

10\) $`\frac{dy}{dx}+y=xy^3`$

11\)
$`x\frac{dy}{dx}+y(x\mathop{\mathrm{ctg}}\nolimits x+1)=x^2\mathop{\mathrm{tg}}\nolimits x`$

12\) $`(x^2-1)\frac{dy}{dx}+xy=x(x^2-1)`$

### Resolver las siguientes ecuaciones diferenciales Homogéneas

1\) $`xy^2\,dy=(x^3+y^3)\,dx`$

2\) $`(x-y)\,dx=2x\,dy`$

3\) $`(x^2-xy)\frac{dy}{dx}+y^2=0`$

4\) $`(1-x^2y)\frac{dy}{dx}+2xy^2=0`$

## Página 44

5\) $`2x^3\frac{dy}{dx}+(y^3-x^2y)=0`$

6\) $`2(xy^2+1)\,dy+y^3\,dx=0`$

7\) $`y(3-xy)\,dx+x(2-xy)\,dy=0`$

8\) $`(x+2x^2y)\,dy+(2y+3xy^2)\,dx=0`$

9\) $`(x^2y+x)\frac{dy}{dx}+(xy^2-y)=0`$

10\) $`(x^2+2y^3)\,dx+3xy^2\,dy=0`$

### Resolver las ecuaciones a coeficientes constantes de orden superior

1\) $`\frac{d^2y}{dx^2}+\frac{dy}{dx}=0`$

2\) $`y''+2y'-3y=0`$

3\) $`(D^2+D-2)y=0`$

4\) $`(D^3-2D^2-3D)y=0`$

5\) $`y''+y=0`$

6\) $`\frac{d^2y}{dx^2}-2\frac{dy}{dx}+2y=0`$

7\) $`(D^2-4)y=e^x`$

8\) $`y''-y=x`$

9\) $`y''-2y'+y=2e^{2x}`$

10\) $`(D^2+4)y=\cos x`$

11\) $`\frac{d^2y}{dx^2}+4\frac{dy}{dx}+3y=1+5\cos x`$

12\) $`(D^2-D)=x^2`$

13\) $`(D^2+1)y=\mathop{\mathrm{sen}}\nolimits x`$

14\) $`(D^2+2D)=3xe^x`$

15\) $`\frac{d^2y}{dx^2}+9y=4x\mathop{\mathrm{sen}}\nolimits x`$

16\) $`y''-3y'=2e^{2x}\mathop{\mathrm{sen}}\nolimits x`$

17\) $`\frac{d^2y}{dx^2}+\frac{dy}{dx}-2y=e^x+e^{2x}`$

18\) $`y''-y=x^2+\cos2x`$

19\) $`(D^2-4D-5)y=e^{2x}+4\mathop{\mathrm{sen}}\nolimits x`$

20\) $`(D^2-4)y=\mathop{\mathrm{sen}}\nolimits \pi x+e^x`$

21\) $`(D^2+1)y=e^{2x}+x^2`$

22\) $`(D^2+2D)y=e^x+\cos x+x`$

### Hallar las series que sean soluciones de cada una de las ecuaciones siguientes

1\) $`y'=-y;\quad y(0)=1`$

2\) $`y'=y-x`$

3\) $`y''+y=0`$

4\) $`y''+y'=0`$

## Página 45

5\) $`y'=xy;\quad y(0)=2`$

6\) $`y'=2x-3y`$

7\) $`y''=y;\quad y(0)=0;\quad y'(0)=0`$

8\) $`y''-y'-2y=0`$

En cada una de las ecuaciones diferenciales y condiciones, determínese el valor
indicado de $`Y`$ utilizando el número especificado de subdivisiones “$`n`$”. De
ser posible, compárese sus resultados con los valores que se obtengan
resolviéndolas exactamente.

| Nº | Ecuación y condición | Obténgase | Subdivisiones |
| -- | -- | -- | -- |
| 1 | $`y'=2x+y;\ y(0)=1`$ | $`y(0,5)`$ | $`n=5`$ |
| 2 | $`y'=x^2-y;\ y(1)=0`$ | $`y(1,6)`$ | $`n=6`$ |
| 3 | $`y'=(y+1)/x;\ y(2)=3`$ | $`y(2,8)`$ | $`n=8\land n=4`$ |
| 4 | $`y'=(x-y)/(x+y);\ y(0)=2`$ | $`y(1)`$ | $`n=5\land n=10`$ |
| 5 | $`y'=x^2+y^2;\ y(1)=2`$ | $`y(0,5)`$ | $`n=5\land n=10`$ |
| 6 | $`y'=\sqrt{x+y};\ y(5)=4`$ | $`y(4)`$ | $`n=5\land n=10`$ |
| 7 | $`y'=y^2+\sqrt y;\ y(0)=5`$ | $`y(1)`$ | $`n=5\land n=10`$ |
