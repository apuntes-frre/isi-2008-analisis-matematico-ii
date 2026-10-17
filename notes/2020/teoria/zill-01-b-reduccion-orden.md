# 4.2 Reducción de orden

> Fuente editorial atribuida a Zill por el archivo
> `Ecuaciones diferenciales con aplicaciones de modelado - Zill.pdf`,
> `2020/15-EDO 2do Orden/`. El extracto no contiene portada bibliográfica ni año
> de edición. Sin atribución a ISI. Desde el segundo tema de PDF14 (impresa130)
> hasta el primer tema de PDF17 (impresa133). Continuación de
> [teoría lineal](zill-01-a-teoria-lineal.md).

## Página 130 — 4.2 REDUCCIÓN DE ORDEN

REPASO DE MATERIAL

- Sección 2.5 (utilizando una sustitución).
- Sección 4.1.

**INTRODUCCIÓN.** En la sección anterior vimos que la solución general de una
ecuación diferencial lineal homogénea de segundo orden

```math
a_2(x)y''+a_1(x)y'+a_0(x)y=0\tag{1}
```

es una combinación lineal $`y=c_1y_1+c_2y_2`$, donde $`y_1`$ y $`y_2`$ son
soluciones que constituyen un conjunto linealmente independiente en cierto
intervalo $`I`$. Al comienzo de la siguiente sección se analiza un método para
determinar estas soluciones cuando los coeficientes de la ED en (1) son
constantes. Este método, que es un ejercicio directo en álgebra, falla en
algunos casos y sólo produce una solución simple $`y_1`$ de la ED. En estos
casos se puede construir una segunda solución $`y_2`$ de una ecuación homogénea
(1) (aun cuando los coeficientes en (1) son variables) siempre que se conozca
una solución no trivial $`y_1`$ de la ED. La idea básica que se describe en esta
sección es que *la ecuación (1) se puede reducir a una ED lineal de primer orden
por medio de una sustitución* en la que interviene la solución conocida $`y_1`$.
Una segunda solución $`y_2`$ de (1) es evidente después de resolver la ED de
primer orden.

**REDUCCIÓN DE ORDEN.** Suponga que $`y_1`$ denota una solución no trivial de
(1) y que $`y_1`$ se define en un intervalo $`I`$. Se busca una segunda solución
$`y_2`$ tal que $`y_1`$ y $`y_2`$ sean un conjunto linealmente independiente en
$`I`$. Recuerde de la sección 4.1 que si $`y_1`$ y $`y_2`$ son linealmente
independientes, entonces su cociente $`y_2/y_1`$ no es constante en $`I`$, es
decir, $`y_2(x)/y_1(x)=u(x)`$ o $`y_2(x)=u(x)y_1(x)`$. La función $`u(x)`$ se
determina al sustituir $`y_2(x)=u(x)y_1(x)`$ en la ecuación diferencial dada.
Este método se llama **reducción de orden** porque debemos resolver una ecuación
diferencial lineal de primer orden para encontrar a $`u`$.

## Página 131

### EJEMPLO 1. Una segunda solución por reducción de orden

Dado que $`y_1=e^x`$ es una solución de $`y''-y=0`$ en el intervalo
$`(-\infty,\infty)`$, use reducción de orden para determinar una segunda
solución $`y_2`$.

**SOLUCIÓN.** Si $`y=u(x)y_1(x)=u(x)e^x`$, entonces aplicando la regla del
producto se obtiene

```math
y'=ue^x+e^xu',\quad y''=ue^x+2e^xu'+e^xu'',
```

por tanto

```math
y''-y=e^x(u''+2u')=0.
```

Puesto que $`e^x\ne0`$, la última ecuación requiere que $`u''+2u'=0`$. Si se
hace la sustitución $`w=u'`$, esta ecuación lineal de segundo orden en $`u`$ se
convierte en $`w'+2w=0`$, que es una ecuación lineal de primer orden en $`w`$.
Si se usa el factor integrante $`e^{2x}`$, se puede escribir
$`\frac d{dx}[e^{2x}w]=0`$. Después de integrar, se obtiene $`w=c_1e^{-2x}`$ o
$`u'=c_1e^{-2x}`$. Al integrar de nuevo se obtiene $`u=-\frac12c_1e^{-2x}+c_2`$.
Así

```math
y=u(x)e^x=-\frac{c_1}2e^{-x}+c_2e^x.\tag{2}
```

Haciendo $`c_2=0`$ y $`c_1=-2`$, se obtiene la segunda solución deseada,
$`y_2=e^{-x}`$. Puesto que $`W(e^x,e^{-x})\ne0`$ para toda $`x`$, las soluciones
son linealmente independientes en $`(-\infty,\infty)`$.

Puesto que se ha demostrado que $`y_1=e^x`$ y $`y_2=e^{-x}`$ son soluciones
linealmente independientes de una ecuación lineal de segundo orden, la expresión
en (2) es en realidad la solución general de $`y''-y=0`$ en
$`(-\infty,\infty)`$.

**CASO GENERAL.** Suponga que se divide entre $`a_2(x)`$ para escribir la
ecuación (1) en la **forma estándar**

```math
y''+P(x)y'+Q(x)y=0,\tag{3}
```

donde $`P(x)`$ y $`Q(x)`$ son continuas en algún intervalo $`I`$. Supongamos
además que $`y_1(x)`$ es una solución conocida de (3) en $`I`$ y que
$`y_1(x)\ne0`$ para toda $`x`$ en el intervalo. Si se define $`y=u(x)y_1(x)`$,
se tiene que

```math
y'=uy_1'+y_1u',\quad y''=uy_1''+2y_1'u'+y_1u''
```

```math
y''+Py'+Qy=u[\underbrace{y_1''+Py_1'+Qy_1}_{\text{cero}}]
+y_1u''+(2y_1'+Py_1)u'=0.
```

Esto implica que se debe tener

```math
y_1u''+(2y_1'+Py_1)u'=0\quad\text{o}\quad
 y_1w'+(2y_1'+Py_1)w=0,\tag{4}
```

donde hacemos que $`w=u'`$. Observe que la última ecuación en (4) es tanto
lineal como separable. Separando las variables e integrando, se obtiene

```math
\frac{dw}{w}+2\frac{y_1'}{y_1}\,dx+P\,dx=0
```

```math
\ln|wy_1^2|=-\int P\,dx+c\quad\text{o}\quad wy_1^2=c_1e^{-\int P\,dx}.
```

Despejamos a $`w`$ de la última ecuación, usamos $`w=u'`$ e integrando
nuevamente:

```math
u=c_1\int\frac{e^{-\int P\,dx}}{y_1^2}\,dx+c_2.
```

## Página 132

Eligiendo $`c_1=1`$ y $`c_2=0`$, se encuentra de $`y=u(x)y_1(x)`$ que una
segunda solución de la ecuación (3) es

```math
y_2=y_1(x)\int\frac{e^{-\int P(x)\,dx}}{y_1^2(x)}\,dx.\tag{5}
```

Un buen ejercicio de derivación es comprobar que la función $`y_2(x)`$ que se
define en (5) satisface la ecuación (3) y que $`y_1`$ y $`y_2`$ son linealmente
independientes en algún intervalo en el que $`y_1(x)`$ no es cero.

### EJEMPLO 2. Una segunda solución por la fórmula (5)

La función $`y_1=x^2`$ es una solución de $`x^2y''-3xy'+4y=0`$. Encuentre la
solución general de la ecuación diferencial en el intervalo $`(0,\infty)`$.

**SOLUCIÓN.** De la forma estándar de la ecuación,

```math
y''-\frac3xy'+\frac4{x^2}y=0,
```

encontramos de (5)

```math
\begin{aligned}
y_2&=x^2\int\frac{e^{3\int dx/x}}{x^4}\,dx\\
&=x^2\int\frac{dx}x=x^2\ln x.
\end{aligned}
```

Nota de la fórmula: $`e^{3\int dx/x}=e^{\ln x^3}=x^3`$.

La solución general en el intervalo $`(0,\infty)`$ está dada por
$`y=c_1y_1+c_2y_2`$; es decir, $`y=c_1x^2+c_2x^2\ln x`$.

### COMENTARIOS

i) La deducción y uso de la fórmula (5) se ha mostrado aquí porque esta fórmula
aparece de nuevo en la siguiente sección y en las secciones 4.7 y 6.2. La
ecuación (5) se usa simplemente para ahorrar tiempo en obtener un resultado
deseado. Su profesor le indicará si debe memorizar la ecuación (5) o si debe
conocer los primeros principios de la reducción de orden.

ii) La reducción de orden se puede usar para encontrar la solución general de
una ecuación no homogénea $`a_2(x)y''+a_1(x)y'+a_0(x)y=g(x)`$ siempre que se
conozca una solución $`y_1`$ de la ecuación homogénea asociada. Vea los
problemas 17 a 20 en los ejercicios 4.2.

### EJERCICIOS 4.2

*Las respuestas a los problemas con número impar comienzan en la página RES-4.*

En los problemas 1 a 16 la función indicada $`y_1(x)`$ es una solución de la
ecuación diferencial dada. Use la reducción de orden o la fórmula (5), como se
indica, para encontrar una segunda solución $`y_2(x)`$.

1\) $`y''-4y'+4y=0`$; $`y_1=e^{2x}`$.

2\) $`y''+2y'+y=0`$; $`y_1=xe^{-x}`$.

3\) $`y''+16y=0`$; $`y_1=\cos4x`$.

4\) $`y''+9y=0`$; $`y_1=\mathop{\mathrm{sen}}\nolimits 3x`$.

5\) $`y''-y=0`$; $`y_1=\cosh x`$.

6\) $`y''-25y=0`$; $`y_1=e^{5x}`$.

7\) $`9y''-12y'+4y=0`$; $`y_1=e^{2x/3}`$.

8\) $`6y''+y'-y=0`$; $`y_1=e^{x/3}`$.

9\) $`x^2y''-7xy'+16y=0`$; $`y_1=x^4`$.

10\) $`x^2y''+2xy'-6y=0`$; $`y_1=x^2`$.

11\) $`xy''+y'=0`$; $`y_1=\ln x`$.

12\) $`4x^2y''+y=0`$; $`y_1=x^{1/2}\ln x`$.

13\) $`x^2y''-xy'+2y=0`$; $`y_1=x\mathop{\mathrm{sen}}\nolimits (\ln x)`$.

14\) $`x^2y''-3xy'+5y=0`$; $`y_1=x^2\cos(\ln x)`$.

## Página 133 — Continuación de ejercicios 4.2

15\) $`(1-2x-x^2)y''+2(1+x)y'-2y=0`$; $`y_1=x+1`$.

16\) $`(1-x^2)y''+2xy'=0`$; $`y_1=1`$.

En los problemas 17 al 20 la función que se indica $`y_1(x)`$ es una solución de
la ecuación homogénea asociada. Use el método de reducción de orden para
determinar una segunda solución $`y_2(x)`$ de la ecuación homogénea y una
solución particular de la ecuación no homogénea dada.

17\) $`y''-4y=2`$; $`y_1=e^{-2x}`$.

18\) $`y''+y'=1`$; $`y_1=1`$.

19\) $`y''-3y'+2y=5e^{3x}`$; $`y_1=e^x`$.

20\) $`y''-4y'+3y=x`$; $`y_1=e^x`$.

### Problemas para analizar

21\) a) Proporcione una demostración convincente de que la ecuación de segundo
orden $`ay''+by'+cy=0`$, $`a,b`$, y $`c`$ constantes, tiene siempre cuando menos
una solución de la forma $`y_1=e^{m_1x}`$, $`m_1`$ es una constante.

b) Explique por qué la ecuación diferencial que se proporciona en el inciso a)
debe tener una segunda solución de la forma $`y_2=e^{m_2x}`$ o de la forma
$`y_2=xe^{m_1x}`$, $`m_1`$ y $`m_2`$ son constantes.

c) Analice de nuevo los problemas 1 al 8. ¿Puede explicar por qué los enunciados
de los incisos a) y b) anteriores no se contradicen con las respuestas de los
problemas 3 al 5?

22\) Compruebe que $`y_1(x)=x`$ es una solución de $`xy''-xy'+y=0`$. Utilice la
reducción de orden para encontrar una segunda solución $`y_2(x)`$ en la forma de
una serie infinita. Estime un intervalo de definición para $`y_2(x)`$.

### Tarea para el laboratorio de computación

23\) a) Compruebe que $`y_1(x)=e^x`$ es una solución de

```math
xy''-(x+10)y'+10y=0.
```

b) Use la ecuación (5) para determinar una segunda solución $`y_2(x)`$. Usando
un SAC realice la integración que se requiere.

c) Explique, usando el corolario (A) del teorema 4.1.2, por qué la segunda
solución puede escribirse en forma compacta como

```math
y_2(x)=\sum_{n=0}^{10}\frac1{n!}x^n.
```

Continúa en
[4.3 Ecuaciones lineales homogéneas con coeficientes constantes](zill-01-c-coeficientes-constantes.md),
que comienza en esta misma página del original.
