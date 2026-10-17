# Cobertura de las guías y apuntes PDF de 2016

Se revisaron todas las páginas de las fuentes listadas. Se compararon la
extracción de PyMuPDF4LLM, `pdftotext -layout` y los renders completos con
`pdftoppm`. Los originales se preservaron y las figuras se recortaron de las
páginas originales.

Las fórmulas perdidas por la extracción se transcribieron visualmente en LaTeX.
La prueba de Docling con enriquecimiento de fórmulas y el modelo local no
recuperó todas las ecuaciones; sus resultados no se aceptaron sin cotejo. No se
resolvieron ejercicios ni se corrigieron silenciosamente las erratas.

| Fuente | SHA-256 | Páginas revisadas | Nota |
| -- | -- | -- | -- |
| `Problemas ecuaciones Diferenciales.pdf` | `81bf4a15fb4b12dc44ca4c8a94cf3a933b25dea70abaf83447dd2bdc34497dc2` | 1–1 | [Transcripción](../../notes/2016/practica/aplicaciones-edo-primer-orden.md) |
| `Guia completa TP.pdf` | `81904abdbf3a7b1f30e98ca1d94690f9ce5c9f797e5893ae5601d54833cc12bd` | 1–30 | [Transcripción](../../notes/2016/practica/guia-completa-tp.md) |
| `Extremos condicionados.pdf` | `d884d40f2f40675e17855d27383134413497907bfe3677fb0d9cc5a96936e1fc` | 1–1 | [Transcripción](../../notes/2016/practica/extremos-condicionados.md) |
| `Diferenciales.pdf` | `aa463643dea563d1d43bb2856273135d22634dc157748742d7a18ced3e9385d4` | 1–1 | [Transcripción](../../notes/2016/practica/diferenciales.md) |
| `Práctica 4°parcial.pdf` | `f841293a1657801ff36ae4d7b4d80d8c141cfc3b29e54bc192ee28db6666574a` | 1–1 | [Transcripción](../../notes/2016/practica/practica-cuarto-parcial.md) |
| `Funciones_vectoriales.pdf` | `fa54e1ff334cfc21455c6d01e3be3daada5b32be99863e2fdd8b47de24e6504a` | 1–2 | [Transcripción](../../notes/2016/practica/funciones-vectoriales.md) |
| `Integrales de línea.pdf` | `82f202de675475aa05074c207f57a65b42fbc77406c12896f356a9651db79f08` | 1–3 | [Transcripción](../../notes/2016/practica/integrales-de-linea.md) |
| `Análisis vectorial.pdf` | `da628be5df05a861c8879fe3598d791d0093491274f711f978dd5c412760379f` | 1–2 | [Transcripción](../../notes/2016/practica/analisis-vectorial.md) |
| `Extremos absolutos y relativos.pdf` | `deb4ef3e05937e3e9557087c9c62a4cb5fefe7565b3568d5cffde5dde0a62707` | 1–2 | [Transcripción](../../notes/2016/practica/extremos-absolutos-y-relativos.md) |
| `Derivadas.pdf` | `f31924fc8772bdd04f7ea07897071d29a45f71dc52b071a3609477c0a4d52c7c` | 1–1 | [Transcripción](../../notes/2016/practica/derivadas-parciales.md) |
| `Gráficas Cuádricas.pdf` | `97e56cb8a4db202d1a927a3a98466cdbc85ed0990f082d23095e6aeb4daaa9b3` | 1–1 | [Transcripción](../../notes/2016/practica/graficas-cuadricas.md) |
| `Teórico Multiplicadores de Lagrange.pdf` | `5dbe7f56c564d67459aaf1722e25cd1f6464ff2f95a7c8aa9d01736f4e514288` | 1–2 | [Transcripción](../../notes/2016/teoria/multiplicadores-de-lagrange.md) |
| `Gradiente.pdf` | `093d85e918e12a62438e776133a0e237c3a502ed53f4ccfc2984c8e9f773047f` | 1–3 | [Transcripción](../../notes/2016/teoria/gradiente.md) |
| `Qué esperamos del estudiante.pdf` | `a45b53c14dc56f254ab544075761e387526629bd6179a9a2b78cbc4a47befe29` | 1–1 | [Transcripción](../../notes/2016/teoria/que-esperamos-del-estudiante.md) |
| `Funciones de dos o más variables.pdf` | `e0f38d684e896ef8d93f07c3e6e801035f982882e408aa3b009398677c5d2f04` | 1–4 | [Transcripción](../../notes/2016/teoria/funciones-de-dos-o-mas-variables.md) |
| `Integrales.pdf` | `68e0519be849eb9f920ac5d44ff32ec51004f230497282ea931306da70e8cc4c` | 1–29 | [Transcripción](../../notes/2016/teoria/integrales-multiples.md) |
| `Espacio Métrico.pdf` | `76b592cff32df803867c0be7509cbebce81f46363d94be871f93bce475fd4648` | 1–2 | [Transcripción](../../notes/2016/teoria/espacio-metrico.md) |

## Contenido y límites

La guía completa conserva las ocho partes y los 133 números de ejercicio, con
sus incisos, tablas y ejemplos resueltos ya presentes en la fuente. Incluye las
hojas de Mathcad y 27 imágenes: diagramas de los problemas, 13 gráficas de
Fourier y la salida gráfica final. La numeración anómala se mantiene. Los glifos
que no se representan en nº108 y nº111 están marcados en el texto.

El apunte de integrales múltiples conserva las 29 diapositivas y 21 grupos de
figuras originales. Los textos y fórmulas de todos los paneles se
transcribieron; las erratas de componentes y coordenadas se señalan en la nota.

En Funciones de dos o más variables, las etiquetas pequeñas borrosas de la
última figura no se reconstruyen. Se conserva la figura original. Las gráficas y
las salidas de Mathcad de la guía y los apuntes se cotejaron tras el recorte.

Los encabezados de procedencia enlazan al registro con archivo original, SHA-256
y alias entre años. No consta año impreso en estas fuentes; 2016 designa su
ubicación de archivo.

## Herramientas y validación

Herramientas administradas por mise: PyMuPDF4LLM 1.28.2, Docling 2.133, Poppler,
mdformat GFM+MyST, markdownlint-cli2 y KaTeX. Los recortes usan Pillow del
runtime de Codex. El formato se comparó antes y después para asegurar que las
expresiones LaTeX no cambiaron. El informe general registra el resultado del
checker final.
