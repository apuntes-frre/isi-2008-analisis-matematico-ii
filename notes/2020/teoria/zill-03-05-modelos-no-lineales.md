# Zill — Final de ejercicios 5.2 y modelos no lineales

Fuente: extracto «Ecuaciones diferenciales con aplicaciones de modelado -
Zill.pdf». Zill es la atribución del nombre del archivo; edición y año no
constan en estas páginas. Material bibliográfico, no autoría de ISI.
[Procedencia y cobertura](../../../resources/2020/zill-03-cobertura.md).

Páginas PDF 91–91 (impresas 207–207). Se conserva el orden del extracto y la
continuidad de los capítulos.

## Página PDF 91 — Página impresa 207

### Tarea para el laboratorio de computación — Continuación de ejercicios 5.2

**35.** Use un SAC para trazar las gráficas que lo convenzan de que la ecuación
$`\tan\alpha=-\alpha`$ del problema 34 tiene un número infinito de raíces.
Explique por qué se pueden despreciar las raíces negativas de la ecuación.
Explique por qué $`\lambda=0`$ no es un eigenvalor aun cuando $`\alpha=0`$ es
una solución obvia de la ecuación $`\tan\alpha=-\alpha`$.

**36.** Usando un programa para determinar raíces de un SAC aproxime los
primeros cuatro valores propios $`\lambda_1`$, $`\lambda_2`$, $`\lambda_3`$ y
$`\lambda_4`$ para el PVF del problema 34.

En los problemas 37 y 38, determine los eigenvalores y las funciones propias del
problema con valores en la frontera. Use un SAC para aproximar los primeros
cuatro valores propios $`\lambda_1`$, $`\lambda_2`$, $`\lambda_3`$ y
$`\lambda_4`$.

**37.** $`y''+\lambda y=0`$, $`y(0)=0`$, $`y(1)-\frac12y'(1)=0`$.

**38.** $`y^{(4)}-\lambda y=0`$, $`y(0)=0`$, $`y'(0)=0`$, $`y(1)=0`$,
$`y'(1)=0`$. \[*Sugerencia*: considere sólo $`\lambda=\alpha^4`$,
$`\alpha\gt 0`$.\]

### 5.3 Modelos no lineales

### Repaso de material

- Sección 4.9

### Introducción

En esta sección se examinan algunos modelos matemáticos no lineales de orden
superior. Algunos de estos modelos se pueden resolver usando el método de
sustitución (lo que conduce a la reducción de orden de la ED) presentado en la
página 174. En algunos casos donde no se puede resolver el modelo, se muestra
cómo se reemplaza la ED no lineal por una ED lineal mediante un proceso conocido
como linealización.

### Resortes no lineales

El modelo matemático en (1) de la sección 5.1 tiene la forma

```math
m\frac{d^2x}{dt^2}+F(x)=0,\tag{1}
```

donde $`F(x)=kx`$. Debido a que $`x`$ denota el desplazamiento de la masa desde
su posición de equilibrio, $`F(x)=kx`$ es la ley de Hooke, es decir, la fuerza
ejercida por el resorte que tiende a restaurar la masa a la posición de
equilibrio. Un resorte que actúa bajo una fuerza restauradora lineal $`F(x)=kx`$
se llama **resorte lineal**. Pero los resortes pocas veces son lineales.
Dependiendo de cómo esté construido y del material utilizado, un resorte puede
variar desde “flexible” o suave, hasta “rígido” o duro, por lo que su fuerza
restauradora puede variar respecto a la ley lineal. En el caso de movimiento
libre, si se supone que un resorte en buen estado tiene algunas características
no lineales, entonces podría ser razonable suponer que la fuerza restauradora de
un resorte, es decir, $`F(x)`$ en la ecuación (1), es proporcional al cubo del
desplazamiento $`x`$ de la masa más allá de su posición de equilibrio o que
$`F(x)`$ es una combinación lineal de potencias del desplazamiento como el que
se determina mediante la función no lineal $`F(x)=kx+k_1x^3`$. Un resorte cuyo
modelo matemático incorpora una fuerza restauradora no lineal, como

```math
m\frac{d^2x}{dt^2}+kx^3=0\quad\text{o}\quad
m\frac{d^2x}{dt^2}+kx+k_1x^3=0,\tag{2}
```

se llama **resorte no lineal**. Además, se examinan modelos matemáticos en los
que el amortiguamiento impartido al movimiento era proporcional a la velocidad
instantánea $`dx/dt`$ y la fuerza restauradora de un resorte está dada por la
función lineal $`F(x)=kx`$. Pero estas fueron suposiciones muy simples; en
situaciones más reales, el amortiguamiento podría ser proporcional a alguna
potencia de la velocidad instantánea $`dx/dt`$. La ecuación diferencial no
lineal

```math
m\frac{d^2x}{dt^2}+\beta\left|\frac{dx}{dt}\right|\frac{dx}{dt}+kx=0\tag{3}
```

> Fin del extracto disponible: la oración y la sección 5.3 continúan fuera del
> PDF original de 91 páginas.
