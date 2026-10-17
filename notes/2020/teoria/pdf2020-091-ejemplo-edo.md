<!-- markdownlint-disable MD036 -->

# Ejemplo EDO

> Título editorial tomado del archivo `2020/15-EDO 2do Orden/Ejemplo EDO.pdf`.
> Transcripción del manuscrito de la página 1 de 1; no consta autor ni año
> impreso. Controles en
> [cobertura](../../../resources/2020/pdf2020-cobertura.md).

Resolver $`y''+3y'+5y=0`$ sujeto a condiciones $`y(0)=0`$; $`y'(0)=1`$.

```math
m^2+3m+5=0
```

```math
-\frac32+\frac{\sqrt{3^2-4\cdot5}}2
=-\frac32+\frac{\sqrt{9-20}}2
=-\frac32+i\frac{\sqrt{20-9}}2
=-\frac32+i\frac{\sqrt{11}}2
```

```math
-\frac32-\frac{\sqrt{3^2-4\cdot5}}2
=-\frac32-i\frac{\sqrt{11}}2
```

Solución

```math
y(x)=C_1e^{-\frac32x}\cos\left(\frac{\sqrt{11}}2x\right)
+C_2e^{-\frac32x}\mathop{\mathrm{sen}}\nolimits \left(\frac{\sqrt{11}}2x\right)
```

Determinación de coeficientes $`C_1`$ y $`C_2`$.

```math
y(0)=C_1e^0\cos0+C_2e^0\mathop{\mathrm{sen}}\nolimits 0=C_1=0
```

```math
\begin{aligned}
y'(x)={}&-\frac32C_1e^{-\frac32x}\cos\left(\frac{\sqrt{11}}2x\right)
-C_1e^{-\frac32x}\frac{\sqrt{11}}2\mathop{\mathrm{sen}}\nolimits \left(\frac{\sqrt{11}}2x\right)\\
&-\frac32C_2e^{-\frac32x}\mathop{\mathrm{sen}}\nolimits \left(\frac{\sqrt{11}}2x\right)
+C_2e^{-\frac32x}\frac{\sqrt{11}}2\cos\left(\frac{\sqrt{11}}2x\right)
\end{aligned}
```

```math
y'(0)=-\frac32C_1e^0\cos0-\frac{\sqrt{11}}2C_1e^0\mathop{\mathrm{sen}}\nolimits 0
-\frac32C_2e^0\mathop{\mathrm{sen}}\nolimits 0+C_2e^0\frac{\sqrt{11}}2\cos0=1
```

```math
C_1=0;\quad C_2\frac{\sqrt{11}}2=1\Rightarrow C_2=\frac2{\sqrt{11}}
```

```math
y(x)=\frac2{\sqrt{11}}e^{-\frac32x}\mathop{\mathrm{sen}}\nolimits \left(\frac{\sqrt{11}}2x\right)
```

Si sustituimos $`y(x)`$ en $`y''+3y'+5y=0`$ deberá verificar la identidad.

Queda por cuenta del alumno verificar.

*Scanned by CamScanner*
