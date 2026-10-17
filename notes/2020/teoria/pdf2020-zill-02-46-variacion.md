# 4.6 Variación de parámetros

> Transcripción del extracto *Ecuaciones diferenciales con aplicaciones de
> modelado*, atribuido a Zill por el nombre del archivo. Páginas impresas
> 157–162 (PDF 41–46), sección 4.6. Material bibliográfico externo conservado en
> la carpeta de 2020; sin portada, edición ni año verificables en la copia.

<!-- markdownlint-disable MD029 MD036 -->

## Página 157

### Repaso de material

- La variación de parámetros se introdujo por primera vez en la sección 2.3 y se
  usó de nuevo en la sección 4.2. Se recomienda dar un repaso a estas secciones.

### Introducción

El procedimiento que se utiliza para encontrar una solución particular $y_p$ de
una ecuación diferencial lineal de primer orden en un intervalo es también
aplicable a una ED de orden superior. Para adaptar el método de **variación de
parámetros** a una ecuación diferencial de segundo orden

$$
a_2(x)y''+a_1(x)y'+a_0(x)y=g(x), \tag{1}
$$

comenzamos por escribir la ecuación en su forma estándar

$$
y''+P(x)y'+Q(x)y=f(x) \tag{2}
$$

dividiendo entre el coeficiente principal $a_2(x)$. La ecuación (2) es la
análoga de segundo orden de la forma estándar de una ecuación lineal de primer
orden: $dy/dx+P(x)y=f(x)$. En (2) se supone que $P(x)$, $Q(x)$ y $f(x)$ son
continuas en algún intervalo común $I$. Como ya hemos visto en la sección 4.3,
no hay dificultad para obtener la función complementaria $y_c$, la solución
general de la ecuación homogénea asociada de (2), cuando los coeficientes son
constantes.

## Página 158

### Suposiciones

Correspondiendo con la suposición $y_p=u_1(x)y_1(x)$ que se usó en la sección
2.3 para encontrar una solución particular $y_p$ de $dy/dx+P(x)y=f(x)$, para la
ecuación lineal de segundo orden (2) se busca una solución de la forma

$$
y_p=u_1(x)y_1(x)+u_2(x)y_2(x), \tag{3}
$$

donde $y_1$ y $y_2$ forman un conjunto fundamental de soluciones en $I$ de la
forma homogénea asociada de (1). Usando la regla del producto para derivar dos
veces a $y_p$, se obtiene

$$
\begin{aligned}
y_p'&=u_1y_1'+y_1u_1'+u_2y_2'+y_2u_2'\\
y_p''&=u_1y_1''+y_1'u_1'+y_1u_1''+u_1'y_1'
+u_2y_2''+y_2'u_2'+y_2u_2''+u_2'y_2'.
\end{aligned}
$$

Sustituyendo la ecuación (3) y las derivadas anteriores en (2) y agrupando
términos se obtiene

$$
\begin{aligned}
y_p''+P(x)y_p'+Q(x)y_p
&=u_1\underbrace{[y_1''+Py_1'+Qy_1]}_{\text{cero}}
+u_2\underbrace{[y_2''+Py_2'+Qy_2]}_{\text{cero}}
+y_1u_1''+u_1'y_1'\\
&\quad+y_2u_2''+u_2'y_2'+P[y_1u_1'+y_2u_2']+y_1'u_1'+y_2'u_2'\\
&=\frac d{dx}[y_1u_1']+\frac d{dx}[y_2u_2']
+P[y_1u_1'+y_2u_2']+y_1'u_1'+y_2'u_2'\\
&=\frac d{dx}[y_1u_1'+y_2u_2']+P[y_1u_1'+y_2u_2']
+y_1'u_1'+y_2'u_2'=f(x).
\end{aligned} \tag{4}
$$

Como se busca determinar dos funciones desconocidas $u_1$ y $u_2$, la razón
impone que son necesarias dos ecuaciones. Estas ecuaciones se obtienen con la
suposición adicional de que las funciones $u_1$ y $u_2$ satisfacen
$y_1u_1'+y_2u_2'=0$. Esta suposición en azul no se presenta por sorpresa, sino
que es resultado de los dos primeros términos de (4) puesto que si se requiere
que $y_1u_1'+y_2u_2'=0$, entonces (4) se reduce a $y_1'u_1'+y_2'u_2'=f(x)$.
Ahora tenemos nuestras dos ecuaciones deseadas, a pesar de que sean dos
ecuaciones para determinar las derivadas $u_1'$ y $u_2'$. Por la regla de
Cramer, la solución del sistema

$$
\begin{aligned}
y_1u_1'+y_2u_2'&=0\\
y_1'u_1'+y_2'u_2'&=f(x)
\end{aligned}
$$

puede expresarse en términos de determinantes:

$$
u_1'=\frac{W_1}{W}=-\frac{y_2f(x)}W
\quad\text{y}\quad
u_2'=\frac{W_2}{W}=\frac{y_1f(x)}W, \tag{5}
$$

donde

$$
W=\begin{vmatrix}y_1&y_2\\y_1'&y_2'\end{vmatrix},\quad
W_1=\begin{vmatrix}0&y_2\\f(x)&y_2'\end{vmatrix},\quad
W_2=\begin{vmatrix}y_1&0\\y_1'&f(x)\end{vmatrix}. \tag{6}
$$

Las funciones $u_1$ y $u_2$ se encuentran integrando los resultados de (5). El
determinante $W$ se reconoce como el Wronskiano de $y_1$ y $y_2$. Por la
independencia lineal de $y_1$ y $y_2$ en $I$, se sabe que $W(y_1(x),y_2(x))\ne0$
para toda $x$ en el intervalo.

### Resumen del método

Normalmente, no es buena idea memorizar fórmulas en lugar de entender un
procedimiento. Sin embargo, el procedimiento anterior es demasiado largo y
complicado para usarse cada vez que se desee resolver una ecuación diferencial.
En este caso resulta más eficaz usar simplemente las fórmulas de (5). Así que
para resolver $a_2y''+a_1y'+a_0y=g(x)$, primero se encuentra la función
complementaria $y_c=c_1y_1+c_2y_2$ y luego se calcula el Wronskiano
$W(y_1(x),y_2(x))$. Dividiendo entre $a_2$, se escribe la ecuación en la forma
estándar $y''+Py'+Qy=f(x)$ para determinar $f(x)$. Se encuentra $u_1$ y $u_2$
integrando $u_1'=W_1/W$ y $u_2'=W_2/W$, donde $W_1$ y $W_2$ se definen como en
(6). Una solución particular es $y_p=u_1y_1+u_2y_2$. Entonces la solución
general de la ecuación es $y=y_c+y_p$.

## Página 159

### Ejemplo 1. Solución general usando variación de parámetros

Resuelva $y''-4y'+4y=(x+1)e^{2x}$.

**Solución.** De la ecuación auxiliar $m^2-4m+4=(m-2)^2=0$ se tiene
$y_c=c_1e^{2x}+c_2xe^{2x}$. Con las identificaciones $y_1=e^{2x}$ y
$y_2=xe^{2x}$, a continuación se calcula el Wronskiano:

$$
W(e^{2x},xe^{2x})=
\begin{vmatrix}e^{2x}&xe^{2x}\\2e^{2x}&2xe^{2x}+e^{2x}\end{vmatrix}=e^{4x}.
$$

Puesto que la ecuación diferencial dada ya está en la forma (2) (es decir, el
coeficiente de $y''$ es 1), identificamos $f(x)=(x+1)e^{2x}$. De (6), obtenemos

$$
W_1=\begin{vmatrix}0&xe^{2x}\\(x+1)e^{2x}&2xe^{2x}+e^{2x}\end{vmatrix}
=-(x+1)xe^{4x},
$$

$$
W_2=\begin{vmatrix}e^{2x}&0\\2e^{2x}&(x+1)e^{2x}\end{vmatrix}=(x+1)e^{4x},
$$

y así de (5)

$$
u_1'=-\frac{(x+1)xe^{4x}}{e^{4x}}=-x^2-x,\qquad
u_2'=\frac{(x+1)e^{4x}}{e^{4x}}=x+1.
$$

Se tiene que $u_1=-\frac13x^3-\frac12x^2$ y $u_2=\frac12x^2+x$. Por tanto

$$
y_p=\left(-\frac13x^3-\frac12x^2\right)e^{2x}
+\left(\frac12x^2+x\right)xe^{2x}
=\frac16x^3e^{2x}+\frac12x^2e^{2x}
$$

y

$$
y=y_c+y_p=c_1e^{2x}+c_2xe^{2x}+\frac16x^3e^{2x}+\frac12x^2e^{2x}.
$$

### Ejemplo 2. Solución general usando variación de parámetros

Resuelva $4y''+36y=\csc3x$.

**Solución.** Primero se escribe la ecuación en la forma estándar (2) dividiendo
entre 4:

$$
y''+9y=\frac14\csc3x.
$$

Debido a que las raíces de la ecuación auxiliar $m^2+9=0$ son $m_1=3i$ y
$m_2=-3i$, la función complementaria es
$y_c=c_1\cos3x+c_2\mathop{\mathrm{sen}}\nolimits 3x$. Usando $y_1=\cos3x$,
$y_2=\mathop{\mathrm{sen}}\nolimits 3x$, y $f(x)=\frac14\csc3x$, obtenemos

$$
W(\cos3x,\mathop{\mathrm{sen}}\nolimits 3x)=
\begin{vmatrix}\cos3x&\mathop{\mathrm{sen}}\nolimits 3x\\
-3\mathop{\mathrm{sen}}\nolimits 3x&3\cos3x\end{vmatrix}=3,
$$

$$
W_1=\begin{vmatrix}0&\mathop{\mathrm{sen}}\nolimits 3x\\\frac14\csc3x&3\cos3x\end{vmatrix}
=-\frac14,\qquad
W_2=\begin{vmatrix}\cos3x&0\\-3\mathop{\mathrm{sen}}\nolimits 3x&\frac14\csc3x\end{vmatrix}
=\frac14\frac{\cos3x}{\mathop{\mathrm{sen}}\nolimits 3x}.
$$

Integrando

$$
u_1'=\frac{W_1}W=-\frac1{12}\quad\text{y}\quad
u_2'=\frac{W_2}W=\frac1{12}\frac{\cos3x}{\mathop{\mathrm{sen}}\nolimits 3x}
$$

Se obtiene $u_1=-\frac1{12}x$ y
$u_2=\frac1{36}\ln|\mathop{\mathrm{sen}}\nolimits 3x|$. Así una solución
particular es

$$
y_p=-\frac1{12}x\cos3x+\frac1{36}(\mathop{\mathrm{sen}}\nolimits 3x)\ln|\mathop{\mathrm{sen}}\nolimits 3x|.
$$

La solución general de la ecuación es

$$
y=y_c+y_p=c_1\cos3x+c_2\mathop{\mathrm{sen}}\nolimits 3x-\frac1{12}x\cos3x
+\frac1{36}(\mathop{\mathrm{sen}}\nolimits 3x)\ln|\mathop{\mathrm{sen}}\nolimits 3x|. \tag{7}
$$

## Página 160

La ecuación (7) representa la solución general de la ecuación diferencial en,
digamos, el intervalo $(0,\pi/6)$.

### Constantes de integración

Cuando se calculan las integrales indefinidas de $u_1'$ y $u_2'$, no es
necesario introducir algunas constantes. Esto es porque

$$
\begin{aligned}
y=y_c+y_p&=c_1y_1+c_2y_2+(u_1+a_1)y_1+(u_2+b_1)y_2\\
&=(c_1+a_1)y_1+(c_2+b_1)y_2+u_1y_1+u_2y_2\\
&=C_1y_1+C_2y_2+u_1y_1+u_2y_2.
\end{aligned}
$$

### Ejemplo 3. Solución general usando variación de parámetros

Resuelva $y''-y=\frac1x$.

**Solución.** La ecuación auxiliar $m^2-1=0$ produce $m_1=-1$ y $m_2=1$. Por
tanto $y_c=c_1e^x+c_2e^{-x}$. Ahora $W(e^x,e^{-x})=-2$, y

$$
u_1'=-\frac{e^{-x}(1/x)}{-2},\qquad
u_1=\frac12\int_{x_0}^x\frac{e^{-t}}t\,dt,
$$

$$
u_2'=\frac{e^x(1/x)}{-2},\qquad
u_2=-\frac12\int_{x_0}^x\frac{e^t}t\,dt.
$$

Puesto que las integrales anteriores son no elementales, nos vemos obligados a
escribir

$$
y_p=\frac12e^x\int_{x_0}^x\frac{e^{-t}}t\,dt
-\frac12e^{-x}\int_{x_0}^x\frac{e^t}t\,dt,
$$

y por tanto

$$
y=y_c+y_p=c_1e^x+c_2e^{-x}
+\frac12e^x\int_{x_0}^x\frac{e^{-t}}t\,dt
-\frac12e^{-x}\int_{x_0}^x\frac{e^t}t\,dt. \tag{8}
$$

En el ejemplo 3 se puede integrar en algún intervalo $[x_0,x]$ que no contenga
al origen.

### Ecuaciones de orden superior

El método que se describió para ecuaciones diferenciales no homogéneas de
segundo orden se puede generalizar a ecuaciones lineales de $n$-ésimo orden que
se han escrito en forma estándar

$$
y^{(n)}+P_{n-1}(x)y^{(n-1)}+\cdots+P_1(x)y'+P_0(x)y=f(x). \tag{9}
$$

Si $y_c=c_1y_1+c_2y_2+\cdots+c_ny_n$ es la función complementaria para (9),
entonces una solución particular es

$$
y_p=u_1(x)y_1(x)+u_2(x)y_2(x)+\cdots+u_n(x)y_n(x),
$$

donde los $u_k'$, $k=1,2,\ldots,n$ se determinan por las $n$ ecuaciones

$$
\begin{aligned}
y_1u_1'+y_2u_2'+\cdots+y_nu_n'&=0\\
y_1'u_1'+y_2'u_2'+\cdots+y_n'u_n'&=0\\
&\ \vdots\\
y_1^{(n-1)}u_1'+y_2^{(n-1)}u_2'+\cdots+y_n^{(n-1)}u_n'&=f(x).
\end{aligned} \tag{10}
$$

## Página 161

Las primeras $n-1$ ecuaciones de este sistema, al igual que $y_1u_1'+y_2u_2'=0$
en (4), son suposiciones que se hacen para simplificar la ecuación resultante
después de que $y_p=u_1(x)y_1(x)+\cdots+u_n(x)y_n(x)$ se sustituye en (9). En
este caso usando la regla de Cramer se obtiene

$$
u_k'=\frac{W_k}W,\quad k=1,2,\ldots,n,
$$

donde $W$ es el Wronskiano de $y_1,y_2,\ldots,y_n$ y $W_k$ es el determinante
que se obtiene al remplazar la $k$-ésima columna del Wronskiano por la columna
formada por el lado derecho de (10), es decir, la columna que consta de
$(0,0,\ldots,f(x))$. Cuando $n=2$, se obtiene la ecuación (5). Cuando $n=3$, la
solución particular $y_p=u_1y_1+u_2y_2+u_3y_3$, donde $y_1$, $y_2$ y $y_3$
constituyen un conjunto linealmente independiente de soluciones de la ED
homogénea asociada y $u_1$, $u_2$ y $u_3$ se determinan a partir de

$$
u_1'=\frac{W_1}W,\quad u_2'=\frac{W_2}W,\quad u_3'=\frac{W_3}W, \tag{11}
$$

$$
W_1=\begin{vmatrix}0&y_2&y_3\\0&y_2'&y_3'\\f(x)&y_2''&y_3''\end{vmatrix},
\quad
W_2=\begin{vmatrix}y_1&0&y_3\\y_1'&0&y_3'\\y_1''&f(x)&y_3''\end{vmatrix},
$$

$$
W_3=\begin{vmatrix}y_1&y_2&0\\y_1'&y_2'&0\\y_1''&y_2''&f(x)\end{vmatrix},
\quad
W=\begin{vmatrix}y_1&y_2&y_3\\y_1'&y_2'&y_3'\\y_1''&y_2''&y_3''\end{vmatrix}.
$$

Véanse los problemas 25 y 26 de los ejercicios 4.6.

### Comentarios

i) La variación de parámetros tiene una ventaja particular sobre el método de
coeficientes indeterminados en cuanto a que *siempre* produce una solución
particular $y_p$, siempre y cuando se pueda resolver la ecuación homogénea
asociada. Este método no se limita a una función $f(x)$ que es una combinación
de las cuatro clases que se listan en la página 141. Como se verá en la
siguiente sección, la variación de parámetros, a diferencia de los coeficientes
indeterminados, es aplicable a ED lineales con coeficientes variables.

ii) En los problemas siguientes, no dude en simplificar la forma de $y_p$.
Dependiendo de cómo se encuentren las antiderivadas de $u_1'$ y $u_2'$, es
posible que no se obtenga la misma $y_p$ que se da en la sección de respuestas.
Por ejemplo, en el problema 3 de los ejercicios 4.6 tanto
$y_p=\frac12\mathop{\mathrm{sen}}\nolimits x-\frac12x\cos x$ como
$y_p=\frac14\mathop{\mathrm{sen}}\nolimits x-\frac12x\cos x$ son respuestas
válidas. En cualquier caso la solución general $y=y_c+y_p$ se simplifica a
$y=c_1\cos x+c_2\mathop{\mathrm{sen}}\nolimits x-\frac12x\cos x$. ¿Por qué?

### Ejercicios 4.6

*Las respuestas a los problemas con número impar comienzan en la página RES-5.*

En los problemas 1 a 18 resuelva cada ecuación diferencial por medio de
variación de parámetros.

1. $y''+y=\sec x$
1. $y''+y=\tan x$
1. $y''+y=\mathop{\mathrm{sen}}\nolimits x$
1. $y''+y=\sec\theta\tan\theta$
1. $y''+y=\cos^2x$
1. $y''+y=\sec^2x$
1. $y''-y=\cosh x$
1. $y''-y=\mathop{\mathrm{senh}}\nolimits 2x$
1. $y''-4y=e^{2x}/x$
1. $y''-9y=9x/e^{3x}$
1. $y''+3y'+2y=1/(1+e^x)$
1. $y''-2y'+y=e^x/(1+x^2)$
1. $y''+3y'+2y=\mathop{\mathrm{sen}}\nolimits e^x$
1. $y''-2y'+y=e^t\arctan t$
1. $y''+2y'+y=e^{-t}\ln t$
1. $2y''+2y'+y=4\sqrt{x}$
1. $3y''-6y'+6y=e^x\sec x$
1. $4y''-4y'+y=e^{x/2}\sqrt{1-x^2}$

## Página 162 (fin de sección 4.6)

En los problemas 19 a 22 resuelva cada ecuación diferencial mediante variación
de parámetros, sujeta a las condiciones iniciales $y(0)=1$, $y'(0)=0$.

19. $4y''-y=xe^{x/2}$
01. $2y''+y'-y=x+1$
01. $y''+2y'-8y=2e^{-2x}-e^{-x}$
01. $y''-4y'+4y=(12x^2-6x)e^{2x}$

En los problemas 23 y 24 las funciones que se indican son soluciones linealmente
independientes de la ecuación diferencial homogénea asociada en $(0,\infty)$.
Determine la solución general de la ecuación homogénea.

23. $x^2y''+xy'+(x^2-\frac14)y=x^{3/2};$

    $y_1=x^{-1/2}\cos x,\ y_2=x^{-1/2}\mathop{\mathrm{sen}}\nolimits x$

01. $x^2y''+xy'+y=\sec(\ln x);$

    $y_1=\cos(\ln x),\ y_2=\mathop{\mathrm{sen}}\nolimits (\ln x)$

En los problemas 25 y 26 resuelva la ecuación diferencial de tercer orden usando
variación de parámetros.

25. $y'''+y'=\tan x$
01. $y'''+4y'=\sec2x$

### Problemas para analizar

En los problemas 27 y 28 analice cómo pueden combinarse los métodos de
coeficientes indeterminados y variación de parámetros para resolver la ecuación
diferencial. Lleve a cabo sus ideas.

27. $3y''-6y'+30y=15\mathop{\mathrm{sen}}\nolimits x+e^x\tan3x$

01. $y''-2y'+y=4x^2-3+x^{-1}e^x$

01. ¿Cuáles son los intervalos de definición de las soluciones generales en los
    problemas 1, 7, 9 y 18? Analice por qué el intervalo de definición de la
    solución del problema 24 *no* es $(0,\infty)$.

01. Encuentre la solución general de $x^4y''+x^3y'-4x^2y=1$ dado que $y_1=x^2$
    es una solución de la ecuación homogénea asociada.

01. Suponga que $y_p(x)=u_1(x)y_1(x)+u_2(x)y_2(x)$, donde $u_1$ y $u_2$ están
    definidas por (5) es una solución particular de (2) en un intervalo $I$ para
    el que $P$, $Q$ y $f$ son continuas. Demuestre que $y_p$ se puede escribir
    como

    $$
    y_p(x)=\int_{x_0}^xG(x,t)f(t)\,dt, \tag{12}
    $$

    donde $x$ y $x_0$ están en $I$,

    $$
    G(x,t)=\frac{y_1(t)y_2(x)-y_1(x)y_2(t)}{W(t)}, \tag{13}
    $$

    y $W(t)=W(y_1(t),y_2(t))$ es el Wronskiano. La función $G(x,t)$ en (13) se
    llama la **función de Green** para la ecuación diferencial (2).

01. Use (13) para construir la función de Green para la ecuación diferencial del
    ejemplo 3. Exprese la solución general dada en (8) en términos de la
    solución particular (12).

01. Compruebe que (12) es una solución del problema con valores iniciales

    $$
    \frac{d^2y}{dx^2}+P\frac{dy}{dx}+Qy=f(x),\quad y(x_0)=0,\quad y'(x_0)=0
    $$

    en el intervalo $I$. \[*Sugerencia:* Busque la regla de Leibniz para derivar
    bajo un signo de integral.\]

01. Use los resultados de los problemas 31 y 33 y la función de Green encontrada
    del problema 32 para encontrar una solución del problema con valores
    iniciales

    $$
    y''-y=e^{2x},\quad y(0)=0,\quad y'(0)=0
    $$

    usando (12). Evalúe la integral.

## Nota de transcripción

Se conserva “solución general de la ecuación homogénea” en la instrucción de los
ejercicios 23 y 24, aunque las ecuaciones mostradas tienen miembro derecho no
nulo. No se corrige el enunciado ni se resuelven los ejercicios.
