# Estrategias prácticas — Series de Fourier

Fuente: «Consideraciones sobre Series de Fourier.pdf», archivo de 2016, Arnaldo
César Flores. Transcripción de las páginas 1–5; página 6 vacía.
[Procedencia y revisión](../../../resources/2016/resume-teoria-cobertura.md).

## Página 1

La redacción de este artículo, de carácter breve, tiene como objetivo para el
que se inicia en el estudio de la serie de Fourier, encontrar una ayuda, con el
fin de evitar los cálculos para obtener los coeficientes de la serie de una
función dada, a partir de la serie conocida de otra función, suponiendo que se
presentan cambios de amplitud, fase y frecuencia entre ambas.

Arnaldo César Flores

Es $`f(x)`$ función desarrollable según la serie de Fourier, periódica o no, y
definida en el intervalo $`c\le x\le c+2L`$ con $`c,L\in\mathbb R`$, $`L\gt 0`$.

```math
f(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}(a_n\cos[n\omega x]+b_n\sin[n\omega x])
```

```math
\frac{a_0}{2}=\frac1{2L}\int_c^{c+2L}f(x)\,dx
```

```math
a_n=\frac1L\int_c^{c+2L}f(x)\cos(n\omega x)\,dx
```

```math
b_n=\frac1L\int_c^{c+2L}f(x)\sin(n\omega x)\,dx
```

```math
\omega=\frac{2\pi}{2L}
```

### Primer Caso: Corrimiento en el eje vertical

(Jerga técnica: sumamos una continua)

Sea $`g(x)`$ función desarrollable según la serie de Fourier, periódica o no, y
definida en el intervalo $`c\le x\le c+2L`$ con $`c,L\in\mathbb R`$, $`L\gt 0`$,
condiciones iguales a $`f(x)`$ y sea:

```math
g(x)=f(x)+k,\qquad k\in\mathbb R
```

```math
g(x)=\frac{a'_0}{2}+\sum_{n=1}^{\infty}(a'_n\cos[n\omega x]+b'_n\sin[n\omega x])
```

Los coeficientes de Fourier son:

```math
\begin{aligned}
\frac{a'_0}{2}&=\frac1{2L}\int_c^{c+2L}g(x)\,dx
=\frac1{2L}\int_c^{c+2L}(f(x)+k)\,dx\\
&=\frac1{2L}\int_c^{c+2L}f(x)\,dx+\frac1{2L}\int_c^{c+2L}k\,dx
=\frac1{2L}\int_c^{c+2L}f(x)\,dx+k
\end{aligned}
```

## Página 2

Decimos que el coeficiente $`\frac{a'_0}{2}`$ de la serie de $`g(x)`$, es igual
al coeficiente $`\frac{a_0}{2}`$ de la serie de $`f(x)`$, MÄS la constante
$`k`$.

```math
a'_0=a_0+k
```

Respecto del coeficiente $`a_n`$, decimos:

```math
\begin{aligned}
a'_n&=\frac1L\int_c^{c+2L}g(x)\cos(n\omega x)\,dx
=\frac1L\int_c^{c+2L}[f(x)+k]\cos(n\omega x)\,dx\\
&=\frac1L\int_c^{c+2L}f(x)\cos(n\omega x)\,dx
+\frac1L\int_c^{c+2L}k\cos(n\omega x)\,dx\\
&=\frac1L\int_c^{c+2L}f(x)\cos(n\omega x)\,dx
\end{aligned}
```

Con

```math
\frac1L\int_c^{c+2L}k\cos(n\omega x)\,dx=0,\qquad\forall n
```

Decimos que el coeficiente $`a'_n`$ de la serie de $`g(x)`$, es igual al
coeficiente $`a_n`$ de la serie de $`f(x)`$ e igualmente ocurre con $`b'_n`$.

```math
a'_n=a_n;\qquad b'_n=b_n
```

### Segundo Caso: Cambio de amplitud

Sea $`g(x)`$ función desarrollable según la serie de Fourier, periódica o no, y
definida en el intervalo $`c\le x\le c+2L`$ con $`c,L\in\mathbb R`$, $`L\gt 0`$,
condiciones iguales a $`f(x)`$ y sea:

```math
g(x)=hk\,f(x),\qquad h\in\mathbb R
```

```math
g(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}(a_n\cos[n\omega x]+b_n\sin[n\omega x])
=h\,f(x)=\frac{ha_0}{2}+\sum_{n=1}^{\infty}(ha_n\cos[n\omega x]+hb_n\sin[n\omega x])
```

Decimos que los coeficientes de la serie de Fourier de $`g(x)`$, son iguales a
los de $`f(x)`$, salvo la constante multiplicadora $`h`$.

```math
\frac{a'_0}{2}=\frac{ha_0}{2};\qquad a'_n=ha_n;\qquad b'_n=hb_n
```

### Tercer caso: generalización

El lector está en condiciones ahora de reconocer que el caso generalizado

```math
g(x)=h\,f(x)+k
```

Conduce a

## Página 3

```math
\frac{a'_0}{2}=\frac{ha_0}{2}+k;\qquad a'_n=ha_n;\qquad b'_n=hb_n
```

### Cuarto Caso: Corrimiento en el eje horizontal

(Jerga técnica: desfasamiento o ángulo de fase entre ambas, hay corrimiento
temporal, cuando la variable es tiempo)

Es $`f(x)`$ función desarrollable según la serie de Fourier, periódica o no, y
definida en el intervalo $`c\le x\le c+2L`$ con $`c,L\in\mathbb R`$, $`L\gt 0`$.

```math
f(x)=\frac{a_0}{2}+\sum_{n=1}^{\infty}(a_n\cos[n\omega x]+b_n\sin[n\omega x])
```

Es $`g(x')`$ función desarrollable según la serie de Fourier, periódica o no, y
definida en el intervalo $`c'\le x\le c'+2L`$ con $`c',L\in\mathbb R`$,
$`L\gt 0`$, $`c'\ne c`$.

La imagen de $`f(x)`$ es igual a la imagen de $`g(x')`$ pero difieren en el
intervalo de definición, no así, en su extensión $`2L`$, es común a ambas
funciones.

$`f(x)`$ y $`g(x')`$ tienen el mismo período y frecuencia, pero “arrancan en
lugares distintos” dado que $`c'\ne c`$.

Resulta $`x=x'-\delta`$.

Donde $`c'-c=\delta`$.

En razón de la semejanza, los coeficientes son iguales.

Por lo tanto “transformamos” a $`f(x)`$ en $`g(x')`$ cambiando la variable que
la define, y como conocemos el desarrollo de Fourier de $`f(x)`$, resulta:

```math
g(x')=\frac{a_0}{2}+\sum_{n=1}^{\infty}(a_n\cos[n\omega(x'-\delta)]+b_n\sin[n\omega(x'-\delta)])
```

```math
\cos[n\omega(x'-\delta)]=\cos n\omega x'\cos n\omega\delta+\sin n\omega x'\sin n\omega\delta
```

```math
\sin[n\omega(x'-\delta)]=\sin n\omega x'\sin n\omega\delta-\cos n\omega x'\cos n\omega\delta
```

```math
\begin{aligned}
&a_n\cos n\omega x'\cos n\omega\delta+a_n\sin n\omega x'\sin n\omega\delta
+b_n\sin n\omega x'\sin n\omega\delta-b_n\cos n\omega x'\cos n\omega\delta\\
&=(a_n-b_n)\cos n\omega x'\cos n\omega\delta+(a_n+b_n)\sin n\omega x'\sin n\omega\delta
\end{aligned}
```

## Página 4

```math
g(x')=\frac{a_0}{2}+\sum_{n=1}^{\infty}\left((a_n-b_n)\cos n\omega x'\cos n\omega\delta+(a_n+b_n)\sin n\omega x'\sin n\omega\delta\right)
```

### Quinto caso: cambio de escala en la variable

(Jerga técnica, cambio de frecuencia)

Se tiene el caso donde $`x'=mx`$ y por esta razón $`g(x')=g(mx)=f(x)`$.

El rango de cada función es igual, cambia el intervalo donde se define,
achicándose o agrandándose, en otras palabras, cambiamos la frecuencia.

Ejemplo:

Es $`f(x)`$ función desarrollable según la serie de Fourier, periódica o no, y
definida en el intervalo $`c\le x\le c+2L`$ con $`c,L\in\mathbb R`$, $`L\gt 0`$.

```math
f(x)=x;\qquad c=0;\qquad 2L=1
```

Sea $`g(x')`$ función desarrollable según la serie de Fourier, periódica o no, y
definida en el intervalo $`c'\le x\le c'+2L'`$ con $`c',L'\in\mathbb R`$,
$`L'\gt 0`$.

```math
g(x')=2x';\qquad c'=0;\qquad 2L'=0{,}5
```

El lector notará que la primer función en el intervalo [0,1] varía entre 0 y 1,
mientras que en la segunda ocurre exactamente lo mismo pero en el intervalo
[0,1/2].

Concretamente

```math
x'=0{,}5x
```

Una conveniente representación gráfica, elimina inconvenientes de
interpretación.

En otras palabras, si afectamos a la variable x de f(x) por un multiplicador
constante igual a 0,5, obtenemos g(x’).

Generalizando y siendo $`x'=mx`$.

Los coeficientes de una función $`f(x)`$, supuestamente conocidos, por ejemplo:

```math
\frac{a_0}{2}=\frac1{2L}\int_c^{c+2L}f(x)\,dx
```

Al ser considerado un cambio de escala y multiplicado x por la constante m,
resulta necesario, en la formulación cambiar las escalas en todos los factores
intervinientes:

```math
\frac{a_0}{2}=\frac1{2mL}\int_{mc}^{m(c+2L)}f(mx)\,(m\,dx)
=\frac1{2L'}\int_{c'}^{c'+2L'}g(x')\,dx'
```

Lo que en palabras resulta expresado: el coeficiente constante de ambas series
de Fourier, tanto de $`f(x)`$

Como de $`g(x')`$ son IGUALES.

## Página 5

En el coeficiente:

```math
a_n=\frac1L\int_c^{c+2L}f(x)\cos(n\omega x)\,dx
```

Al ser considerado un cambio de escala y multiplicado x por la constante m,
resulta necesario, en la formulación cambiar las escalas en todos los factores
intervinientes:

```math
a_n=\frac1{mL}\int_{mc}^{m(c+2L)}f(mx)\cos\left(\frac{n2\pi}{2mL}mx\right)m\,dx
=a_n=\frac1{L'}\int_{c'}^{c'+2L'}g(x')\cos(n\omega'x')\,dx'
```

Lo que en palabras resulta expresado: el coeficiente $`a_n`$ de ambas series de
Fourier, tanto de $`f(x)`$

Como de $`g(x')`$ son IGUALES.

Lo mismo ocurre con $`b_n`$.

Y el desarrollo resultante será:

```math
g(x')=\frac{a_0}{2}+\sum_{n=1}^{\infty}(a_n\cos[n\omega'x']+b_n\sin[n\omega'x'])
```

```math
\omega'=\frac{2\pi}{2L'}
```

Dos funciones que difieran en frecuencia, únicamente, tendrán los coeficientes
de sus armónicos iguales, de igual manera, sus términos constantes.

## Observaciones de transcripción

Se conserva la notación y las expresiones del original, incluidas las
inconsistencias: en la página 2 figura $`a'_0=a_0+k`$ y $`g(x)=hkf(x)`$; en las
páginas 3–4 se conserva la identidad de seno y su desarrollo tal como aparecen.
No se han corregido sus resultados matemáticos.

La página 6 solo contiene un borde superior, sin texto ni figuras.
