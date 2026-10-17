<!-- markdownlint-disable MD060 -->

# Hoja de ruta para el práctico 6

> Fuente: `2022 [Intensivo]/CamScanner 11-15-2022 18.24.pdf`. Archivo de 2022;
> sin año impreso. Procedencia y controles en
> [cobertura PDF 2022](../../../resources/2022/documentos-pdf-cobertura.md).

UNIVERSIDAD TECNOLOGICA NACIONAL — FACULTAD REGIONAL RESISTENCIA.

GUÍA DE TRABAJOS PRÁCTICOS — ANÁLISIS MATEMÁTICO II.

## Página 1

**10.** Si la ecuación auxiliar $`ar^2+br+c=0`$ tiene sólo una raíz real $`r`$,
por lo tanto la solución general de $`ay''+by'+cy=0`$ es

```math
y=c_1e^{rx}+c_2xe^{rx}.
```

**11.** Si las raíces de la ecuación auxiliar $`ar^2+br+c=0`$ son números
complejos $`r_1=\alpha+i\beta`$, $`r_2=\alpha-i\beta`$, en consecuencia la
solución general de $`ay''+by'+cy=0`$ es

```math
y=e^{\alpha x}(c_1\cos\beta x+c_2\mathop{\mathrm{sen}}\nolimits \beta x).
```

**RESUMEN: SOLUCIONES DE $`ay''+by'+c=0`$**

| Raíces de $`ar^2+br+c=0`$ | Solución general |
| -- | -- |
| $`r_1`$, $`r_2`$ reales y distintas | $`y=c_1e^{r_1x}+c_2e^{r_2x}`$ |
| $`r_1=r_2=r`$ | $`y=c_1e^{rx}+c_2xe^{rx}`$ |
| $`r_1`$, $`r_2`$ complejas: $`\alpha\pm i\beta`$ | $`y=e^{\alpha x}(c_1\cos\beta x+c_2\mathop{\mathrm{sen}}\nolimits \beta x)`$ |

### ECUACIONES LINEALES NO HOMOGÉNEAS

En esta sección se aprende cómo resolver ecuaciones diferenciales lineales de
segundo orden no homogéneas con coeficientes constantes, es decir, ecuaciones de
la forma

```math
ay''+by'+cy=G(x)\qquad(1)
```

donde $`a`$, $`b`$ y $`c`$ son constantes y $`G`$ es una función continua. La
ecuación homogénea relacionada

```math
ay''+by'+cy=0\qquad(2)
```

se llama **ecuación complementaria** y juega un papel importante en la solución
de la ecuación no homogénea original (1).

**3 TEOREMA** La solución general de la ecuación diferencial no homogénea (1) se
puede escribir como

```math
y(x)=y_P(x)+y_C(x)
```

donde $`y_P`$ es una solución particular de la ecuación 1 y $`y_C`$ es la
solución general de la ecuación complementaria 2.

## Página 2

UNIVERSIDAD TECNOLOGICA NACIONAL — FACULTAD REGIONAL RESISTENCIA.

GUÍA DE TRABAJOS PRÁCTICOS — ANÁLISIS MATEMÁTICO II.

HOJA DE RUTA PARA EL PRÁCTICO 6.

### RESUMEN DEL MÉTODO DE COEFICIENTES INDETERMINADOS

1. Si $`G(x)=e^{kx}P(x)`$, donde $`P`$ es un polinomio de grado $`n`$, en
   seguida intente $`y_P(x)=e^{kx}Q(x)`$, donde $`Q(x)`$ es un polinomio de
   n-ésimo grado (cuyos coeficientes están determinados por sustitución en la
   ecuación diferencial).

1. Si $`G(x)=e^{kx}P(x)\cos mx`$ o si
   $`G(x)=e^{kx}P(x)\mathop{\mathrm{sen}}\nolimits mx`$, donde $`P`$ es un
   polinomio de n-ésimo grado, en tal caso intente

   $`\displaystyle y_P(x)=e^{kx}Q(x)\cos mx+e^{kx}R(x)\mathop{\mathrm{sen}}\nolimits mx`$

   donde $`Q`$ y $`R`$ son polinomios de n-ésimo grado.

**Modificación:** Si cualquier término de $`y_P`$ es una solución de la ecuación
complementaria, multiplique $`y_P`$ por $`x`$ (o por $`x^2`$ si es necesario).

| $`r(x)`$ |  | $`y_1`$ |
| -- | -- | -- |
| $`x^n`$ | $`0`$ | $`a_nx^n+\cdots+a_2x^2+a_1x+a_0`$ |
| $`e^{\alpha x}`$ | $`\alpha`$ | $`ae^{\alpha x}`$ |
| $`\cos\beta x`$ | $`\alpha+\beta i`$ | $`a\cos\beta x+b\mathop{\mathrm{sen}}\nolimits \beta x`$ |
| $`\mathop{\mathrm{sen}}\nolimits \beta x`$ | $`\alpha+\beta i`$ | $`a\cos\beta x+b\mathop{\mathrm{sen}}\nolimits \beta x`$ |
| $`x^ne^{\alpha x}`$ | $`\alpha`$ | $`e^{\alpha x}(a_nx^n+\cdots+a_1x+a_0)`$ |
| $`e^{\alpha x}\mathop{\mathrm{sen}}\nolimits \beta x`$ | $`\alpha+\beta i`$ | $`e^{\alpha x}(a\cos\beta x+b\mathop{\mathrm{sen}}\nolimits \beta x)`$ |
| $`e^{\alpha x}\cos\beta x`$ | $`\alpha+\beta i`$ | $`e^{\alpha x}(a\cos\beta x+b\mathop{\mathrm{sen}}\nolimits \beta x)`$ |
| $`x^ne^{\alpha x}\mathop{\mathrm{sen}}\nolimits \beta x`$ | $`\alpha+\beta i`$ | $`e^{\alpha x}\cos\beta x(a_nx^n+\cdots+a_1x+a_0)+e^{\alpha x}\mathop{\mathrm{sen}}\nolimits \beta x(b_nx^n+\cdots+a_1x+a_0)`$ |

## Página 3 — manuscrito

Para el método de coeficientes indeterminados.

```math
Y_G=Y_P+Y_C.
```

Si:

```math
g(x)=x^2\Rightarrow y_P(x)=Ax^2+Bx+C.
```

```math
g(x)=e^{3x}\Rightarrow y_P(x)=Ae^{3x}.
```

```math
g(x)=\mathop{\mathrm{sen}}\nolimits x\Rightarrow y_P(x)=A\cos Kx+B\mathop{\mathrm{sen}}\nolimits Kx.
```

```math
g(x)=xe^x+\cos2x\Rightarrow
\begin{cases}
y_{(P_1)}(x)=(Ax+B)e^x,\\
y_{(P_2)}(x)=C\cos2x+D\mathop{\mathrm{sen}}\nolimits 2x.
\end{cases}
```

- $`g(x)=x\Rightarrow y_P(x)=Ax+B`$.
- $`g(x)=\cos x\Rightarrow y_P(x)=A\mathop{\mathrm{sen}}\nolimits x+B\cos x`$.
- $`g(x)=e^{2x}+x^2\Rightarrow y_P(x)=Ke^{2x}+Ax^2+Bx+C`$.
- $`g(x)=e^x+\cos x+x\Rightarrow y_P(x)=Ke^x+A\mathop{\mathrm{sen}}\nolimits x+B\cos x+Cx+D`$.
- $`g(x)=1+5\cos x\Rightarrow y_P(x)=C+A\mathop{\mathrm{sen}}\nolimits x+B\cos x`$.

## Página 4 — Ejercicios

1. $`\frac{d^2y}{dx^2}+\frac{dy}{dx}=0`$.

1. $`y''+2y'-3y=0`$.

1. $`y''+y=0`$.

1. $`y''+y'-2y=0`$.

1. $`y''-2y'+2y=0`$.

1. $`4y''+12y'+9y=0`$, $`y(0)=4`$, $`y'(0)=-3`$.

   Anotación adicional con llave: $`y(0)=4`$, $`y(0)=0`$, $`y(0)=-4`$, con
   $`y'(0)=-3`$.

1. $`9y''+6y'+325y=0`$, $`y(0)=12`$, $`y'(0)=50`$.

1. Hallar la solución particular de la ecuación diferencial $`y''-6y+9y=0`$ que
   pasa por el punto $`(x_0,y_0)=(0,1)`$ con $`y'(0)=0`$.

1. Dada la ecuación diferencial $`y''-2y'+5y=0`$ se pide:

   a) La solución general.

   b) La solución particular que pasa por $`(x_0,y_0)=(0,2)`$ con $`y'(0)=1`$.

## Página 5 — método de los coeficientes indeterminados

1. $`y''-4y=e^x`$.
1. $`y''-y=x`$.
1. $`y''-2y'+y=2e^{2x}`$.
1. $`y''-4y=\cos x`$.
1. $`y''+4y'+3y=1+5\cos x`$.
1. $`y''-y'=x^2`$.
1. $`y''+y=\mathop{\mathrm{sen}}\nolimits x`$.
1. Dada la ecuación diferencial $`y''-3y'+2y=8x`$ hallar la solución particular
   que en el punto $`(0,y_0)`$ tiene recta tangente con la ecuación $`y=6x+8`$.
1. Hallar la ecuación cartesiana de la curva solución de $`y''-y=4e^x`$ que pasa
   por el origen de coordenadas con pendiente 2 en dicho punto.

Scanned with CamScanner (pie presente en las cinco páginas).

## Notas de transcripción

Se conservan las particularidades del original: el título del resumen de la
página 1 omite $`y`$ después de $`c`$; la segunda columna de la tabla de la
página 2 no tiene encabezado y las filas de seno/coseno incluyen $`\alpha`$; el
último polinomio de esa tabla combina $`b_n`$ con $`a_1,a_0`$; en la página 3
aparece $`Kx`$ para la propuesta de $`g(x)=\mathop{\mathrm{sen}}\nolimits x`$;
en el punto 8 de la página 4 no se distingue prima sobre el término $`-6y`$. No
se completan ni resuelven los apartados.
