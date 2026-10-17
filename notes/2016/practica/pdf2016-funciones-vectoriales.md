# Funciones vectoriales

Fuente: `Funciones_vectoriales.pdf`, páginas 1–2.
[Procedencia](../../../resources/2016/fuentes.md).

1. Representar las curvas planas por medio de una función vectorial

   a. $`y=4-x`$

   b. $`y=(x-2)^2`$

   c. $`x^2+y^2=25`$

   d. $`(x-2)^2+y^2=4`$

1. Una partícula sigue la trayectoria recta que pasa por los puntos $`(2,3,0)`$
   y $`(0,8,8)`$. Hallar una función vectorial para la trayectoria. (Hay muchas
   respuestas posibles).

1. El borde exterior de un tobogán tiene forma de hélice de radio 1.5 metros. El
   tobogán tiene una altura de 2 metros y da una vuelta completa de arriba hacia
   abajo. Hallar una función vectorial para la hélice. (Hay muchas respuestas
   posibles).

1. Dibujar las curvas en el espacio representadas por la intersección de las
   superficies. Después representar las curvas por medio de una función
   vectorial usando el parámetro dado.

   | Superficies | Parámetro |
   | -- | -- |
   | $`z=x^2+y^2`$, $`x+y=0`$ | $`x=t`$ |
   | $`z=x^2+y^2`$, $`z=4`$ | $`X=2\cos t`$ |
   | $`x^2+y^2=4`$, $`z=x^2`$ | $`X=2\mathop{\mathrm{sen}}\nolimits t`$ |

1. El vector posición $`\vec{r}(t)`$ describe la trayectoria de un objeto que se
   mueve en el espacio. Hallar la velocidad, la rapidez y la aceleración del
   objeto.

   a. $`\vec{r}(t)=t\vec{i}+t^2\vec{j}+\frac{t^2}{2}\vec{k}`$

   b. $`\vec{r}(t)=t\vec{i}+t\vec{j}+\sqrt{9-t^2}\vec{k}`$

   c. $`\vec{r}(t)=(e^t\cos t,e^t\mathop{\mathrm{sen}}\nolimits t,e^t)`$

## Vectores tangentes y normales

Sea $`C`$ una curva suave en un intervalo abierto $`I`$, representada por
$`r(t)`$:

**Vector unitario tangente** $`T(t)=\frac{r'(t)}{\|r'(t)\|}`$, $`r'(t)\ne0`$

**Vector unitario normal principal** $`N(t)=\frac{T'(t)}{\|T'(t)\|}`$,
$`T'(t)\ne0`$

**Teorema:** Si $`r(t)`$ es el vector posición de una curva suave $`C`$ y
$`N(t)`$ existe, entonces el vector aceleración $`a(t)`$ se encuentra en el
plano determinado por $`T(t)`$ y $`N(t)`$.

**Teorema: :** Si $`r(t)`$ es el vector posición de una curva suave $`C`$ y
$`N(t)`$ existe, entonces las componentes tangencial y normal de la aceleración
son:

```math
a_T=a\cdot T=\frac{v\cdot a}{\|v\|}
```

```math
a_N=a\cdot N=\frac{\|v\times a\|}{\|v\|}=\sqrt{\|a\|^2-a_T^2}
```

A la componente normal de la aceleración se la llama **componente centrípeta de
la aceleración**.

1. Para un objeto que se mueve a lo largo de la trayectoria dada por la función
   vectorial $`r(t)`$, hallar $`v(t)`$, $`a(t)`$, $`T(t)`$ y $`N(t)`$ (si
   existe). Usar los resultados para determinar la forma de la trayectoria. ¿Es
   constante la rapidez del objeto o cambiante?

   a. $`r(t)=4t\vec{i}`$

   b. $`r(t)=4t^2\vec{i}`$

   c. $`r(t)=4t\vec{i}-2t\vec{j}`$

   d. $`r(t)=4t^2\vec{j}+\vec{k}`$

1. Considerar la hélice representada por
   $`\vec{r}(t)=(2\cos t,2\mathop{\mathrm{sen}}\nolimits t,t)`$

   a. Expresar la longitud de arco $`s`$ de la hélice como función de $`t`$

   b. Hallar las coordenadas del punto en la hélice con longitud de arco
   $`s=\sqrt5`$ y $`s=4`$
