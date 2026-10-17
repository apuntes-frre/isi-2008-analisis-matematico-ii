# Ecuaciones diferenciales ordinarias — Parte 2

> Fuente: `2020/15-EDO 2do Orden/Apunte Ecuaciones Diferenciales.pdf`. Apunte de
> las clases del Ing. Leopoldo S. de Urrutia. Universidad Tecnológica Nacional,
> Facultad Regional Resistencia. Sin año impreso. Páginas impresas 16–28 (PDF
> 18–30). Se conservan las expresiones y erratas del original. Procedencia en
> [cobertura](../../../resources/2020/pdf2020-cobertura.md).

## Página 16 — ECUACIONES DIFERENCIALES LINEALES DE SEGUNDO ORDEN

Sea la ecuación diferencial general de la forma:

```math
y^{(n)}+a_1y^{(n-1)}+a_2y^{(n-2)}+\cdots+a_{n-1}y'+a_ny=f(x)
```

donde los coeficientes $`a_1,a_2,\ldots,a_n`$ son constantes, o a lo sumo
funciones de una única variable independiente $`x`$. Por ser esta ecuación de
primer grado algebraico respecto de la función “$`y`$” y de sus derivadas, es de
tipo lineal, y por ser “$`n`$” su mayor orden de derivación, será una ecuación
diferencial lineal de orden “$`n`$”.

Si en particular hacemos $`n=2`$ obtendremos:

```math
y''+a_1y'+a_2y=f(x)\tag{1}
```

Ecuación Diferencial Segundo Orden, ecuación ésta que estudiaremos su
resolución.

A los efectos de la determinación de las soluciones de la ecuación diferencial,
tendremos en cuenta las siguientes propiedades:

### Primera propiedad

Si $`y_1\land y_2`$ son soluciones de la ecuación diferencial (1), se puede
demostrar que la función $`y=y_1+y_2`$ es también solución de la ecuación.

```math
\text{Si }y_1\land y_2\in S\Rightarrow y=y_1+y_2\in S
```

como $`y_1\in S`$ se verificará en (1): $`y_1''+a_1y_1'+a_2y_1=0`$

como $`y_2\in S`$ se verificará en (1): $`y_2''+a_1y_2'+a_2y_2=0`$

supongamos ahora la función $`y=y_1+y_2\in S`$ se verificará en (1):

```math
(y_1+y_2)''+a_1(y_1+y_2)'+a_2(y_1+y_2)=0
```

operando en el primer miembro

```math
y_1''+y_2''+a_1y_1'+a_1y_2'+a_2y_1+a_2y_2=0
```

agrupando términos:

```math
(y_1''+a_1y_1'+a_2y_1)+(y_2''+a_1y_2'+a_2y_2)=0
```

como $`y_1\land y_2\in S`$, $`0+0=0\ \therefore\ y\in S`$.

### Segunda propiedad

Si $`y_1`$ es solución de la Ecuación Diferencial (1) la función $`y=Cy_1`$ es
también una solución. ($`C=`$ constante ó función que no depende de $`x`$).

## Página 17

```math
\text{Si }y_1\in S\Rightarrow y=Cy_1\in S
```

Si $`y_1\in S`$ se verificará en (1): $`y_1''+a_1y_1'+a_2y_1=0`$

si $`y=Cy_1\in S`$ se verificará en (1)

```math
(Cy_1)''+a_1(Cy_1)'+a_2(Cy_1)=0
```

operando en esta expresión:

```math
Cy_1''+a_1Cy_1'+a_2Cy_1=0
```

Factorizando:

```math
C(y_1''+a_1y_1'+a_2y_1)=0
```

como $`y_1\in S\Rightarrow C\cdot0=0\quad\forall C`$

```math
\therefore\quad y=Cy_1\in S
```

### Tercera propiedad

```math
\text{Si }y_1\land y_2\in S\Rightarrow y=C_1y_1+C_2y_2\in S
```

donde $`C_1\land C_2`$ son constantes. Para su demostración debemos tener en
cuenta la aplicación de las dos propiedades anteriores.

### Cuarta propiedad

Dos funciones $`y_1\land y_2`$, ambas soluciones de una ecuación diferencial son
linealmente independientes, cuando la razón entre ambas “no es una constante”.

Dada $`y_1\land y_2\in S`$

```math
\text{si }\frac{y_1}{y_2}=K\Rightarrow
 y_1\land y_2\text{ son linealmente dependientes}
```

```math
\therefore\quad y=C_1y_1+C_2y_2\notin S
```

```math
\text{si }\frac{y_1}{y_2}\ne K\Rightarrow
 y_1\land y_2\text{ son linealmente independientes}.
```

Otra forma para determinar si son linealmente independientes, es aplicando los
conceptos de álgebra y geometría analítica:

si $`y_1\land y_2\in S\ \therefore`$ en el sistema:

```math
\begin{cases}
C_1y_1+C_2y_2=0\\
C_1y_1'+C_2y_2'=0
\end{cases}\quad\forall x\in I
```

```math
\text{si }W(y_1,y_2)=\begin{vmatrix}y_1&y_2\\y_1'&y_2'\end{vmatrix}\ne0
\Rightarrow C_1=C_2=0
\Rightarrow y_1\land y_2\text{ son linealmente independientes}.
```

esta última expresión $`W(y_1,y_2)`$, llamada determinante de wronski.

## Página 18

También simplemente se la suele denominar como Wronskiano de las funciones
$`y_1\land y_2`$, es de suma importancia en la resolución de ecuaciones
diferenciales de orden superior.

### Soluciones de Ecuación Diferencial

```math
y''+a_1y'+a_2y=0\tag{1}
```

Analicemos primeramente la forma de la solución de una ecuación diferencial
lineal homogénea de primer Orden, de la forma:

```math
\frac{dy}{dx}-ry=0\quad\text{ó}\quad y'-ry=0,
```

operando tendríamos:

```math
\frac{dy}{dx}=ry\Rightarrow\frac{dy}{y}=r\,dx
```

integrando obtenemos:

```math
\int\frac{dy}{y}=\int r\,dx\Rightarrow\ln y=rx+\ln C
```

ó también

```math
\ln y-\ln C=rx\quad\therefore\quad\ln\frac yC=rx
\Rightarrow\frac yC=e^{rx}
```

donde $`y=Ce^{rx}`$, ésta es una función de tipo exponencial y por tanto los
coeficientes que aparezcan en las derivadas sucesivas de la función “$`y`$”
serán un múltiplo de sí mismo, veamos:

```math
y=Ce^{rx}\Rightarrow y'=Cre^{rx}\Rightarrow y''=Cr^2e^{rx}
\Rightarrow y'''=Cr^3e^{rx}\ldots
```

siendo $`r`$ una constante. Por esto, es factible que una función de este tipo,
pueda ser propuesta como posible solución de una ecuación diferencial de 2do
orden como la enunciada (1).

Si $`y=Ce^{rx}\in S\quad\forall r=`$ constante “$`y`$” deberá satisfacer la
ecuación diferencial (1) propuesta.

```math
y=e^{rx}\Rightarrow y'=re^{rx}\Rightarrow y''=r^2e^{rx}
```

reemplazando en (1)

```math
y''+a_1y'+a_2y=0
```

```math
r^2e^{rx}+a_1re^{rx}+a_2e^{rx}=0
```

```math
e^{rx}(r^2+a_1r+a_2)=0
```

como $`e^{rx}\ne0`$ deberá cumplirse que $`r^2+a_1r+a_2=0`$ expresión ésta que
se la define como “ecuación característica asociada a la ecuación diferencial
(1)”.

## Página 19

Los valores de $`r`$ que verifiquen la igualdad serán aquellos obtenidos por:

```math
r_{1,2}=\frac{-a_1\pm\sqrt{a_1^2-4a_2}}2
```

por ser una ecuación de 2do grado, por lo tanto es necesario un análisis para
los distintos casos:

1º) si $`a_1^2-4a_2>0\Rightarrow r_1\ne r_2;\quad r_1\land r_2\in\mathbb R`$

2º) si $`a_1^2-4a_2=0\Rightarrow r_1=r_2=r=-a_1/2\in\mathbb R`$

3º) si $`a_1^2-4a_2<0\Rightarrow r_{1,2}=\alpha\pm\beta i\in\mathbb C`$

### Caso de raíces reales y distintas

$`r_1\land r_2\in\mathbb R;\quad r_1\ne r_2`$.

Si $`r_1\land r_2`$ son ceros de la ecuación asociada, las funciones
$`y_1=e^{r_1x}\land y_2=e^{r_2x}`$ serán dos soluciones de la ecuación
diferencial (1).

Verifiquemos si son linealmente independientes:

```math
\begin{aligned}
W(y_1,y_2)&=\begin{vmatrix}
e^{r_1x}&e^{r_2x}\\r_1e^{r_1x}&r_2e^{r_2x}
\end{vmatrix}\\
&=r_2e^{(r_1+r_2)x}-r_1e^{(r_1+r_2)x}\\
&=(r_2-r_1)e^{(r_1+r_2)x}\ne0
\end{aligned}
```

Si $`W(y_1,y_2)\ne0`$, $`y_1`$ e $`y_2`$ son linealmente independientes y por lo
tanto son “soluciones particulares” de la Ecuación Diferencial (1) y la solución
general será:

```math
y=C_1e^{r_1x}+C_2e^{r_2x}
```

Ejemplo: Resolver: $`y''+3y'-4y=0`$.

La ecuación característica asociada será: $`r^2+3r-4=0`$

por lo tanto $`r_1=1`$, $`r_2=-4\Rightarrow y_1=e^x;\ y_2=e^{-4x}`$

```math
y=C_1e^x+C_2e^{-4x}
```

### Caso de raíces reales iguales

Si $`r_1\land r_2\in\mathbb R`$ además $`r_1=r_2=r=-a_1/2`$

```math
y_1=e^{r_1x},\quad y_2=e^{r_2x}
```

pero $`W(y_1,y_2)=e^{(r_1+r_2)x}(r_2-r_1)=0`$.

## Página 20

por lo que $`y_1\land y_2`$ son linealmente dependientes.

Proponemos entonces una solución de la forma:

```math
y=\phi(x)e^{rx}
```

para simplificar la escritura llamamos $`\phi(x)=\phi`$.

```math
y=\phi e^{rx}\Rightarrow y'=\phi'e^{rx}+\phi re^{rx}
```

```math
y''=\phi''e^{rx}+2r\phi'e^{rx}+r^2\phi e^{rx}
```

si es solución de la ecuación diferencial (1), deberá satisfacerla.

```math
(\phi''e^{rx}+2r\phi'e^{rx}+r^2\phi e^{rx})
+a_1(\phi'e^{rx}+\phi re^{rx})+a_2\phi e^{rx}=0
```

```math
e^{rx}[\phi''+\underbrace{(2r+a_1)}_0\phi'
+\underbrace{(r^2+a_1r+a_2)}_0\phi]=0
```

como $`e^{rx}\ne0`$

```math
\phi''=0\Rightarrow\phi'=C_1\Rightarrow\phi=C_1x+C_2
\quad\therefore\quad y=(C_1x+C_2)e^{rx}
```

Ejemplo: Resolver $`y''+4y'+4y=0`$.

La ecuación característica será: $`r^2+4r+4=0\Rightarrow r_1=r_2=-2`$.

```math
y=(C_1x+C_2)e^{-2x}\Rightarrow y_1=e^{-2x},\quad y_2=xe^{-2x}
```

### Caso de raíces complejas

Si
$`r_1\ne r_2;\quad r_1\land r_2\in\mathbb C\Rightarrow r_{1,2}=\alpha\pm i\beta`$.

Este caso admite la misma solución prevista para el caso de raíces reales y
distintas, o sea, si $`r_1=\alpha+i\beta\land r_2=\alpha-i\beta`$

```math
y_1=e^{r_1x},\quad y_2=e^{r_2x}
\Rightarrow y=C_1e^{(\alpha+\beta i)x}+C_2e^{(\alpha-\beta i)x}
```

operando podemos dar una forma equivalente mediante una función real de variable
real basándonos en las “fórmulas de Euler”. Recordemos:

```math
e^{i\beta x}=\cos\beta x+i\mathop{\mathrm{sen}}\nolimits \beta x
```

```math
e^{-i\beta x}=\cos\beta x-i\mathop{\mathrm{sen}}\nolimits \beta x
```

entonces

```math
y=C_1e^{(\alpha+\beta i)x}+C_2e^{(\alpha-\beta i)x}
=C_1e^{\alpha x}e^{i\beta x}+C_2e^{\alpha x}e^{-i\beta x}
```

## Página 21

```math
\begin{aligned}
y&=e^{\alpha x}(C_1e^{i\beta x}+C_2e^{-i\beta x})\\
&=e^{\alpha x}[C_1(\cos\beta x+i\mathop{\mathrm{sen}}\nolimits \beta x)
+C_2(\cos\beta x-i\mathop{\mathrm{sen}}\nolimits \beta x)]\\
&=e^{\alpha x}[(C_1+C_2)\cos\beta x+i(C_1-C_2)\mathop{\mathrm{sen}}\nolimits \beta x]
\end{aligned}
```

si $`C_1+C_2=P;\quad i(C_1-C_2)=Q`$

```math
y=e^{\alpha x}(P\cos\beta x+Q\mathop{\mathrm{sen}}\nolimits \beta x)
```

Supongamos ahora una ecuación diferencial general completa, o sea que su segundo
miembro es distinto de cero y tendría forma:

```math
a_0y^{(n)}+a_1y^{(n-1)}+a_2y^{(n-2)}+\cdots+a_{n-1}y'+a_ny=b(x)\tag{1}
```

podemos, para simplificar la escritura durante su análisis, expresar la misma
ecuación diferencial mediante un operador diferencial:

```math
\phi(D)y=b(x)
```

si en particular $`\phi[D]y=0`$ estamos en presencia de una ecuación diferencial
homogénea de orden “$`n`$” $`\forall a_0\ne0`$.

Supongamos que:

La función $`Y_p`$ es una solución particular de (1)

```math
\phi[D]Y_p=b(x)
```

que $`Y_c`$ es una solución de la ecuación diferencial complementaria (u
homogénea) ó sea $`\phi[D]Y_c=0`$. En estas condiciones la función
$`Y_g=Y_c+Y_p`$

```math
Y_g'=Y_c'+Y_p'\qquad Y_g''=Y_c''+Y_p''\quad\ldots
```

observamos que $`Y_g`$ y sus derivadas sucesivas se componen de la suma de 2
términos que contienen a $`Y_c`$ ó $`Y_p`$ o sus respectivas derivadas según el
orden del término que se tome, reemplazándolas en (1) tendremos:

```math
a_0y^{(n)}+a_1y^{(n-1)}+\cdots+a_{n-1}y'+a_ny=b(x)
```

```math
a_0(Y_c^{(n)}+Y_p^{(n)})+a_1(Y_c^{(n-1)}+Y_p^{(n-1)})
+\cdots+a_{n-1}(Y_c'+Y_p')+a_n(Y_c+Y_p)=b(x)
```

```math
(a_0Y_c^{(n)}+a_1Y_c^{(n-1)}+\cdots+a_{n-1}Y_c'+a_nY_c)
+(a_0Y_p^{(n)}+a_1Y_p^{(n-1)}+\cdots+a_{n-1}Y_p'+a_nY_p)=b(x)
```

como vemos los términos encerrados en el primer paréntesis representan

## Página 22

$`\phi[D]Y_c=0`$, mientras que los del segundo $`\phi[D]Y_p=b(x)`$ por lo que
$`Y_g`$ es una solución general de la ecuación (1).

Sabemos que $`Y_c`$ es la función solución de la ecuación complementaria u
homogénea que se obtiene de la ecuación (1) haciendo $`b(x)=0`$ por lo tanto el
problema se reduce a encontrar una “solución particular” $`Y_p`$, para lo cual
existen diferentes métodos.

### Método de los Coeficientes Indeterminados

Este método se puede aplicar a la ecuación diferencial

```math
\phi[D]y=b(x)
```

en los casos que $`b(x)`$ contiene un polinomio, términos de forma
$`\mathop{\mathrm{sen}}\nolimits px,\cos px;\ e^{px}`$ siendo $`p`$ una
constante, o bién, combinaciones de sumas y productos de estos términos. Para
facilitar la comprensión del método, nos plantearemos problemas prácticos para
su discusión, en los que mantendremos inalterable el primer miembro, por
simplicidad.

### I. Caso en que b(x) tenga forma polinómica de grado n

```math
y''+y'-6y=x^2+3x
```

utilizando simbología de operador:

```math
(D^2+D-6)y=x^2+3x
```

Sabemos que $`Y_c`$ es la solución de la ecuación complementaria definida por:

```math
(D^2+D-6)y=0\quad\text{ó}\quad y''+y'-6y=0
```

de donde $`Y_c=C_1e^{2x}+C_2e^{-3x}\Rightarrow(D^2+D-6)Y_c=0`$.

Para hallar una solución particular, nos preguntaremos: ¿qué función de una
variable independiente dará un polinomio al tomar sus derivadas?

Es evidente, que los polinomios tienen por derivadas a polinomios. Propongamos
entonces que la solución sea un polinomio del mismo grado

```math
Y_p=Ax^2+Bx+C
```

completo en $`x`$, donde $`A`$, $`B`$, $`C`$ son coeficientes constantes a
determinar. Si es así, al reemplazar la supuesta solución y sus derivadas
respectivas, tendremos:

```math
Y_p=Ax^2+Bx+C;\quad Y_p'=2Ax+B;\quad Y_p''=2A
```

## Página 23

```math
2A+(2Ax+B)-6(Ax^2+Bx+C)=x^2+3x
```

operando:

```math
-6Ax^2+(2A-6B)x+(2A+B-6C)=x^2+3x
```

comparando los coeficientes de ambos miembros de potencias análogas de $`x`$
tendremos:

```math
-6A=1;\quad2A-6B=3;\quad2A+B-6C=0
```

y resolviendo:

```math
A=-\frac16;\quad B=-\frac59;\quad C=-\frac4{27}
\qquad Y_p=-\frac16x^2-\frac59x-\frac4{27}
```

En consecuencia, la solución general de la ecuación propuesta será:

```math
Y_g=Y_c+Y_p=C_1e^{2x}+C_2e^{-3x}-\frac16x^2-\frac59x-\frac4{27}
```

### II. Caso en que b(x) tenga forma trigonométrica

que puede expresarse bajo la forma $`\mathop{\mathrm{sen}}\nolimits px`$,
$`\cos px`$, ó la combinación de ambas:

Supongamos la ecuación

```math
y''+y'-6y=6\mathop{\mathrm{sen}}\nolimits 3x
```

sabemos por cálculo anterior que $`Y_c=C_1e^{2x}+C_2e^{-3x}`$. Para hallar
$`Y_p`$ nos preguntaremos qué funciones derivadas una vez, dos veces, etc. dan
la función $`\mathop{\mathrm{sen}}\nolimits 3x`$ ó
$`k\mathop{\mathrm{sen}}\nolimits 3x`$ (siendo $`k=`$ cte). Es evidente que los
términos $`\mathop{\mathrm{sen}}\nolimits 3x`$ ó $`\cos3x`$ lo darán, por lo
tanto podemos ensayar como solución particular

```math
Y_p=A\mathop{\mathrm{sen}}\nolimits 3x+B\cos3x
```

siendo $`A`$, $`B`$ constantes, resolviendo sus derivadas y reemplazando en la
ecuación tenemos:

```math
Y_p'=3A\cos3x-3B\mathop{\mathrm{sen}}\nolimits 3x
```

```math
Y_p''=-9A\mathop{\mathrm{sen}}\nolimits 3x-9B\cos3x
```

```math
(-9A\mathop{\mathrm{sen}}\nolimits 3x-9B\cos3x)+(3A\cos3x-3B\mathop{\mathrm{sen}}\nolimits 3x)
-6(A\mathop{\mathrm{sen}}\nolimits 3x+B\cos3x)=6\mathop{\mathrm{sen}}\nolimits 3x
```

```math
(-15A-3B)\mathop{\mathrm{sen}}\nolimits 3x+(-15B+3A)\cos3x=6\mathop{\mathrm{sen}}\nolimits 3x
```

comparando los coeficientes, resulta $`A=-5/8;\ B=-1/8`$, por lo tanto la
solución particular es:

```math
Y_p=-\frac58\mathop{\mathrm{sen}}\nolimits 3x-\frac{\cos3x}{8}
\Rightarrow Y_g=C_1e^{2x}+C_2e^{-3x}-\frac58\mathop{\mathrm{sen}}\nolimits 3x-\frac{\cos3x}{8}
```

En el caso de funciones trigonométricas como la resuelta, pueden presentarse
algunos casos muy particulares en lo que la ecuación complementaria tenga raíces
complejas que una vez llevadas a su forma general real contenga en alguno de sus
términos la función $`b(x)`$.

## Página 25 — PDF 26

> Nota editorial: el original coloca la hoja impresa 25 antes de la 24. Se
> conserva este orden físico.

Debemos decidir, qué forma supondremos la solución particular.

Veamos: por el término $`2\cos2x`$, supondremos
$`A\mathop{\mathrm{sen}}\nolimits 2x+B\cos2x`$ por el término $`3x+2`$ el
polinomio de primer grado $`Cx+D`$, por el término $`6e^x`$ proponemos $`ke^x`$
por lo que la forma propuesta:

```math
Y_p=A\mathop{\mathrm{sen}}\nolimits 2x+B\cos2x+Cx+D+ke^x
```

basándonos en las propiedades operacionales de las derivadas de funciones, es
posible plantear soluciones en forma separadas:

```math
Y_{p_1}=A\mathop{\mathrm{sen}}\nolimits 2x+B\cos2x
```

```math
Y_{p_2}=Cx+D
```

```math
Y_{p_3}=ke^x
```

operar por separado cada una en forma aislada, resolver sus constantes y luego
hacer $`Y_p=Y_{p_1}+Y_{p_2}+Y_{p_3}`$, u operar con la función $`Y_p`$ y sus
derivadas sucesivas, como en los problemas anteriores ya resueltos. Supongamos
entonces:

```math
Y_p=A\mathop{\mathrm{sen}}\nolimits 2x+B\cos2x+Cx+D+ke^x
```

```math
Y_p'=2A\cos2x-2B\mathop{\mathrm{sen}}\nolimits 2x+C+ke^x
```

```math
Y_p''=-4A\mathop{\mathrm{sen}}\nolimits 2x-4B\cos2x+ke^x
```

reemplazando en la ecuación

```math
(-4A\mathop{\mathrm{sen}}\nolimits 2x-4B\cos2x+ke^x)
+(2A\cos2x-2B\mathop{\mathrm{sen}}\nolimits 2x+C+ke^x)
-6(A\mathop{\mathrm{sen}}\nolimits 2x+B\cos2x+Cx+D+ke^x)
=2\cos2x+3x+2+6e^x
```

operando en el primer miembro y comparando los coeficientes:

```math
A=\frac1{26};\quad B=\frac5{26};\quad C=\frac12;
\quad D=-\frac14;\quad k=\frac32
```

```math
Y_p=\frac1{26}\mathop{\mathrm{sen}}\nolimits 2x+\frac5{26}\cos2x
+\frac x2-\frac14+\frac32e^x
```

solución particular.

La solución general será $`Y_g=Y_c+Y_p`$

```math
Y_g=C_1e^{2x}+C_2e^{-3x}+\frac{\mathop{\mathrm{sen}}\nolimits 2x}{26}
+\frac5{26}\cos2x+\frac x2-\frac14+\frac{3e^x}{2}
```

Este método de los coeficientes indeterminados si bién lo hemos demostrado y
aplicado a las ecuaciones diferenciales de segundo orden a coeficientes
constantes general completas, el método se aplica

## Página 24 — PDF 27

en este caso no será válido proponer una solución complementaria “a menos de una
constante”, propondremos como caso de excepción la solución particular
$`Y_p=x(A\mathop{\mathrm{sen}}\nolimits px+B\cos px)`$ y seguiremos el mismo
procedimiento descripto para el caso anterior.

### III. Caso en que b(x) tenga forma exponencial del tipo Aeᵖˣ

Supongamos la ecuación $`y''+y'-6y=4e^{3x}`$, vimos que la solución
complementaria:

```math
Y_c=C_1e^{2x}+C_2e^{-3x}
```

Para hallar una solución particular nos preguntaremos, ¿qué función tiene por
derivadas a la función $`e^{3x}`$? Como sabemos una función del tipo $`ke^{3x}`$
satisface nuestras exigencias por lo que podríamos proponerla como posible
solución:

```math
Y_p=ke^{3x}\Rightarrow Y_p'=3ke^{3x}\qquad Y_p''=9ke^{3x}
```

reemplazando: $`(9ke^{3x})+(3ke^{3x})-6(ke^{3x})=4e^{3x}`$ operando tendremos:

```math
6ke^{3x}=4e^{3x}\Rightarrow k=\frac23\quad\therefore\quad Y_p=\frac23e^{3x}
```

```math
Y_g=C_1e^{2x}+C_2e^{-3x}+\frac23e^{3x}
```

solución general buscada.

En este caso también se puede presentar una excepción al método, que queda
establecida cuando la solución complementaria de tipo exponencial contenga a la
función del segundo miembro a menos de una constante, en dicho caso propondremos
$`Y_p=kxe^{px}`$ operando luego de la misma forma que en el caso anterior.

Si en particular la solución $`Y_c`$ es de la forma $`Y_c=(C_1+C_2x)e^{px}`$
solución ésta en el caso de raíces reales múltiples adoptaremos

```math
Y_p=kx^2e^{px}
```

y operamos como los anteriores.

### IV. Caso en que b(x) presenta una combinación lineal

de las funciones resueltas en los puntos anteriores y que representa la forma
más general que podemos abordar con este método.

Supongamos la ecuación:

```math
y''+y'-6y=2\cos2x+3x+2+6e^x
```

La solución complementaria: $`Y_c=C_1e^{2x}+C_2e^{-3x}`$ ya calculada.

## Página 26

de la misma forma con las mismas excepciones a ecuaciones diferenciales de orden
$`n>2`$.

### MÉTODO DE LAGRANGE (o de Variación de Parámetros)

Este método permite resolver ecuaciones diferenciales lineales de segundo orden
de forma: $`y''+a_1y'+a_2y=b(x)`$, con $`a_0,a_1,a_2`$ constantes, o sea:

```math
[D^2+a_1D+a_2]y=b(x)\Rightarrow\phi[D]y=b(x)
```

Como primer paso se calcula la solución de la ecuación diferencial
complementaria $`\phi[D]y=0`$, que ya sabemos resolver. Supongamos que
$`Y_c=C_1\phi_1+C_2\phi_2`$ es una solución, por lo tanto:

```math
\phi[D]Y_c=0
```

El método consiste, a diferencia del anterior, en obtener una solución
particular $`Y_p`$ a partir de la solución complementaria ya calculada
previamente, de la siguiente manera:

si $`Y_c=C_1\phi_1+C_2\phi_2`$ se reemplaza las constantes $`C_1`$ y $`C_2`$ por
los coeficientes a determinar que son “funciones de variable $`x`$”, adoptando
una $`Y_p=A(x)\phi_1+B(x)\phi_2`$, que si es solución de la ecuación dada:
$`\phi[D]Y_p=b(x)`$, por lo que procederemos a derivarla sucesivamente y
reemplazarla, observando que $`\phi_1`$ y $`\phi_2`$ son funciones de $`x`$ y
que las incógnitas son funciones de $`A(x)`$ y $`B(x)`$, así:

```math
Y_p=A(x)\phi_1+B(x)\phi_2
```

```math
Y_p'=A'(x)\phi_1+B'(x)\phi_2+A(x)\phi_1'+B(x)\phi_2'
```

Imponemos la condición que

```math
A'(x)\phi_1+B'(x)\phi_2=0\tag{1}
```

```math
Y_p'=A(x)\phi_1'+B(x)\phi_2'
```

derivando nuevamente

```math
Y_p''=A'(x)\phi_1'+B'(x)\phi_2'+A(x)\phi_1''+B(x)\phi_2''
```

reemplazando:

```math
Y_p''+a_1Y_p'+a_2Y_p=b(x)
```

## Página 27

```math
\begin{aligned}
&A(x)\phi_1''+B(x)\phi_2''+A'(x)\phi_1'+B'(x)\phi_2'\\
&\quad+A(x)a_1\phi_1'+B(x)a_1\phi_2'\\
&\quad+A(x)a_2\phi_1+B(x)a_2\phi_2
\end{aligned}
```

```math
A(x)(\phi_1''+a_1\phi_1'+a_2\phi_1)
+B(x)(\phi_2''+a_1\phi_2'+a_2\phi_2)
+A'(x)\phi_1'+B'(x)\phi_2'=b(x)
```

como $`\phi_1`$ y $`\phi_2`$ son soluciones de la ecuación complementaria será:

```math
\phi[D]\phi_1=0\qquad\phi[D]\phi_2=0
```

por lo tanto nos queda:

```math
A'(x)\phi_1'+B'(x)\phi_2'=b(x)\tag{2}
```

Se forma un sistema de ecuaciones a resolver:

```math
\begin{cases}
(1)\quad A'(x)\phi_1+B'(x)\phi_2=0\\
(2)\quad A'(x)\phi_1'+B'(x)\phi_2'=b(x)
\end{cases}
```

sistema éste donde $`A'(x)\land B'(x)`$ son las incógnitas, operando, el
determinante principal, será

```math
W(\phi_1,\phi_2)=\begin{vmatrix}\phi_1&\phi_2\\\phi_1'&\phi_2'\end{vmatrix}\ne0
```

ya que $`\phi_1`$ y $`\phi_2`$ son linealmente independientes, por lo que el
sistema tendrá solución.

```math
A'(x)=\frac{\begin{vmatrix}0&\phi_2\\b(x)&\phi_2'\end{vmatrix}}{W(\phi_1,\phi_2)}
=-\frac{b(x)\phi_2}{W(\phi_1,\phi_2)}
\Rightarrow A(x)=-\int\frac{b(x)\phi_2}{W(\phi_1,\phi_2)}\,dx
```

```math
B'(x)=\frac{\begin{vmatrix}\phi_1&0\\\phi_1'&b(x)\end{vmatrix}}{W(\phi_1,\phi_2)}
=\frac{b(x)\phi_1}{W(\phi_1,\phi_2)}
\Rightarrow B(x)=\int\frac{b(x)\phi_1}{W(\phi_1,\phi_2)}\,dx
```

conocido los valores de $`A(x)`$ y $`B(x)`$, tendremos $`Y_p`$.

```math
Y_p=-\phi_1\int\frac{b(x)\phi_2}{W(\phi_1,\phi_2)}\,dx
+\phi_2\int\frac{b(x)\phi_1}{W(\phi_1,\phi_2)}\,dx
```

La solución general será: $`Y_g=Y_c+Y_p`$, como en casos anteriores.

## Página 28

Ejemplo práctico de aplicación del método descripto:

Supongamos la ecuación $`y''+y'-6y=\cos x`$.

Calculamos $`Y_c=C_1e^{2x}+C_2e^{-3x}`$ o sea $`\phi_1=e^{2x}`$,
$`\phi_2=e^{-3x}`$.

Proponemos como posible solución particular a la función:

```math
Y_p=A(x)\phi_1+B(x)\phi_2=A(x)e^{2x}+B(x)e^{-3x}
```

calculamos primero

```math
W(\phi_1,\phi_2)=\begin{vmatrix}e^{2x}&e^{-3x}\\2e^{2x}&-3e^{-3x}\end{vmatrix}
=-3e^{-x}-2e^{-x}=-5e^{-x}
```

luego calculamos las funciones $`A(x)`$ y $`B(x)`$ mediante:

```math
A(x)=-\int\frac{b(x)\phi_2}{W(\phi_1,\phi_2)}\,dx
=-\int\frac{\cos x\,e^{-3x}}{-5e^{-x}}\,dx
=\int\frac{\cos x}{5e^{2x}}\,dx
```

```math
B(x)=\int\frac{b(x)\phi_1}{W(\phi_1,\phi_2)}\,dx
=\int\frac{\cos x\,e^{2x}}{-5e^{-x}}\,dx
=\int-\frac{\cos x\,e^{3x}}5\,dx
```

resolviendo las integrales planteadas, obtendremos reemplazando la solución
buscada. Si bién el método se describió para una ecuación de segundo orden, éste
se generaliza y aplicó a un orden “$`n`$”.

### Resolución de Ecuaciones Diferenciales mediante el empleo de Series

Hasta ahora solamente hemos tratado ecuaciones diferenciales que podían
resolverse en forma “exacta”, o dicho de otra manera la integral general o
solución era una función elemental, del tipo algebraica, trigonométrica,
exponencial, logarítmica, etc.

Sin embargo, hay ecuaciones diferenciales de extraordinaria importancia en
distintas disciplinas, cuya solución no está en el campo de las funciones
elementales y que no pueden resolverse exactamente por ningún método (en muchos
casos tampoco interesa su cálculo “exacto”).
