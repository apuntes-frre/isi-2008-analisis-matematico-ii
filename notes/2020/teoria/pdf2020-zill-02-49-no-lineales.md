# 4.9 Ecuaciones diferenciales no lineales (comienzo)

> Transcripción del extracto *Ecuaciones diferenciales con aplicaciones de
> modelado*, atribuido a Zill por el nombre del archivo. Páginas impresas
> 174–176 (PDF 58–60). La sección continúa después de este rango. Material
> bibliográfico externo conservado en la carpeta de 2020; sin portada, edición
> ni año verificables en la copia.

## Página 174

### Repaso de material

- Secciones 2.2 y 2.5.
- Sección 4.2.
- También se recomienda un repaso de series de Taylor.

### Introducción

A continuación se examinan las dificultades en torno a las ED *no lineales* de
orden superior y los pocos métodos que producen soluciones analíticas. Dos de
los métodos de solución que se consideran en esta sección emplean un cambio de
variable para reducir una ED de segundo orden a una de primer orden. En ese
sentido los métodos son análogos al material de la sección 4.2.

### Algunas diferencias

Entre las ecuaciones diferenciales lineales y no lineales hay varias diferencias
importantes. En la sección 4.1 vimos que las ecuaciones lineales homogéneas de
orden dos o superior tienen la propiedad de que una combinación lineal de
soluciones también es una solución (teorema 4.1.2). Las ecuaciones no lineales
no tienen esta propiedad de superposición. Vea los problemas 1 y 18 de los
ejercicios 4.9. Podemos encontrar soluciones generales de ED lineales de primer
orden y ecuaciones de orden superior con coeficientes constantes. Aun cuando se
pueda resolver una ecuación diferencial no lineal de primer orden en la forma de
una familia uniparamétrica, esta familia no representa, como regla, una solución
general. Es decir, las ED no lineales de primer orden pueden tener soluciones
singulares, en tanto que las ecuaciones lineales no. Pero la principal
diferencia entre las ecuaciones lineales y no lineales de orden dos o superior
radica en el área de la solubilidad. Dada una ecuación lineal, hay una
probabilidad de encontrar alguna forma de solución que se pueda analizar, una
solución explícita o quizá una solución en la forma de una serie infinita (vea
el capítulo 6). Por otro lado, las ecuaciones diferenciales no lineales de orden
superior desafían virtualmente la solución con métodos analíticos. Aunque esto
podría sonar desalentador, aún hay cosas que se pueden hacer. Como se señaló al
final de la sección 1.3, siempre es posible analizar de modo cualitativo y
numérico una ED no lineal.

Desde el principio se aclaró que las ecuaciones diferenciales no lineales de
orden superior son importantes, digamos ¿quizá más que las lineales?, porque a
medida que se ajusta un modelo matemático, por ejemplo, un sistema físico, se
incrementa por igual la probabilidad de que este modelo de mayor definición sea
no lineal.

Empezamos por mostrar un método analítico que *en ocasiones* permite determinar
soluciones explícitas o implícitas de clases especiales de ecuaciones
diferenciales de segundo orden no lineales.

### Reducción de orden

Las ecuaciones diferenciales no lineales de segundo orden $F(x,y',y'')=0$, donde
falta la variable dependiente $y$, y $F(y,y',y'')=0$, donde falta la variable
independiente $x$, a veces se resuelven usando métodos de primer orden. Cada
ecuación se reduce a una de primer orden por medio de la sustitución $u=y'$.

En el ejemplo siguiente se ilustra la técnica de sustitución para una ecuación
de la forma $F(x,y',y'')=0$. Si $u=y'$, entonces la ecuación diferencial se
convierte en $F(x,u,u')=0$. Si podemos resolver esta última ecuación para $u$,
podemos encontrar a $y$ por integración. Observe que como se está resolviendo
una ecuación de segundo orden, su solución contendrá dos constantes arbitrarias.

### Ejemplo 1. Falta la variable dependiente y

Resuelva $y''=2x(y')^2$.

## Página 175

**Solución.** Si hacemos $u=y'$, entonces $du/dx=y''$. Después de sustituir, la
segunda ecuación diferencial se reduce a una ecuación de primer orden con
variables separables; la variable independiente es $x$ y la variable dependiente
es $u$:

$$
\frac{du}{dx}=2xu^2\quad\text{o}\quad\frac{du}{u^2}=2x\,dx
$$

$$
\int u^{-2}\,du=\int2x\,dx
$$

$$
-u^{-1}=x^2+c_1^2.
$$

La constante de integración se escribe como $c_1^2$ por conveniencia. La razón
debe ser obvia en los pocos pasos siguientes. Debido a que $u^{-1}=1/y'$, se
tiene que

$$
\frac{dy}{dx}=-\frac1{x^2+c_1^2},
$$

y así

$$
y=-\int\frac{dx}{x^2+c_1^2}
\quad\text{o}\quad y=-\frac1{c_1}\tan^{-1}\frac x{c_1}+c_2.
$$

A continuación se muestra cómo resolver una ecuación que tiene la forma
$F(y,y',y'')=0$. Una vez más se hace $u=y'$, pero debido a que falta la variable
independiente $x$, esta sustitución se usa para convertir la ecuación
diferencial en una en la que la variable independiente es $y$ y la variable
dependiente es $u$. Entonces utilizamos la regla de la cadena para calcular la
segunda derivada de $y$:

$$
y''=\frac{du}{dx}=\frac{du}{dy}\frac{dy}{dx}=u\frac{du}{dy}.
$$

En este caso la ecuación de primer orden que debemos resolver es

$$
F\left(y,u,u\frac{du}{dy}\right)=0.
$$

### Ejemplo 2. Falta la variable independiente x

Resuelva $yy''=(y')^2$.

**Solución.** Con ayuda de $u=y'$, la regla de la cadena que se acaba de mostrar
y de la separación de variables, la ecuación diferencial se convierte en

$$
y\left(u\frac{du}{dy}\right)=u^2\quad\text{o}\quad\frac{du}u=\frac{dy}y.
$$

Entonces, integrando la última ecuación se obtiene $\ln|u|=\ln|y|+c_1$, que, a
su vez, da $u=c_2y$, donde la constante $\pm e^{c_1}$ se identifica como $c_2$.
Ahora se vuelve a sustituir $u=dy/dx$, se separan de nuevo las variables, se
integra y se etiquetan las constantes por segunda vez:

$$
\int\frac{dy}y=c_2\int dx\quad\text{o}\quad\ln|y|=c_2x+c_3
\quad\text{o}\quad y=c_4e^{c_2x}.
$$

### Uso de series de Taylor

En algunos casos una solución de un problema con valores iniciales no lineales,
en el que las condiciones iniciales se específican en $x_0$, se puede aproximar
mediante una serie de Taylor centrada en $x_0$.

## Página 176

### Ejemplo 3. Series de Taylor de un PVI

Supongamos que existe una solución del problema con valores iniciales

$$
y''=x+y-y^2,\quad y(0)=-1,\quad y'(0)=1. \tag{1}
$$

Si además se supone que la solución $y(x)$ del problema es analítica en 0,
entonces $y(x)$ tiene un desarrollo en serie de Taylor centrado en 0:

$$
y(x)=y(0)+\frac{y'(0)}{1!}x+\frac{y''(0)}{2!}x^2
+\frac{y'''(0)}{3!}x^3+\frac{y^{(4)}(0)}{4!}x^4+\frac{y^{(5)}(0)}{5!}x^5+\cdots.
\tag{2}
$$

Observe que se conocen los valores del primero y segundo términos en la serie
(2) puesto que esos valores son las condiciones iniciales especificadas
$y(0)=-1$, $y'(0)=1$. Además, la ecuación diferencial por sí misma define el
valor de la segunda derivada en 0: $y''(0)=0+y(0)-y(0)^2=0+(-1)-(-1)^2=-2$.
Entonces se pueden encontrar expresiones para las derivadas superiores $y'''$,
$y^{(4)}$, $\ldots$ calculando las derivadas sucesivas de la ecuación
diferencial:

$$
y'''(x)=\frac d{dx}(x+y-y^2)=1+y'-2yy' \tag{3}
$$

$$
y^{(4)}(x)=\frac d{dx}(1+y'-2yy')=y''-2yy''-2(y')^2 \tag{4}
$$

$$
y^{(5)}(x)=\frac d{dx}(y''-2yy''-2(y')^2)=y'''-2yy'''-6y'y'', \tag{5}
$$

etcétera. Ahora usando $y(0)=-1$ y $y'(0)=1$, se encuentra de (3) que
$y'''(0)=4$. De los valores $y(0)=-1$, $y'(0)=1$ y $y''(0)=-2$ se encuentra
$y^{(4)}(0)=-8$ de (4). Con la información adicional de que $y'''(0)=4$,
entonces se ve de (5) que $y^{(5)}(0)=24$. Por tanto de (2) los primeros seis
términos de una solución en serie del problema con valores iniciales (1) son

$$
y(x)=-1+x-x^2+\frac23x^3-\frac13x^4+\frac15x^5+\cdots.
$$

### Uso de un programa de solución numérica

Los métodos numéricos, como el de Euler o el de Runge-Kutta, se desarrollaron
sólo para ecuaciones diferenciales de primer orden y luego se ampliaron a
sistemas de ecuaciones de primer orden. Para analizar en forma numérica un
problema con valores iniciales de $n$-ésimo orden, se expresa la EDO de
$n$-ésimo orden como un sistema de $n$ ecuaciones de primer orden. En resumen,
aquí se muestra cómo se hace esto para un problema con valores iniciales de
segundo orden: primero, se resuelve para $y''$, es decir, se escribe la ED en la
forma normal $y''=f(x,y,y')$ y después se hace que $y'=u$. Por ejemplo, si
sustituimos $y'=u$ en

$$
\frac{d^2y}{dx^2}=f(x,y,y'),\quad y(x_0)=y_0,\quad y'(x_0)=u_0, \tag{6}
$$

entonces $y''=u'$ y $y'(x_0)=u(x_0)$, por lo que el problema con valores
iniciales (6) se convierte en

$$
\text{Resuelva:}\quad
\begin{cases}
y'=u\\
u'=f(x,y,u)
\end{cases}
$$

$$
\text{Sujeto a:}\quad y(x_0)=y_0,\ u(x_0)=u_0.
$$

Sin embargo, se debe observar que un programa de solución numérica *podría no*
requerir[^programa] que se proporcione el sistema.

## Notas de transcripción

Se conserva la constante $c_1^2$ elegida en el ejemplo 1 y la familia presentada
sin ampliar sus casos ni añadir soluciones. Se conserva “segunda ecuación
diferencial” y la grafía “específican” de la página 175. La continuación de la
sección y sus ejercicios quedan fuera de este rango de páginas.

[^programa]: Algunos programas de solución numérica sólo requieren que una
    ecuación diferencial de segundo orden sea expresada en la forma
    normal $y''=f(x,y,y')$. La traducción de la única ecuación en un
    sistema de dos ecuaciones se construye en el programa de
    computadora, ya que la primera ecuación del sistema siempre es
    $y'=u$ y la segunda ecuación es $u'=f(x,y,u)$.
