<!-- markdownlint-disable MD029 -->

# Análisis vectorial

Fuente: `Análisis vectorial (1).pdf`, páginas 1–2.
[Procedencia](../../../resources/2016/fuentes.md).

1. Dar la definición de función vectorial en el plano y en el espacio.
1. Si $r(t)$ es una función vectorial, ¿es la gráfica de la función vectorial
   $u(t)=r(t-2)$ una traslación horizontal de la gráfica de $r(t)$?
1. Definir derivada de una función vectorial. Describir cómo hallar la derivada
   de una función vectorial y dar su interpretación geométrica.
1. ¿Cómo se encuentra la integral de una función vectorial?
1. La componente $z$ de la derivada de la función vectorial $\vec{u}$ es 0 para
   $t$ en el dominio de la función. ¿Qué implica esa información acerca de la
   gráfica de $\vec{u}$?

<!-- El original reinicia la numeración. -->

1. Dibujar la curva plana representada por la función vectorial
   $r(t)=2\cos t\vec{i}-3\operatorname{sen}t\vec{j}$, $0\le t\le2\pi$.

1. Dibujar la curva en el espacio representada por la función vectorial
   $r(t)=4\cos t\vec{i}-4\operatorname{sen}t\vec{j}+t\vec{k}$, $0\le t\le4\pi$.

1. Representar la parábola $y=x^2+1$ mediante una función vectorial

1. Usar un sistema computacional para representar gráficamente las función
   vectorial $r(t)$. Para cada $u(t)$, conjeturar sobre la transformación (si la
   hay) de la gráfica de $r(t)$. Usar un sistema computacional con el objeto de
   verificar la conjetura.
   $r(t)=2\cos t\vec{i}+2\operatorname{sen}t\vec{j}+\frac12t\vec{k}$

   a. $u(t)=2(\cos t-1)\vec{i}+2\operatorname{sen}t\vec{j}+\frac12t\vec{k}$

   b. $u(t)=2\cos t\vec{i}+2\operatorname{sen}t\vec{j}+2t\vec{k}$

   c. $u(t)=2\cos(-t)\vec{i}+2\operatorname{sen}(-t)\vec{j}+\frac12(-t)\vec{k}$

   d. $u(t)=\frac12t\vec{i}+2\operatorname{sen}t\vec{j}+2\cos t\vec{k}$

   e. $u(t)=6\cos t\vec{i}+6\operatorname{sen}t\vec{j}+\frac12t\vec{k}$

## Definiciones

Si $x(t)$ e $y(t)$ son funciones que tienen primera y segunda derivada y $r$ s
una función vectorial que describe una curva suave, dada por $r(t)=x(t)i+y(t)j$,
entonces:

Velocidad $v(t)=r'(t)=x'(t)i+y'(t)j$

Aceleración $a(t)=r''(t)=x''(t)i+y''(t)j$

Rapidez $\|v(t)\|=\|r'(t)\|=\sqrt{[x'(t)]^2+[y'(t)]^2}$

Longitud de la curva $L=\int_a^b\sqrt{[x'(t)]^2+[y'(t)]^2}\,dt$ con
$a\le t\le b$

<!-- Página 2; continúa la lista de ejercicios. -->

5. El vector posición $r$ describe la trayectoria de un objeto que se mueve en
   el plano $xy$. Dibujar una gráfica de la trayectoria y dibujar los vectores
   velocidad y aceleración en el punto dado.

   a. $\vec{r}(t)=3t\vec{i}+(t-1)\vec{j}$ en $(3,0)$

   b. $\vec{r}(t)=(6-t)\vec{i}+t\vec{j}$ en $(3,3)$

   c. $\vec{r}(t)=(t-\operatorname{sen}t,1-\cos t)$ en $(\pi,2)$

1. Una partícula se mueve a lo largo de una curva plana $C$ descripta por
   $r(t)=2\operatorname{sen}\frac{t}{2}\vec{i}+2\cos\frac{t}{2}\vec{j}$, con
   $0\le t\le2\pi$ hallar: a) el vector velocidad b) la rapidez de la partícula
   c) el vector aceleración d) la longitud del camino recorrido desde que $t=0$
   hasta $t=\pi$ e) Graficar $C$

## Campos vectoriales

1. Definir un campo vectorial en el plano y en el espacio. Dar algunos ejemplos
   físicos de campos vectoriales.
1. ¿Qué es un campo vectorial conservativo y cuál es su criterio en el plano y
   en el espacio?
1. Definir el rotacional de un campo vectorial.
1. Definir la divergencia de un campo vectorial en el plano y en el espacio.

<!-- El original reinicia la numeración. -->

1. Utilizar un sistema computacional para representar gráficamente varios
   vectores representativos de los campos vectoriales:

   a. $\vec{F}(x,y)=\frac18(2xy\vec{i}+y^2\vec{j})$

   b. $\vec{F}(x,y)=(2y-3x)\vec{i}+(2y+3x)\vec{j})$

   c. $\vec{F}(x,y)=\frac{x\vec{i}+y\vec{j}+z\vec{k}}{\sqrt{x^2+y^2+z^2}}$

Nota de transcripción: se conservan «r s», el paréntesis de cierre adicional en
Campos vectoriales 1.b y los argumentos $(x,y)$ de 1.c. Las estrellas
decorativas destacan ejercicios de uso computacional y no contienen texto.
