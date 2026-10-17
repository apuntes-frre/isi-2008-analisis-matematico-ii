# Multiplicadores de Lagrange

Fuente: `Teórico Multiplicadores de Lagrange.pdf`, páginas 1–2.
[Procedencia](../../../resources/2016/fuentes.md).

Muchos problemas de optimización están sometidos a restricciones o ligaduras
para los valores que pueden usarse para dar la solución óptima. Tales
restricciones tienden a complicar los problemas de optimización porque la
solución óptima pueden encontrarse en un punto frontera del dominio. El método
de los multiplicadores de Lagrange es eminentemente práctico y facilita la
resolución de este tipo de situaciones.

## Teorema de Lagrange

Sean $F$ y $G$ dos funciones de tres variables, ambas con derivadas parciales
continuas y las derivadas de $G$ no son todas nulas. Sea $F_A$ la restricción de
$F$ al conjunto $A\{(x,y,z)/G(x,y,z)=0\}$.

Si $P$ es un punto crítico de $F_A$, entonces $P$ es un punto crítico de la
función $H$, definida de la siguiente manera:
$H(x,y,z,\lambda)=F(x,y,z)+\lambda G(x,y,z)$ donde $P$ pertenece al dominio de
$F$ y de $G$.

## Método de los multiplicadores de Lagrange

Si un problema de optimización de una función $f$ con restricciones $g_1=0$,
....., $g_m=0$ tiene un máximo o mínimo en un punto $P$ donde las todas las
funciones admiten derivadas parciales de primer orden continuas, y los vectores
gradientes de las funciones de restricción no se anulan en dicho punto; entonces
existen unos números, $\lambda$, $\mu$, ......, $\gamma$, llamados
multiplicadores de Lagrange, que dan lugar a la función
$F=f+\lambda g_1+\mu g_2+\cdots+\gamma g_m$, función de Lagrange, tales que $P$
es solución del sistema:

$$
\frac{dF}{dx_1}=0;\ \frac{dF}{dx_2}=0;\ \frac{dF}{dx_3}=0;\ \ldots;\ \frac{dF}{dx_n}=0
$$

$$
g_1(x_1,x_2,\ldots,x_n)=0;\ g_2(x_1,x_2,\ldots,x_n)=0;\ \ldots;\ g_m(x_1,x_2,\ldots,x_n)=0
$$

Una vez conocidos los puntos solución del sistema, podemos utilizar las
condiciones del problema para distinguir si son máximos o mínimos. Con
frecuencia son problemas geométricos y es fácil hacerlo. Si $P(a,b)$ es un punto
crítico, evaluamos $f(a,b)$ y los puntos terminales de la ecuación de ligadura
(condición), si los tiene y así distinguimos los valores máximos y mínimos.

## Ejemplo 1

Hallar el máximo de $f(x,y)=4xy$ donde $x>0$ e $y>0$, sujeto a la restricción o
ligadura $\left(\frac{x^2}{9}\right)+\left(\frac{y^2}{4}\right)=1$.

**Solución:** La función que queremos maximizar es $z=f(x,y)$ y la condición
$g(x,y)=0$ es $\left(\frac{x^2}{9}\right)+\left(\frac{y^2}{4}\right)-1=0$,
entonces trabajamos con la función
$H(x,y,\lambda)=4xy+\lambda\left[\left(\frac{x^2}{9}\right)+\left(\frac{y^2}{4}\right)-1\right]$
y hallamos sus puntos críticos resolviendo el sistema de ecuaciones que
obtenemos de igualar sus derivadas parciales a cero.

$$
\begin{cases}
H'_x=4y+\dfrac29x\lambda=0\\
H'_y=4x+\dfrac24y\lambda=0\\
H'_\lambda=\left(\dfrac{x^2}{9}\right)+\left(\dfrac{y^2}{4}\right)-1=0
\end{cases}
$$

despejamos $\lambda$ de la primera ecuación y el resultado obtenido lo
reemplazaremos en la tercera ecuación.

$\lambda=\frac{18y}{x}$ lo reemplazamos en la segunda ecuación y obtenemos
$x^2=\frac9{16}y^2$

que sustituyendo en la tercera ecuación nos queda:

$$
\left(\frac{x^2}{9}\right)+\left(\frac{y^2}{4}\right)-1=0
\quad\text{con }x^2=\frac9{16}y^2
\Rightarrow\left(\frac{\frac9{16}y^2}{9}\right)+\left(\frac{y^2}{4}\right)-1=0
\Rightarrow y^2=8\Rightarrow y=\pm2\sqrt2
$$

pero como $y>0$ se elige el valor positivo $y=2\sqrt2$ para hallar el valor de
$x$ $\Rightarrow$ reemplazando en $x^2=\frac9{16}y^2$ nos queda
$x=\frac3{\sqrt2}$

Por tanto, el valor máximo de $f$ es
$f\left(\frac3{\sqrt2},2\sqrt2\right)=4\cdot\frac3{\sqrt2}\cdot(2\sqrt2)=24$

Nota de transcripción: el original imprime $\lambda=18y/x$ sin signo negativo y
contiene pasos numéricos incompatibles en el ejemplo. Se conserva íntegramente
la solución dada, sin corregirla ni sustituirla por otra.
