# Series de Fourier — Conceptos previos

Fuente: «Apunte de Clases del Ing. Urrutia.pdf», carpeta de 2020. Esta parte
transcribe páginas PDF 1–16 (portada y hojas impresas 1–15).
[Procedencia y cobertura](../../../resources/2020/pdf2020-fourier-urrutia-cobertura.md).

## Página PDF 1 — Portada

UNIVERSIDAD TECNOLÓGICA NACIONAL

FACULTAD REGIONAL RESISTENCIA

ANÁLISIS MATEMÁTICO II

SERIES DE FOURIER

Apunte de clase del Ing. Leopoldo S. de Urrutia

## Página PDF 2 — Hoja N° 1

UNIVERSIDAD TECNOLÓGICA NACIONAL

FACULTAD REGIONAL RESISTENCIA

### Serie de Fourier

### Conceptos previos

Iniciaremos este capítulo con la revisión de algunos conceptos elementales que
serán de aplicación en los desarrollos posteriores.

### I.- Funciones Pares e Impares

**1.** Una función de variable “x”, $f(x)$ es **par** si $\forall x$, se
verifica la igualdad:

$$
f(-x)=f(+x)=f(x)
$$

son funciones pares, entre otras las siguientes:

a) $f(x)=\cos nx$;

b) $f(x)=x^n$ para n entero y par;

c) $f(x)=K$ (constante)

como consecuencia inmediata de la definición podemos observar que para todo par
de puntos simétricos al origen “-$x_{0}$”; “$x_{0}$”, pertenecientes a su
dominio, la función toma los mismos valores numéricos y por lo tanto “su gráfica
es simétrica respecto al eje de ordenadas”.

![Gráfica par: valores iguales en menos x0 y x0](../../../resources/2020/pdf2020-fourier-urrutia/p02-par.png)

## Página PDF 3 — Hoja N° 2

### Propiedades de las Funciones Pares

Sean $f(x)$ y $g(x)$ dos funciones pares, $U(x)$=$f(x)$+$g(x)$ y
$V(x)$=$f(x)$.$g(x)$ demostraremos que:

**2.** La suma de dos funciones pares es otra función par. En efecto:

$$
U(-x)=f(-x)+g(-x)=f(x)+g(x)=U(x),
$$

por lo tanto se cumple que:

$$
U(-x)=U(x)
$$

**3.** El producto o cociente de dos funciones pares es otra función par.

$$
V(x)=f(x)\cdot g(x)=f(-x)\cdot g(-x)=V(-x),
$$

por lo tanto se cumple que:

$$
V(-x)=V(x)
$$

**4.** Si $f(x)$ es par entonces:

$$
\int_{-a}^a f(x)\cdot dx=2\cdot\int_0^a f(x)\cdot dx
$$

esta propiedad de la integral definida de una función par, en intervalo de
integración simétrico respecto del origen es evidente, si se tiene en cuenta la
simetría de representación abordada anteriormente, y el valor de la integral
como área.

![Áreas iguales de una función par](../../../resources/2020/pdf2020-fourier-urrutia/p03-integral-par.png)

## Página PDF 4 — Hoja N° 3

**5.** Una función de variable independiente x, $f(x)$ es “impar”, si se
verifica que:

$$
f(-x)=-f(x)\qquad\forall x,
$$

son funciones impares las siguientes:

a) $f(x)=\operatorname{sen}x$

b) $f(x)=\operatorname{tg}x$

c) $f(x)=x^n$ si n es entero e impar.

Sean $f(x)$ y $g(x)$ funciones impares y $U(x)$=$f(x)$+$g(x)$,
$V(x)$=$f(x)$.$g(x)$.

**6.** La suma de dos funciones impares es otra función impar. En efecto:

$$
U(-x)=f(-x)+g(-x)=-f(x)-g(x)=-(f(x)+g(x))=-U(x)
$$

por lo tanto $U(-x)=-U(x)$

**7.** El producto o cociente de dos funciones impares es una función “Par”.

$$
V(-x)=f(-x)\cdot g(-x)=[-f(x)]\cdot[-g(x)]=f(x)\cdot g(x)=V(x)
$$

por lo tanto:

$$
V(-x)=V(x)
$$

**8.** El producto o cociente de una función PAR y otra IMPAR da como resultado
otra función IMPAR. Supongamos dos funciones:

$f(x)=f(-x)$ función par y $g(-x)=-g(x)$ una función impar,

entonces $V(x)=f(x)\cdot g(x)$ resulta:

$$
V(-x)=f(-x)\cdot g(-x)=f(x)\cdot(-g(x))=-(f(x)\cdot g(x))=-V(x)
$$

por lo tanto $V(x)$ es impar.

**9.** Dado que una función impar toma valores numéricos opuestos para valores
opuestos de la variable independiente, su gráfica es una curva simétrica
respecto al punto de origen. Ejemplo:

$$
f(x)=x^3
$$

**10.** Como consecuencia de la propiedad de simetría geomé-

## Página PDF 5 — Hoja N° 4

trica expresada en el punto anterior resulta evidente que toda integral definida
de una función impar en un intervalo de integración simétrico respecto del
origen es nula, por lo tanto

$$
\int_{-a}^a f(x)\cdot dx=0,\quad\text{si }f(x)\text{ es una función impar.}
$$

## Página PDF 6 — Hoja N° 5

### II.- Funciones Periódicas

**1.** Se dice que una función y=$f(x)$ es periódica y que su período es “p”, si
se cumple que:

$$
f(x+p)=f(x),\quad\forall x\in\mathbb R,
$$

un ejemplo son las funciones trigonométricas, ya que:

$$
\operatorname{sen}(x+2\pi)=\operatorname{sen}x;\quad
\cos(x+2\pi)=\cos x,\quad\operatorname{tg}(x+\pi)=\operatorname{tg}x
$$

en los dos primeros casos el período es $2\pi$ y en el tercero es $\pi$. Como
consecuencia inmediata de la definición observamos que la gráfica de una función
periódica se repite en intervalos consecutivos cuya amplitud es “p”.
Representamos la función de período $2\pi$ definida por:

$$
f(x)=\begin{cases}x&\text{si }0<x<\pi\\\pi&\text{si }\pi<x<2\pi\end{cases}
$$

![Función periódica por tramos](../../../resources/2020/pdf2020-fourier-urrutia/p06-tramos.png)

### Propiedades de las funciones periódicas

**2.** Si $f(x+p)=f(x)\;\forall x\in\mathbb R$ y n es un número entero ≠0 será
$f(x+np)=f(x)$, de modo que “cualquier múltiplo entero del período, también es
período de la misma función”. El período “p de menor valor”, se denomina
“período primitivo de la función”. Hemos visto en el punto anterior que
$\operatorname{tg}(x)=\operatorname{tg}(x+\pi)$, son también períodos de la
función tangente, $\pm2\pi$, $\pm3\pi$, $\pm4\pi$, etc., pero el período
primitivo de la función es $p=\pi$.

**3.** Si $f(x)$ es una función periódica de período p, f(ax) es otra función
periódica de período p/a $\forall a>0$. Para su demostración reemplacemos en la
función f(ax), a la variable (x) por el valor (x+p/a).

## Página PDF 7 — Hoja N° 6

$f(a(x+p/a))=f(ax+p)$ como $f(x+p)=f(x)\;\forall x$ incluso (x.a)

$f(a(x+p/a))=f(ax)$ con lo cual queda demostrado su período p/a.

Como aplicación de esta propiedad observamos que siendo el período de
$f(x)=\operatorname{sen}x;\;p=2\pi$, por lo tanto el de la función
$f(x)=\operatorname{sen}nx$, será $p=2\pi/n$.

Así entonces, las gráficas correspondientes a: sen x, sen 2x, sen 3x,…, se
repiten 1, 2, 3,… veces el período $2\pi$, como se puede observar.

![sen x, sen 2x y sen 3x y sus períodos](../../../resources/2020/pdf2020-fourier-urrutia/p07-senos.png)

Lo mismo ocurre con las funciones cosenoidales para cos x, cos 2x, cos 3x, que
ya conocemos su gráfica.

**4.** Si $f(x)$ es una función periódica de período p y b≠0, entonces f(x/b) es
otra función periódica cuyo período es p.b. Lo demostraremos:

$$
f\left(\frac{x+p\cdot b}{b}\right)=f\left(\frac xb+p\right)\quad\text{pero}
$$

$$
f\left(\frac xb+p\right)=f\left(\frac xb\right)\quad\text{por ser }f(x+p)=f(x)\;\forall x
$$

## Página PDF 8 — Hoja N° 7

$$
f\left(\frac{x+p\cdot b}{b}\right)=f\left(\frac xb+p\right)\quad\text{pero}
$$

$$
f\left(\frac xb+p\right)=f\left(\frac xb\right)
$$

por ser $f(x+p)=f(x)\;\forall x$, entonces $f(\frac xb)$ es periódica de período
b.p.

**5.** La suma de funciones periódicas de igual período es otra función
periódica del mismo período.

sean $f(x)$ y $g(x)$ tales que:

$$
\begin{cases}f(x+p)=f(x)\\g(x+p)=g(x)\\h(x)=f(x)+g(x)\end{cases}\quad\forall x
$$

entonces se cumplirá:

$$
h(x+p)=f(x+p)+g(x+p)=f(x)+g(x)=h(x)
$$

por lo tanto $h(x+p)=h(x)$.

**6.** Supongamos la función:

$$
f(x)=2\cdot\operatorname{sen}x+\frac32\cdot\operatorname{sen}2x+\operatorname{sen}3x,
$$

es una función, suma de funciones periódicas; la primera de las cuales (sen x)
tiene por período $p=2\pi$ y la segunda (sen 2x) tiene un período primitivo
$p=\pi$ y la tercera $2\pi/3$; pero considerando la propiedad 2, ambas admiten
también $p=2\pi$.

En consecuencia $f(x)$ tiene por período $p=2\pi$.

Por ser de suma importancia para interpretar algunos de los desarrollos en serie
de Fourier construiremos su gráfica correspondiente. Para ello recordemos que en
la función y=A.sen x,

## Página PDF 9 — Hoja N° 8

el coeficiente A es la “amplitud” de la onda de modo que:

$$
-A\le f(x)\le A
$$

![Suma de 2 sen x, tres medios sen 2x y sen 3x](../../../resources/2020/pdf2020-fourier-urrutia/p09-suma-senos.png)

## Página PDF 10 — Hoja N° 9

### 7. Integrales Definidas de Funciones Periódicas

Sea $f(x)$ una función periódica de período P;
$f(x)=f(x+P)\;\forall x\in\mathbb R$. Si $f(x)$ es integrable en un intervalo de
amplitud igual al período P, entonces es integrable sobre cualquier intervalo
$\in\mathbb R$. Además se verifica que:

![Integración sobre un período con comienzo variable](../../../resources/2020/pdf2020-fourier-urrutia/p10-integral-periodica.png)

$\int_a^{a+P}f(x)dx$, es constante, cualquiera sea el valor de a y siempre que
la longitud del intervalo de integración sea P.

Demostración:

$$
\int_a^{a+P}f(x)dx=\int_0^P f(x)\cdot dx+\int_P^{a+P}f(x)\cdot dx-\int_0^a f(x)\cdot dx\tag{1}
$$

Analicemos la segunda integral, del segundo miembro:

$\int_P^{a+P}f(x)\cdot dx$; si hacemos $x=t+P\Rightarrow dx=dt$ además,

si $P=x\Rightarrow t=0$; si $x=a+P\Rightarrow t=a\;\therefore$ reemplazando

$\int_P^{a+P}f(x)\cdot dx=\int_0^a f(t+P)dt=\int_0^a f(x)\cdot dx$, reemplazando
en 1

$\int_a^{a+P}f(x)\cdot dx=\int_0^P f(x)\cdot dx+\int_0^a f(x)dx-\int_0^a f(x)dx$
por lo tanto

$$
\int_a^{a+P}f(x)\cdot dx=\int_0^P f(x)\cdot dx=\int_{-P/2}^{P/2}f(x)\cdot dx
$$

## Página PDF 11 — Hoja N° 10

### Fórmulas De Posterior Aplicación

Verificaremos las siguientes expresiones, donde m y n son números enteros.

### 1.-

$$
\int_{-\pi}^{\pi}\cos nx\cdot dx=0\;\therefore\;
\int_{-\pi}^{\pi}\cos nx\cdot dx=\frac1n\int_{-\pi}^{\pi}\cos(nx)\cdot d(nx)
=\left.\frac1n\operatorname{sen}nx\right|_{-\pi}^{\pi}=0
$$

**2.-** $\int_{-\pi}^{\pi}\operatorname{sen}nx\cdot dx=0$ es nula por ser “sen
nx” una función impar.

**3.-** $\int_{-\pi}^{\pi}\operatorname{sen}(mx)\cdot\cos(nx)\cdot dx=0$ por lo
tanto dado que se trata de un integrando producto de dos funciones una par (cos
nx) y una impar (sen mx), la resultante será otra función impar, como los
límites de integración son simétricos la integral es nula.

### 4.-

$$
\int_{-\pi}^{\pi}\operatorname{sen}(mx)\cdot\operatorname{sen}(nx)\cdot dx
=\begin{cases}0&\text{si }m\ne n\\\pi&\text{si }m=n\end{cases}
$$

a) primer caso si m≠n

$$
\int_{-\pi}^{\pi}\operatorname{sen}(mx)\cdot\operatorname{sen}(nx)\cdot dx
=\frac12\left[\frac{\operatorname{sen}(m-n)\cdot x}{m-n}
-\frac{\operatorname{sen}(m+n)\cdot x}{m+n}\right]_{x=-\pi}^{\pi}
$$

$$
=\frac12\left[\frac{\operatorname{sen}(m-n)\pi}{m+n}
-\frac{\operatorname{sen}(m+n)\pi}{m+n}\right]=0\quad\text{por ser }(m\pm n)\in\mathbb Z
$$

b) segundo caso si m=n

$$
\begin{aligned}
\int_{-\pi}^{\pi}\operatorname{sen}(mx)\cdot\operatorname{sen}(nx)\cdot dx
&=\int_{-\pi}^{\pi}\operatorname{sen}^2(mx)\cdot dx
=\frac1m\int_{-\pi}^{\pi}\operatorname{sen}^2(mx)\cdot d(mx)\\
&=\frac1{2\cdot m}[mx-\operatorname{sen}(mx)\cdot\cos(mx)]_{x=-\pi}^{\pi}\\
&=\frac1{2\cdot m}[m\pi-m(-\pi)]=\frac{2m\pi}{2m}=\pi
\end{aligned}
$$

### 5.-

$$
\int_{-\pi}^{\pi}\cos(mx)\cdot\cos(nx)\cdot dx
=\begin{cases}0&\text{si }m\ne n\\\pi&\text{si }m=n\end{cases}
$$

## Página PDF 12 — Hoja N° 11

a) primer caso si m≠n

$$
\int_{-\pi}^{\pi}\cos(mx)\cdot\cos(nx)\cdot dx
=\frac12\left[\frac{\operatorname{sen}(m-n)x}{m-n}
+\frac{\operatorname{sen}(m+n)x}{m+n}\right]_{x=-\pi}^{\pi}
=\frac{\operatorname{sen}(m-n)\cdot\pi}{m-n}+\frac{\operatorname{sen}(m+n)\pi}{m+n}
$$

por ser m±n∈Z, por lo tanto la integral es nula.

b) segundo caso si m=n

$$
\begin{aligned}
\int_{-\pi}^{\pi}\cos(mx)\cdot\cos(nx)\cdot dx
&=\int_{-\pi}^{\pi}\cos^2(mx)\cdot dx
=\frac1m\int_{-\pi}^{\pi}\cos^2(mx)\cdot d(mx)\\
&=\frac1{2\cdot m}[mx+\cos(mx)\cdot\operatorname{sen}(mx)]_{x=-\pi}^{\pi}\\
&=\frac1{2\cdot m}[m\pi-m(-\pi)]=\frac{2m\pi}{2m}=\pi
\end{aligned}
$$

### 6.-

$$
P(x)=\frac12+\sum_{K=1}^n\cos K\cdot x
=\frac{\operatorname{sen}(n+1/2)x}{2\cdot\operatorname{sen}x/2}
$$

Desarrollando:

$P(x)=\frac12+\cos x+\cos2x+\cos3x+\cdots+\cos nx$, por lo tanto

sabemos que $\cos\alpha=\frac{e^{i\alpha}+e^{-i\alpha}}2$; reemplazando en cada
término:

$$
\begin{aligned}
P(x)&=\frac12+\frac12(e^{ix}+e^{-ix})+\frac12(e^{i2x}+e^{-i2x})+\cdots+\frac12(e^{inx}+e^{-inx})\\
&=\frac12(e^{-inx}+\cdots+e^{-i2x}+e^{-ix}+1+e^{ix}+e^{i2x}+\cdots+e^{inx})
\end{aligned}
$$

sumando el segundo miembro, como los términos de una progresión geométrica, de
razón $q=e^{ix}$, cuyo número de términos es (2n+1) y el primer término es
$e^{-inx}$, resulta que:

## Página PDF 13 — Hoja N° 12

multiplicando numerador y denominador por una misma expresión $e^{-\frac12ix}$
obtenemos:

$$
P(x)=1/2\cdot\frac{e^{ix(n+1/2)}-e^{-ix(n+1/2)}}{e^{1/2ix}-e^{-1/2ix}}
$$

dividiendo y multiplicando por 2i tendremos:

$$
P(x)=1/2\cdot\frac{\frac{e^{ix(n+1/2)}-e^{-ix(n+1/2)}}{2i}}
{\frac{e^{1/2ix}-e^{-1/2ix}}{2i}}
=1/2\frac{\operatorname{sen}(n+1/2)\cdot x}{\operatorname{sen}(1/2\cdot x)}
$$

quedando así demostrada.

**7.** Si a la igualdad
$\frac12+\sum_{K=1}^n\cos Kx=\frac{\operatorname{sen}(n+1/2)\cdot x}{2\cdot\operatorname{sen}x/2}$
se la integra entre $-\pi$ y $\pi$.

$$
\frac12\int_{-\pi}^{\pi}dx+\sum_{K=1}^n\int_{-\pi}^{\pi}\cos Kx\cdot dx
=\int_{-\pi}^{\pi}\frac{\operatorname{sen}(n+1/2)\cdot x\,dx}{2\cdot\operatorname{sen}x/2}
$$

en el primer miembro tendremos:

$$
\frac12\left.x\right|_{-\pi}^{\pi}+\sum_{K=1}^n\left.\frac1K\cdot\operatorname{sen}Kx\right|_{-\pi}^{\pi}
=\frac12\cdot2\pi+\sum_{K=1}^n\frac2K\cdot\operatorname{sen}K\pi=\pi
$$

en consecuencia tendremos:

$$
\int_{-\pi}^{\pi}\frac{\operatorname{sen}(n+1/2)\cdot x}{2\cdot\operatorname{sen}x/2}dx=\pi
$$

De la misma manera que el caso 6, se demuestra:

$$
\sum_{K=1}^n\operatorname{sen}Kx
=\frac12\operatorname{cotg}x/2-\frac{\cos(n+1/2)x}{\operatorname{sen}x/2}
$$

## Página PDF 14 — Hoja N° 13

funciones continuas por tramos en [a,b], entonces se verificará que:

$$
\lim_{\lambda\to\infty}\int_a^b f(x)\cdot\operatorname{sen}\lambda x\cdot dx=0,
\quad\text{o bien que}\quad
\lim_{\lambda\to\infty}\int_a^b f(x)\cdot\cos\lambda x\cdot dx=0
$$

Demostración:

Supondremos primero que la función $f(x)$ es continua en (a,b). Llamemos:

$$
I(\lambda)=\int_a^b f(x)\cdot\operatorname{sen}\lambda x\cdot dx\tag{1}
$$

haciendo $x=t+\pi/\lambda$

$$
\begin{cases}
x=a\Rightarrow t=a-\pi/\lambda\;\wedge\;x=b\Rightarrow t=b-\pi/\lambda\\
f(x)=f(t+\pi/\lambda)\\
\operatorname{sen}\lambda x=\operatorname{sen}\lambda(t+\pi/\lambda)
=\operatorname{sen}(\lambda t+\pi)=-\operatorname{sen}\lambda t
\end{cases}
$$

por lo tanto:

$$
I(\lambda)=-\int_{a-\pi/\lambda}^{b-\pi/\lambda}f(t+\pi/\lambda)\cdot\operatorname{sen}\lambda t\cdot dt
=-\int_{a-\pi/\lambda}^{b-\pi/\lambda}f(x+\pi/\lambda)\cdot\operatorname{sen}\lambda x\cdot dx\tag{2}
$$

sumando las expresiones (1) y (2) tendremos:

$$
\begin{aligned}
2I(\lambda)&=-\int_{a-\pi/\lambda}^a f(x+\pi/\lambda)\cdot\operatorname{sen}\lambda x\cdot dx\\
&\quad+\int_a^{b-\pi/\lambda}[f(x)-f(x+\pi/\lambda)]\cdot\operatorname{sen}\lambda x\cdot dx
+\int_{b-\pi/\lambda}^b f(x)\cdot\operatorname{sen}\lambda x\cdot dx
\end{aligned}
$$

llamando M al máximo valor de la función $f(x)$ en (a,b);

$$
|f(x)|\le M\quad\forall x\in(a,b)
$$

y considerando que $|\operatorname{sen}\lambda x|\le1$, reemplazando resulta:

$$
2|I(\lambda)|\le M\int_{a-\pi/\lambda}^a dx
+\int_a^{b-\pi/\lambda}|f(x)-f(x+\pi/\lambda)|dx+M\int_{b-\pi/\lambda}^b dx
$$

$$
2|I(\lambda)|\le2M\pi/\lambda+\int_a^{b-\pi/\lambda}|f(x)-f(x+\pi/\lambda)|dx\;\therefore
$$

## Página PDF 15 — Hoja N° 14

para $\lambda>K_2$ es $|f(x)-f(x+\pi/\lambda)|<\frac\xi{b-a}$ por ser $f(x)$
continua en (a,b)

$$
\int_a^{b-\pi/\lambda}|f(x)-f(x+\pi/\lambda)|\cdot dx
<\frac\xi{b-a}\int_a^{b-\pi/\lambda}dx
=\frac\xi{b-a}(b-a-\pi/\lambda)<\xi
$$

en consecuencia:

$$
2|I(\lambda)|<2M\cdot\frac\xi{2M}+\xi\Rightarrow|I(\lambda)|<\xi;
\quad\forall\lambda>i\lambda\;(i\lambda=\operatorname{máx}K_1,K_2)
$$

Este teorema puede extenderse a funciones seccionalmente continuas en un
intervalo (a,b), es decir a funciones que tengan un número finito de
discontinuidades finitas en (a,b). Ejemplo de función seccionalmente continua:

![Función con discontinuidades en c y d](../../../resources/2020/pdf2020-fourier-urrutia/p15-seccional.png)

Bastará para demostrarlo, efectuar una partición del intervalo (a,b) en cada uno
de los puntos de discontinuidad y verificar que el teorema se cumple en cada uno
de los subintervalos resultantes de la partición practicada.

Además si tenemos en cuenta que:

$$
\cos(\alpha x+\beta)=\operatorname{sen}(\alpha x+\beta+\pi/2)
$$

## Página PDF 16 — Hoja N° 15

en consecuencia:

$$
\lim_{\alpha\to\infty}\int_a^b f(x)\cdot\cos(\alpha x+\beta)dx=0
\quad\text{si hacemos }\beta=0
$$

obtendremos:

$$
\lim_{\alpha\to\infty}\int_a^b f(x)\cdot\operatorname{sen}\alpha x\cdot dx=0
\quad\wedge\quad
\lim_{\alpha\to\infty}\int_a^b f(x)\cdot\cos\alpha x\cdot dx=0
$$

donde $f(x)$ es una función que cumple las condiciones expresadas en el teorema.
