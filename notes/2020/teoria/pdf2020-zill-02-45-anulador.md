# 4.5 Coeficientes indeterminados: método del anulador

> Transcripción del extracto *Ecuaciones diferenciales con aplicaciones de
> modelado*, atribuido a Zill por el nombre del archivo. Páginas impresas
> 150–157 (PDF 34–41), hasta el final de los ejercicios 4.5. Material
> bibliográfico externo conservado en la carpeta de 2020; la copia no contiene
> portada y no se infiere edición ni año.

<!-- markdownlint-disable MD029 MD036 -->

## Página 150

### Repaso de material

- Repaso de teoremas 4.1.6 y 4.1.7 (sección 4.1).

### Introducción

En la sección 4.1 vimos que una ecuación diferencial de $n$-ésimo orden se puede
escribir como

$$
a_nD^ny+a_{n-1}D^{n-1}y+\cdots+a_1Dy+a_0y=g(x), \tag{1}
$$

donde $D^ky=d^ky/dx^k$, $k=0,1,\ldots,n$. Cuando es adecuado, la ecuación (1)
también se escribe como $L(y)=g(x)$, donde $L$ denota el operador diferencial o
polinomial, lineal de $n$-ésimo orden

$$
a_nD^n+a_{n-1}D^{n-1}+\cdots+a_1D+a_0. \tag{2}
$$

La notación de operador no sólo es una abreviatura útil, sino que en un nivel
muy práctico la aplicación de operadores diferenciales permite justificar las
reglas un poco abrumadoras para determinar la forma de solución particular $y_p$
presentada en la sección anterior. En esta sección no hay reglas especiales; la
forma de $y_p$ se deduce casi de manera automática una vez que se encuentra un
operador diferencial lineal adecuado que *anula* a $g(x)$ en (1). Antes de
investigar cómo se realiza esto, es necesario analizar dos conceptos.

### Factorización de operadores

Cuando los coeficientes $a_i$, $i=0,1,\ldots,n$ son constantes reales, un
operador diferencial lineal (1) se puede factorizar siempre el polinomio
característico $a_nm^n+a_{n-1}m^{n-1}+\cdots+a_1m+a_0$ sea factorizable. En
otras palabras, si $r_1$ es una raíz de la ecuación auxiliar

$$
a_nm^n+a_{n-1}m^{n-1}+\cdots+a_1m+a_0=0,
$$

entonces $L=(D-r_1)P(D)$, donde la expresión polinomial $P(D)$ es un operador
diferencial lineal de orden $n-1$. Por ejemplo, si se trata a $D$ como una
cantidad algebraica, entonces el operador $D^2+5D+6$ se puede factorizar como
$(D+2)(D+3)$ o como $(D+3)(D+2)$. Así si una función $y=f(x)$ tiene una segunda
derivada, entonces

$$
(D^2+5D+6)y=(D+2)(D+3)y=(D+3)(D+2)y.
$$

Esto muestra una propiedad general:

*Los factores de un operador diferencial con coeficientes constantes conmutan.*

Una ecuación diferencial tal como $y''+4y'+4y=0$ se escribe como

$$
(D^2+4D+4)y=0\quad\text{o}\quad(D+2)(D+2)y=0
\quad\text{o}\quad(D+2)^2y=0.
$$

### Operador anulador

Si $L$ es un operador diferencial lineal con coeficientes constantes y $f$ es
una función suficientemente derivable tal que

$$
L(f(x))=0,
$$

entonces se dice que $L$ es un **anulador** de la función. Por ejemplo, $D$
anula una función constante $y=k$ puesto que $Dk=0$. El operador diferencial
$D^2$ anula la función $y=x$ puesto que la primera y la segunda derivada de $x$
son 1 y 0, respectivamente. De manera similar, $D^3x^2=0$, etcétera.

El operador diferencial $D^n$ anula cada una de las funciones

$$
1,\quad x,\quad x^2,\quad\ldots,\quad x^{n-1}. \tag{3}
$$

## Página 151

Como una consecuencia inmediata de (3) y el hecho de que la derivación se puede
hacer término a término, un polinomio

$$
c_0+c_1x+c_2x^2+\cdots+c_{n-1}x^{n-1} \tag{4}
$$

se anula al encontrar un operador que aniquile la potencia más alta de $x$.

Las funciones que se anulan por un operador diferencial lineal de $n$-ésimo
orden $L$ son simplemente aquellas funciones que se obtienen de la solución
general de la ecuación diferencial homogénea $L(y)=0$.

El operador diferencial $(D-\alpha)^n$ anula cada una de las funciones

$$
e^{\alpha x},\quad xe^{\alpha x},\quad x^2e^{\alpha x},
\quad\ldots,\quad x^{n-1}e^{\alpha x}. \tag{5}
$$

Para ver esto, observe que la ecuación auxiliar de la ecuación homogénea
$(D-\alpha)^ny=0$ es $(m-\alpha)^n=0$. Puesto que $\alpha$ es una raíz de
multiplicidad $n$, la solución general es

$$
y=c_1e^{\alpha x}+c_2xe^{\alpha x}+\cdots+c_nx^{n-1}e^{\alpha x}. \tag{6}
$$

### Ejemplo 1. Operadores anuladores

Encuentre un operador diferencial que anule la función dada.

a) $1-5x^2+8x^3$; b) $e^{-3x}$; c) $4e^{2x}-10xe^{2x}$

**Solución.** a) De (3) se sabe que $D^4x^3=0$, así de (4) se tiene que

$$
D^4(1-5x^2+8x^3)=0.
$$

b) De (5), con $\alpha=-3$ y $n=1$, vemos que

$$
(D+3)e^{-3x}=0.
$$

c) De (5) y (6), con $\alpha=2$ y $n=2$, se tiene que

$$
(D-2)^2(4e^{2x}-10xe^{2x})=0.
$$

Cuando $\alpha$ y $\beta$, $\beta>0$ son números reales, la fórmula cuadrática
revela que $[m^2-2\alpha m+(\alpha^2+\beta^2)]^n=0$ tiene raíces complejas
$\alpha+i\beta$, $\alpha-i\beta$, ambas de multiplicidad $n$. Del análisis al
final de la sección 4.3, se tiene el siguiente resultado.

El operador diferencial $[D^2-2\alpha D+(\alpha^2+\beta^2)]^n$ anula cada una de
las funciones

$$
\begin{array}{lllll}
e^{\alpha x}\cos\beta x,&xe^{\alpha x}\cos\beta x,&x^2e^{\alpha x}\cos\beta x,
&\ldots,&x^{n-1}e^{\alpha x}\cos\beta x,\\
e^{\alpha x}\mathop{\mathrm{sen}}\nolimits \beta x,&xe^{\alpha x}\mathop{\mathrm{sen}}\nolimits \beta x,
&x^2e^{\alpha x}\mathop{\mathrm{sen}}\nolimits \beta x,&\ldots,
&x^{n-1}e^{\alpha x}\mathop{\mathrm{sen}}\nolimits \beta x.
\end{array} \tag{7}
$$

### Ejemplo 2. Operador anulador

Encuentre un operador diferencial que anule
$5e^{-x}\cos2x-9e^{-x}\mathop{\mathrm{sen}}\nolimits 2x$.

**Solución.** La inspección de las funciones $e^{-x}\cos2x$ y
$e^{-x}\mathop{\mathrm{sen}}\nolimits 2x$ muestra que $\alpha=-1$ y $\beta=2$.
Por tanto, de la ecuación (7) se concluye que $D^2+2D+5$ anulará *cualquier*
función que sea combinación lineal de estas funciones tales como
$5e^{-x}\cos2x-9e^{-x}\mathop{\mathrm{sen}}\nolimits 2x$.

## Página 152

Cuando $\alpha=0$ y $n=1$, un caso especial de (7) es

$$
(D^2+\beta^2)\left\{\begin{array}{l}\cos\beta x\\\mathop{\mathrm{sen}}\nolimits \beta x\end{array}\right.=0.
\tag{8}
$$

Por ejemplo $D^2+16$ anulará cualquier combinación lineal de
$\mathop{\mathrm{sen}}\nolimits 4x$ y $\cos4x$.

Con frecuencia estamos interesados en anular la suma de dos o más funciones.
Como acabamos de ver en los ejemplos 1 y 2, si $L$ es un operador diferencial
lineal tal que $L(y_1)=0$ y $L(y_2)=0$, entonces $L$ anulará la combinación
lineal $c_1y_1(x)+c_2y_2(x)$. Esta es una consecuencia directa del teorema
4.1.2. Supongamos ahora que $L_1$ y $L_2$ son operadores diferenciales lineales
con coeficientes constantes tales que $L_1$ anula a $y_1(x)$ y $L_2$ anula a
$y_2(x)$, pero $L_1(y_2)\ne0$ y $L_2(y_1)\ne0$. Entonces el *producto* de los
operadores diferenciales $L_1L_2$ anula la suma $c_1y_1(x)+c_2y_2(x)$. Esto se
puede demostrar fácilmente, usando la linealidad y el hecho de que
$L_1L_2=L_2L_1$:

$$
\begin{aligned}
L_1L_2(y_1+y_2)&=L_1L_2(y_1)+L_1L_2(y_2)\\
&=L_2L_1(y_1)+L_1L_2(y_2)\\
&=L_2[\underbrace{L_1(y_1)}_{\text{cero}}]+
L_1[\underbrace{L_2(y_2)}_{\text{cero}}]=0.
\end{aligned}
$$

Por ejemplo, sabemos de (3) que $D^2$ anula a $7-x$ y de (8) que $D^2+16$ anula
a $\mathop{\mathrm{sen}}\nolimits 4x$. Por tanto el producto de operadores
$D^2(D^2+16)$ anulará la combinación lineal
$7-x+6\mathop{\mathrm{sen}}\nolimits 4x$.

**Nota.** El operador diferencial que anula una función no es único. Vimos en el
inciso b) del ejemplo 1 que $D+3$ anula a $e^{-3x}$, pero también a los
operadores diferenciales de orden superior siempre y cuando $D+3$ sea uno de los
factores del operador. Por ejemplo $(D+3)(D+1)$, $(D+3)^2$ y $D^3(D+3)$ todos
anulan a $e^{-3x}$. (Compruebe esto.) Como algo natural, cuando se busca un
anulador diferencial para una función $y=f(x)$, se quiere que el operador de
*mínimo orden posible* haga el trabajo.

### Coeficientes indeterminados

Lo anterior lleva al punto del análisis previo. Suponga que $L(y)=g(x)$ es una
ecuación diferencial lineal con coeficientes constantes y que la entrada $g(x)$
consiste en sumas y productos finitos de las funciones listadas en (3), (5) y
(7), es decir, $g(x)$ es una combinación lineal de funciones de la forma

$$
k\ (\text{constante}),\quad x^m,\quad x^me^{\alpha x},\quad
x^me^{\alpha x}\cos\beta x,\quad\text{y}\quad
x^me^{\alpha x}\mathop{\mathrm{sen}}\nolimits \beta x,
$$

donde $m$ es un entero no negativo y $\alpha$ y $\beta$ son números reales.
Ahora se sabe que una función tal como $g(x)$ puede ser anulada por un operador
diferencial $L_1$ de menor orden, que es producto de los operadores $D^n$,
$(D-\alpha)^n$ y $(D^2-2\alpha D+\alpha^2+\beta^2)^n$. Al aplicar $L_1$ a ambos
lados de la ecuación $L(y)=g(x)$ se obtiene $L_1L(y)=L_1(g(x))=0$. Al resolver
la ecuación *homogénea de orden superior* $L_1L(y)=0$, se descubre la *forma* de
una solución particular $y_p$ para la ecuación original *no homogénea*
$L(y)=g(x)$. Entonces sustituimos esta forma supuesta en $L(y)=g(x)$ para
encontrar una solución particular explícita. Este procedimiento para determinar
$y_p$, llamado **método de los coeficientes indeterminados**, se ilustra a
continuación en varios ejemplos.

Antes de proceder, recuerde que la solución general de una ecuación diferencial
lineal no homogénea $L(y)=g(x)$ es $y=y_c+y_p$ donde $y_c$ es la función
complementaria, es decir, la solución general de la ecuación homogénea asociada
$L(y)=0$. La solución general de cada ecuación $L(y)=g(x)$ se define en el
intervalo $(-\infty,\infty)$.

## Página 153

### Ejemplo 3. Solución general usando coeficientes indeterminados

Resuelva

$$
y''+3y'+2y=4x^2. \tag{9}
$$

**Solución. Paso 1.** Primero, resolvemos la ecuación homogénea $y''+3y'+2y=0$.
Entonces, de la ecuación auxiliar $m^2+3m+2=(m+1)(m+2)=0$ se encuentra $m_1=-1$
y $m_2=-2$ y así, la función complementaria es

$$
y_c=c_1e^{-x}+c_2e^{-2x}.
$$

**Paso 2.** Ahora, puesto que $4x^2$ se anula con el operador diferencial $D^3$,
se ve que $D^3(D^2+3D+2)y=4D^3x^2$ es lo mismo que

$$
D^3(D^2+3D+2)y=0. \tag{10}
$$

La ecuación auxiliar de la ecuación de quinto orden en (10),

$$
m^3(m^2+3m+2)=0\quad\text{o}\quad m^3(m+1)(m+2)=0,
$$

tiene raíces $m_1=m_2=m_3=0$, $m_4=-1$, y $m_5=-2$. Así que su solución general
debe ser

$$
y=c_1+c_2x+c_3x^2+\boxed{c_4e^{-x}+c_5e^{-2x}}. \tag{11}
$$

Los términos del cuadro sombreado en (11) constituyen la función complementaria
de la ecuación original (9). Se puede argumentar que una solución particular
$y_p$, de (9) también debe satisfacer la ecuación (10). Esto significa que los
términos restantes en (11) deben tener la forma básica de $y_p$:

$$
y_p=A+Bx+Cx^2, \tag{12}
$$

donde, por conveniencia, hemos remplazado $c_1$, $c_2$ y $c_3$ por $A$, $B$ y
$C$, respectivamente. Para que (12) sea una solución particular de (9), es
necesario encontrar coeficientes específicos $A$, $B$ y $C$. Derivando la
ecuación (12), se tiene que

$$
y_p'=B+2Cx,\qquad y_p''=2C,
$$

y sustituyendo esto en la ecuación (9) se obtiene

$$
y_p''+3y_p'+2y_p=2C+3B+6Cx+2A+2Bx+2Cx^2=4x^2.
$$

Como se supone que la última ecuación es una identidad los coeficientes de
potencias semejantes de $x$ deben ser iguales:

$$
\boxed{2C}x^2+\boxed{2B+6C}x+\boxed{2A+3B+2C}=4x^2+0x+0.
$$

*Igual:* $2C$ con $4$; $2B+6C$ con $0$; $2A+3B+2C$ con $0$.

Es decir

$$
2C=4,\qquad 2B+6C=0,\qquad 2A+3B+2C=0. \tag{13}
$$

Resolviendo las ecuaciones de (13) se obtiene $A=7$, $B=-6$ y $C=2$. Por tanto
$y_p=7-6x+2x^2$.

**Paso 3.** La solución general de la ecuación en (9) es $y=y_c+y_p$ o

$$
y=c_1e^{-x}+c_2e^{-2x}+7-6x+2x^2.
$$

## Página 154

### Ejemplo 4. Solución general usando coeficientes indeterminados

Resuelva

$$
y''-3y'=8e^{3x}+4\mathop{\mathrm{sen}}\nolimits x. \tag{14}
$$

**Solución. Paso 1.** La ecuación auxiliar para la ecuación homogénea asociada
$y''-3y'=0$ es $m^2-3m=m(m-3)=0$, y por tanto, $y_c=c_1+c_2e^{3x}$.

**Paso 2.** Ahora, puesto que $(D-3)e^{3x}=0$ y
$(D^2+1)\mathop{\mathrm{sen}}\nolimits x=0$, se aplica el operador diferencial
$(D-3)(D^2+1)$ a ambos lados de la ecuación (14):

$$
(D-3)(D^2+1)(D^2-3D)y=0. \tag{15}
$$

La ecuación auxiliar de (15) es:

$$
(m-3)(m^2+1)(m^2-3m)=0\quad\text{o}\quad m(m-3)^2(m^2+1)=0.
$$

Así

$$
y=\boxed{c_1+c_2e^{3x}}+c_3xe^{3x}+c_4\cos x+c_5\mathop{\mathrm{sen}}\nolimits x.
$$

Una vez que se excluye la combinación lineal de términos dentro del cuadro que
corresponde a $y_c$ se obtiene la forma de $y_p$:

$$
y_p=Axe^{3x}+B\cos x+C\mathop{\mathrm{sen}}\nolimits x.
$$

Sustituyendo $y_p$ en (14) y simplificando, se obtiene

$$
y_p''-3y_p'=3Ae^{3x}+(-B-3C)\cos x+(3B-C)\mathop{\mathrm{sen}}\nolimits x
=8e^{3x}+4\mathop{\mathrm{sen}}\nolimits x.
$$

Igualando los coeficientes se obtiene que $3A=8$, $-B-3C=0$ y $3B-C=4$. Se
encuentra que $A=\frac83$, $B=\frac65$, y $C=-\frac25$ y por tanto,

$$
y_p=\frac83xe^{3x}+\frac65\cos x-\frac25\mathop{\mathrm{sen}}\nolimits x.
$$

**Paso 3.** Entonces la solución general de (14) es

$$
y=c_1+c_2e^{3x}+\frac83xe^{3x}+\frac65\cos x-\frac25\mathop{\mathrm{sen}}\nolimits x.
$$

### Ejemplo 5. Solución general usando coeficientes indeterminados

Resuelva

$$
y''+y=x\cos x-\cos x. \tag{16}
$$

**Solución.** La función complementaria es
$y_c=c_1\cos x+c_2\mathop{\mathrm{sen}}\nolimits x$. Ahora al comparar $\cos x$
y $x\cos x$ con las funciones del primer renglón de (7), vemos que $\alpha=0$ y
$n=1$ y así $(D^2+1)^2$ es un anulador para el miembro derecho de la ecuación en
(16). Aplicando este operador a la ecuación diferencial se obtiene

$$
(D^2+1)^2(D^2+1)y=0\quad\text{o}\quad(D^2+1)^3y=0.
$$

Puesto que $i$ y $-i$ son raíces complejas de multiplicidad 3 de la última
ecuación auxiliar, se concluye que

$$
y=\boxed{c_1\cos x+c_2\mathop{\mathrm{sen}}\nolimits x}
+c_3x\cos x+c_4x\mathop{\mathrm{sen}}\nolimits x+c_5x^2\cos x+c_6x^2\mathop{\mathrm{sen}}\nolimits x.
$$

Sustituyendo

$$
y_p=Ax\cos x+Bx\mathop{\mathrm{sen}}\nolimits x+Cx^2\cos x+Ex^2\mathop{\mathrm{sen}}\nolimits x
$$

en (16) y simplificando:

$$
\begin{aligned}
y_p''+y_p&=4Ex\cos x-4Cx\mathop{\mathrm{sen}}\nolimits x+(2B+2C)\cos x
+(-2A+2E)\mathop{\mathrm{sen}}\nolimits x\\
&=x\cos x-\cos x.
\end{aligned}
$$

## Página 155

Igualando los coeficientes se obtienen las ecuaciones $4E=1$, $-4C=0$,
$2B+2C=-1$, y $-2A+2E=0$, de las que encontramos $A=\frac14$, $B=-\frac12$,
$C=0$ y $E=\frac14$. Por tanto la solución general de (16) es

$$
y=c_1\cos x+c_2\mathop{\mathrm{sen}}\nolimits x+\frac14x\cos x
-\frac12x\mathop{\mathrm{sen}}\nolimits x+\frac14x^2\mathop{\mathrm{sen}}\nolimits x.
$$

### Ejemplo 6. Forma de una solución particular

Determine la forma de una solución particular para

$$
y''-2y'+y=10e^{-2x}\cos x. \tag{17}
$$

**Solución.** La función complementaria de la ecuación dada es
$y_c=c_1e^x+c_2xe^x$.

Ahora de (7), con $\alpha=-2$, $\beta=1$ y $n=1$, se sabe que

$$
(D^2+4D+5)e^{-2x}\cos x=0.
$$

Aplicando el operador $D^2+4D+5$ a (17), se obtiene

$$
(D^2+4D+5)(D^2-2D+1)y=0. \tag{18}
$$

Puesto que las raíces de la ecuación auxiliar de (18) son $-2-i$, $-2+i$, 1 y 1,
vemos de

$$
y=\boxed{c_1e^x+c_2xe^x}+c_3e^{-2x}\cos x+c_4e^{-2x}\mathop{\mathrm{sen}}\nolimits x
$$

que una solución particular de (17) se puede encontrar con la forma

$$
y_p=Ae^{-2x}\cos x+Be^{-2x}\mathop{\mathrm{sen}}\nolimits x.
$$

### Ejemplo 7. Forma de una solución particular

Determine la forma de una solución particular para

$$
y'''-4y''+4y'=5x^2-6x+4x^2e^{2x}+3e^{5x}. \tag{19}
$$

**Solución.** Observe que

$$
D^3(5x^2-6x)=0,\quad (D-2)^3x^2e^{2x}=0
\quad\text{y}\quad(D-5)e^{5x}=0.
$$

Por tanto, $D^3(D-2)^3(D-5)$ aplicado a (19), se obtiene

$$
D^3(D-2)^3(D-5)(D^3-4D^2+4D)y=0
$$

o

$$
D^4(D-2)^5(D-5)y=0.
$$

Las raíces de la ecuación auxiliar para la última ecuación diferencial son 0, 0,
0, 0, 2, 2, 2, 2, 2 y 5. Por tanto,

$$
y=\boxed{c_1}+c_2x+c_3x^2+c_4x^3+\boxed{c_5e^{2x}+c_6xe^{2x}}
+c_7x^2e^{2x}+c_8x^3e^{2x}+c_9x^4e^{2x}+c_{10}e^{5x}. \tag{20}
$$

Debido a que la combinación lineal $c_1+c_5e^{2x}+c_6xe^{2x}$ corresponde a la
función complementaria de (19), los términos restantes en (20) dan la forma de
una solución particular de la ecuación diferencial:

$$
y_p=Ax+Bx^2+Cx^3+Ex^2e^{2x}+Fx^3e^{2x}+Gx^4e^{2x}+He^{5x}.
$$

### Resumen del método

Por conveniencia se resume el método de coeficientes indeterminados como sigue.

## Página 156

### Coeficientes indeterminados: método del anulador

La ecuación diferencial $L(y)=g(x)$ tiene coeficientes constantes y la función
$g(x)$ consiste en sumas y productos finitos de constantes, polinomios,
funciones exponenciales $e^{ax}$, senos y cosenos.

i) Encuentre la función complementaria $y_c$ para la ecuación homogénea
$L(y)=0$.

ii) Opere ambos lados de la ecuación no homogénea $L(y)=g(x)$ con un operador
diferencial $L_1$ que anula la función $g(x)$.

iii) Determine la solución general de la ecuación diferencial homogénea de orden
superior $L_1L(y)=0$.

iv) Elimine de la solución del paso iii) los términos que se duplican en la
solución complementaria $y_c$ encontrada en el paso i). Forme una combinación
lineal $y_p$ de los términos restantes. Esta es la forma de una solución
particular de $L(y)=g(x)$.

v) Sustituya $y_p$ encontrada en el paso iv) en $L(y)=g(x)$. Iguale los
coeficientes de las distintas funciones en cada lado de la igualdad y resuelva
el sistema resultante de ecuaciones para determinar los coeficientes
desconocidos de $y_p$.

vi) Con la solución particular encontrada en el paso v), forme la solución
general $y=y_c+y_p$ de la ecuación diferencial dada.

### Comentarios

El método de coeficientes indeterminados no es aplicable a ecuaciones
diferenciales lineales con coeficientes variables ni tampoco es aplicable a
ecuaciones lineales con coeficientes constantes cuando $g(x)$ es una función tal
que

$$
g(x)=\ln x,\quad g(x)=\frac1x,\quad g(x)=\tan x,\quad
g(x)=\mathop{\mathrm{sen}}\nolimits ^{-1}x,
$$

etcétera. Las ecuaciones diferenciales en las que la entrada $g(x)$ es una
función de esta última clase se consideran en la siguiente sección.

### Ejercicios 4.5

*Las respuestas a los problemas con número impar comienzan en la página RES-5.*

En los problemas 1 a 10 escriba la ecuación diferencial en la forma $L(y)=g(x)$,
donde $L$ es un operador diferencial lineal con coeficientes constantes. Si es
posible, factorice $L$.

1. $9y''-4y=\mathop{\mathrm{sen}}\nolimits x$
1. $y''-5y=x^2-2x$
1. $y''-4y'-12y=x-6$
1. $2y''-3y'-2y=1$
1. $y'''+10y''+25y'=e^x$
1. $y'''+4y'=e^x\cos2x$
1. $y'''+2y''-13y'+10y=xe^{-x}$
1. $y'''+4y''+3y'=x^2\cos x-3x$
1. $y^{(4)}+8y'=4$
1. $y^{(4)}-8y''+16y=(x^3-2x)e^{4x}$

En los problemas 11 a 14 compruebe que el operador diferencial anula las
funciones indicadas.

11. $D^4;\quad y=10x^3-2x$
01. $2D-1;\quad y=4e^{x/2}$
01. $(D-2)(D+5);\quad y=e^{2x}+3e^{-5x}$
01. $D^2+64;\quad y=2\cos8x-5\mathop{\mathrm{sen}}\nolimits 8x$

En los problemas 15 a 26 determine el operador diferencial lineal que anula la
función dada.

15. $1+6x-2x^3$
01. $x^3(1-5x)$
01. $1+7e^{2x}$
01. $x+3xe^{6x}$
01. $\cos2x$
01. $1+\mathop{\mathrm{sen}}\nolimits x$
01. $13x+9x^2-\mathop{\mathrm{sen}}\nolimits 4x$
01. $8x-\mathop{\mathrm{sen}}\nolimits x+10\cos5x$
01. $e^{-x}+2xe^x-x^2e^x$
01. $(2-e^x)^2$
01. $3+e^x\cos2x$
01. $e^{-x}\mathop{\mathrm{sen}}\nolimits x-e^{2x}\cos x$

## Página 157 (fin de ejercicios 4.5)

En los problemas 27 a 34 determine las funciones linealmente independientes que
anulan el operador diferencial dado.

27. $D^5$
01. $D^2+4D$
01. $(D-6)(2D+3)$
01. $D^2-9D-36$
01. $D^2+5$
01. $D^2-6D+10$
01. $D^3-10D^2+25D$
01. $D^2(D-5)(D-7)$

En los problemas 35 a 64 resuelva la ecuación diferencial dada usando
coeficientes indeterminados.

35. $y''-9y=54$
01. $2y''-7y'+5y=-29$
01. $y''+y'=3$
01. $y'''+2y''+y'=10$
01. $y''+4y'+4y=2x+6$
01. $y''+3y'=4x-5$
01. $y'''+y''=8x^2$
01. $y''-2y'+y=x^3+4x$
01. $y''-y'-12y=e^{4x}$
01. $y''+2y'+2y=5e^{6x}$
01. $y''-2y'-3y=4e^x-9$
01. $y''+6y'+8y=3e^{-2x}+2x$
01. $y''+25y=6\mathop{\mathrm{sen}}\nolimits x$
01. $y''+4y=4\cos x+3\mathop{\mathrm{sen}}\nolimits x-8$
01. $y''+6y'+9y=-xe^{4x}$
01. $y''+3y'-10y=x(e^x+1)$
01. $y''-y=x^2e^x+5$
01. $y''+2y'+y=x^2e^{-x}$
01. $y''-2y'+5y=e^x\mathop{\mathrm{sen}}\nolimits x$
01. $y''+y'+\frac14y=e^x(\mathop{\mathrm{sen}}\nolimits 3x-\cos3x)$
01. $y''+25y=20\mathop{\mathrm{sen}}\nolimits 5x$
01. $y''+y=4\cos x-\mathop{\mathrm{sen}}\nolimits x$
01. $y''+y'+y=x\mathop{\mathrm{sen}}\nolimits x$
01. $y''+4y=\cos^2x$
01. $y'''+8y''=-6x^2+9x+2$
01. $y'''-y''+y'-y=xe^x-e^{-x}+7$
01. $y'''-3y''+3y'-y=e^x-x+16$
01. $2y'''-3y''-3y'+2y=(e^x+e^{-x})^2$
01. $y^{(4)}-2y'''+y''=e^x+1$
01. $y^{(4)}-4y''=5x^2-e^{2x}$

En los problemas 65 a 72 resuelva el problema con valores iniciales.

65. $y''-64y=16,\quad y(0)=1,\ y'(0)=0$
01. $y''+y'=x,\quad y(0)=1,\ y'(0)=0$
01. $y''-5y'=x-2,\quad y(0),\ y'(0)=2$
01. $y''+5y'-6y=10e^{2x},\quad y(0)=1,\ y'(0)=1$
01. $y''+y=8\cos2x-4\mathop{\mathrm{sen}}\nolimits x,\quad y(\pi/2)=-1,\ y'(\pi/2)=0$
01. $y'''-2y''+y'=xe^x+5,\quad y(0)=2,\ y'(0)=2,\ y''(0)=-1$
01. $y''-4y'+8y=x^3,\quad y(0)=2,\ y'(0)=4$
01. $y^{(4)}-y'''=x+e^x,\quad y(0)=0,\ y'(0)=0,\ y''(0)=0,\ y'''(0)=0$

### Problemas para analizar

73. Suponga que $L$ es un operador diferencial lineal que se factoriza pero que
    tiene coeficientes variables. ¿Conmutan los factores de $L$? Defienda su
    respuesta.

## Notas de transcripción

Se conserva el $n=1$ impreso en el ejemplo 5 (página 154), aunque allí se usa el
anulador al cuadrado. En el ejercicio 67 el original imprime solamente $y(0)$,
sin igualdad ni valor; no se completa el dato. Se conserva la redacción
“funciones […] que anulan el operador” de los ejercicios 27–34 y “pero también a
los operadores” de la nota de la página 152.
