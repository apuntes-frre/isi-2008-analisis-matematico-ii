<!-- markdownlint-disable MD036 -->

# Ejemplo 3

> Título editorial tomado del archivo `2020/15-EDO 2do Orden/Ejemplo 3.pdf`.
> Transcripción del manuscrito de la página 1 de 1; no consta autor ni año
> impreso. Controles en
> [cobertura](../../../resources/2020/pdf2020-cobertura.md).

$$
y''+3y'+2y=2e^{-2x}
$$

Vimos que la solución es $y(x)=C_1e^{-x}+C_2e^{-2x}-2xe^{-2x}$ sin considerar
los valores de $C_1$ y $C_2$.

La solución característica es

$$
y_c(x)=C_1e^{-x}+C_2e^{-2x}=C_1\phi_1(x)+C_2\phi_2(x)\qquad(*)
$$

Si consideramos el método de Lagrange:

$$
\phi_1=e^{-x}\quad\phi_1'=-e^{-x}\quad
\phi_2=e^{-2x}\quad\phi_2'=-2e^{-2x}
$$

1. Resolvimos

$$
\begin{cases}
C_1'(x)\phi_1+C_2'(x)\phi_2=0\\
C_1'(x)\phi_1'+C_2'(x)\phi_2'=2e^{-2x}
\end{cases}
$$

Siendo la solución $y(x)=C_1(x)\phi_1(x)+C_2(x)\phi_2(x)$.

Notar que sustituimos a la constante $C_1$ y $C_2$ de $(*)$ por $C_1(x)$ y
$C_2(x)$ y en el sistema de ecuaciones aparecen sus derivadas.

$$
\begin{aligned}
C_1'(x)
&=\frac{\begin{vmatrix}0&\phi_2\\2e^{-2x}&\phi_2'\end{vmatrix}}
{\begin{vmatrix}\phi_1&\phi_2\\\phi_1'&\phi_2'\end{vmatrix}}\\
&=\frac{-\phi_2\,2e^{-2x}}{e^{-x}(-2)e^{-2x}-(-e^{-x})e^{-2x}}\\
&=\frac{-2e^{-2x}e^{-2x}}{-2e^{-3x}+e^{-3x}}
=\frac{-2e^{-2x}e^{-2x}}{-e^{-3x}}
=2e^{-4x}e^{3x}=2e^{-x}
\end{aligned}
$$

$$
C_1'(x)=2e^{-x}
$$

$$
C_2'(x)=\frac{\begin{vmatrix}\phi_1&0\\\phi_1'&2e^{-2x}\end{vmatrix}}{-e^{-3x}}
=\frac{2e^{-2x}e^{-x}}{-e^{-3x}}
=-2e^{-3x}e^{3x}=-2;\quad C_2'(x)=-2
$$

$$
C_1'(x)=2e^{-x}\Rightarrow C_1(x)=-2e^{-x}+K_1
$$

$$
C_2'(x)=-2\Rightarrow C_2(x)=-2x+K_2;\quad K_1\text{ y }K_2\text{ ctes.}
$$

$$
\begin{aligned}
y(x)&=C_1(x)\phi_1(x)+C_2(x)\phi_2(x)\\
&=(-2e^{-x}+K_1)e^{-x}+(-2x+K_2)e^{-2x}\\
&=-2e^{-x}e^{-x}+K_1e^{-x}-2xe^{-2x}+K_2e^{-2x}\\
&=K_1e^{-x}+K_2e^{-2x}-2e^{-2x}-2xe^{-2x}\\
&=K_1e^{-x}+(K_2-2)e^{-2x}-2xe^{-2x}
\end{aligned}
$$

Notar que $K_2-2$ es una constante no determinada aún por lo tanto con $K_1=M_1$
y $K_2-2=M_2$.

$$
y(x)=M_1e^{-x}+M_2e^{-2x}-2xe^{-2x}
$$

Solución idéntica a la encontrada anteriormente.

*Scanned by CamScanner*
