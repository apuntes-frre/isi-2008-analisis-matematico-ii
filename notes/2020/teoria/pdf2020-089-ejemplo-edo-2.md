<!-- markdownlint-disable MD036 -->

# Ejemplo 2

> Título editorial tomado del archivo `2020/15-EDO 2do Orden/Ejemplo 2.pdf`.
> Transcripción del manuscrito de la página 1 de 1; no consta autor ni año
> impreso. Controles en
> [cobertura](../../../resources/2020/pdf2020-cobertura.md).

$$
y''+3y'+2y=2e^{-2x}
$$

Condiciones $y(0)=1$, $y(1)=1$.

$$
m^2+3m+2=0
$$

$$
-\frac32+\frac{\sqrt{9-4\cdot2}}2=-\frac32+\frac12=-1
$$

$$
-\frac32-\frac{\sqrt{9-4\cdot2}}2=-\frac32-\frac12=-2
$$

Solución característica

$$
y_c(x)=C_1e^{-x}+C_2e^{-2x}
$$

Solución particular, notar \[flecha hacia el término $e^{-2x}$\], es un caso que
se aparta de lo normal.

Solución propuesta

$$
y_p(x)=Kxe^{-2x}
$$

$$
y_p'(x)=-2Kxe^{-2x}+Ke^{-2x}
$$

$$
y_p''(x)=4Kxe^{-2x}-2Ke^{-2x}-2Ke^{-2x}
$$

$$
\begin{aligned}
y_p''+3y_p'+2y_p
&=4Kxe^{-2x}-2Ke^{-2x}-2Ke^{-2x}
-6Kxe^{-2x}+3Ke^{-2x}+2Kxe^{-2x}\\
&=-Ke^{-2x}=2e^{-2x}
\end{aligned}
$$

$$
\Rightarrow K=-2;\quad y_p(x)=-2xe^{-2x}
$$

Solución

$$
y(x)=C_1e^{-x}+C_2e^{-2x}-2xe^{-2x}
$$

Faltan definir $C_1$ y $C_2$.

$$
y(0)=C_1+C_2=1
$$

$$
y(1)=C_1e^{-1}+C_2e^{-2}-2e^{-2}=1
$$

De donde podemos obtener $C_1$ y $C_2$.

*Scanned by CamScanner*
