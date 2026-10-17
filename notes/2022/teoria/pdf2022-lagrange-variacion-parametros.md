# Lagrange — método de Variación de Parámetros

> Fuente: `2022 [Intensivo]/IMG-20221118-WA0008.jpg`. Archivo de 2022; sin año
> impreso. Procedencia y controles en
> [cobertura PDF 2022](../../../resources/2022/pdf2022-cobertura.md).

Lo aplicamos si $g(x)$ es una función que tiene cierta complejidad.

Si:

$$
ay''+by'+cy=g(x),
$$

donde $a$, $b$ y $c$ son de $\mathbb R$ no simultáneamente nulas.

$$
Y_G=Y_C+Y_P\Rightarrow Y_C=C_1\phi_1+C_2\phi_2.
$$

Lagrange propone que $Y_P=A(x)\phi_1+B(x)\phi_2$, con lo que se deben calcular
$A(x)$ y $B(x)$, resolviendo el siguiente sistema de ecuaciones:

$$
\begin{cases}
A'(x)\phi_1+B'(x)\phi_2=0,\\
A'(x)\phi'_1+B'(x)\phi'_2=g(x).
\end{cases}
$$

Donde $A'(x)$ y $B'(x)$ son las incógnitas.

Wroskiano:

$$
W(\phi_1,\phi_2)=\begin{vmatrix}\phi_1&\phi_2\\\phi'_1&\phi'_2\end{vmatrix}\ne0.
$$

Así:

$$
A'(x)=\frac{\begin{vmatrix}0&\phi_2\\g(x)&\phi'_2\end{vmatrix}}{W(\phi_1,\phi_2)}
=-\frac{g(x)\phi_2}{W(\phi_1,\phi_2)}
\Rightarrow A(x)=-\int\frac{g(x)\phi_2}{W(\phi_1,\phi_2)}\,dx.
$$

$$
B'(x)=\frac{\begin{vmatrix}\phi_1&0\\\phi'_1&g(x)\end{vmatrix}}{W(\phi_1,\phi_2)}
=\frac{g(x)\phi_1}{W(\phi_1,\phi_2)}
\Rightarrow B(x)=\int\frac{g(x)\phi_1}{W(\phi_1,\phi_2)}\,dx.
$$

$$
Y_P=-\phi_1\int\frac{g(x)\phi_2}{W(\phi_1,\phi_2)}\,dx
+\phi_2\int\frac{g(x)\phi_1}{W(\phi_1,\phi_2)}\,dx.
$$

$$
Y_G=Y_P+Y_C.
$$

$$
\boxed{Y_G=C_1\phi_1+C_2\phi_2-\phi_1\int\frac{g(x)\phi_2}{W(\phi_1,\phi_2)}\,dx
+\phi_2\int\frac{g(x)\phi_1}{W(\phi_1,\phi_2)}\,dx.}
$$

Nota de transcripción: se conserva «Wroskiano» y la aparición de $g(x)$ sin
normalizar por $a$ del manuscrito; no se corrige silenciosamente.

[Fotografía original](../../../resources/2022/pdf2022-lagrange-original.jpg).
