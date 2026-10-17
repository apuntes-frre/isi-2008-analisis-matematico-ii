# Cobertura del lote de teoría 2016

Fuentes canónicas: OneDrive-FacultadRegionalResistencia,
`Facultad/Materias Homogeneas/Analisis Matemático II/2016/` (carpeta autorizada
para esta materia). Revisión realizada el 15 de octubre de 2026. Los originales
permanecen intactos; se trabajó sobre copias materializadas fuera del
repositorio, verificadas por SHA-256.

## Originales y resultados

| Original | Páginas | Nota | Revisión |
| -- | -- | -- | -- |
| Consideraciones sobre Series de Fourier.pdf | 6 | [Estrategias prácticas](../../notes/2016/teoria/resume-teoria-consideraciones-series-fourier.md) | 1–6; página 6 sin contenido |
| Teórico Ecuaciones diferenciales.pdf | 14 | [Ecuaciones diferenciales](../../notes/2016/teoria/resume-teoria-ecuaciones-diferenciales.md) | 1–14 |
| Series de Fourier.pdf | 22 | [Series de Fourier](../../notes/2016/teoria/resume-teoria-series-fourier.md) | 1–22; fragmento tapado en página 13 |

### Consideraciones sobre Series de Fourier.pdf

- SHA-256: `d051fd73983dfffa7583db8f924b14dc6ff68e085f5b124f07c538f568de9dc9`.
- Autor: Arnaldo César Flores. Año de edición no indicado; 2016 corresponde al
  archivo de origen.
- 5 casos, con demostraciones y un ejemplo de cambio de escala. Sin ejercicios
  vacíos, tablas, figuras ni anexos. Página 6 con borde, sin texto.
- Texto de páginas 1–5 y todas sus fórmulas transcritos; erratas preservadas y
  señaladas al final de la nota. No quedan fragmentos ilegibles identificados.

### Teórico Ecuaciones diferenciales.pdf

- SHA-256: `97a5e4f9889d33dfc28a3e4511ee24863eb23c4261f63e6ff4431c250bfa198e`.
- Autor y año de edición no indicados; 2016 corresponde al archivo de origen.
- 4 ecuaciones de clasificación; 1 comprobación de solución; 1 ejemplo de
  isoclinas; 2 ejemplos de obtención de ecuación diferencial; 1 desarrollo de
  trayectorias ortogonales; 2 ejemplos de variables separables; 1 ejemplo y 2
  propiedades de funciones homogéneas; 1 ejemplo de coeficientes homogéneos; 2
  ejemplos de ecuaciones exactas; 1 ejemplo lineal; 1 de Bernoulli; 1 problema
  de desintegración. Sin ejercicios vacíos, tablas ni anexos.
- 1 gráfico original de trayectorias ortogonales conservado y enlazado. Las
  fórmulas de las 14 páginas se recuperaron a LaTeX por inspección visual.
- Se conservan las erratas de signos, índices, derivadas y factores, detalladas
  en la nota. No quedan fragmentos ilegibles identificados.

### Series de Fourier.pdf

- SHA-256: `9f1f944b3949952f8afa409575d5f39b5b664b9ce9d59f87f2536faf70276010`.
- Autor: Ing. Leopoldo De Urrutia. Responsable de edición en formato
  electrónico: Prof. Bibiana Altamirano. Gráficos: Ing. Luciano Curie. Año de
  edición no indicado; 2016 corresponde al archivo de origen.
- 3 propiedades de funciones pares, 4 de impares, 5 de periódicas, 7 fórmulas
  numeradas, lema de Rieman-Lebesgue y demostración, 3 ejemplos de ondas,
  derivación de coeficientes de Euler, condiciones y fórmula de Dirichlet,
  demostración de convergencia en 2 casos, desarrollos pares/impares y de
  período 2L, 2 ejemplos resueltos de onda rectangular.
- 3 consignas «Demuestre» preservadas sin resolver. Sin tablas de datos ni
  anexos. Los paneles de gráficas conservan su disposición y etiquetas.
- 42 gráficas conservadas en 20 imágenes (varios paneles reúnen tres gráficas).
  Recortes de los renders del original; ninguna ecuación fue sustituida por una
  captura. Las etiquetas matemáticas también se transcriben en texto.
- Pérdida del original: en la última viñeta de la página 13, el recuadro de aₙ
  oculta parte de la frase y su fórmula. La nota señala el fragmento tapado; no
  se reconstruyó por inferencia. Todo el contenido visible de las 22 páginas fue
  revisado y transcrito.
- Se mantienen las erratas matemáticas y afirmaciones originales, identificadas
  al final de la nota, sin corrección silenciosa.

## Herramientas y controles

- Preflight común: herramientas mise, materialización de originales, comparación
  de SHA-256 y conteos PDF.
- PyMuPDF4LLM 1.28.2,
  `--backend md --workers 1 --ocr-mode never --write-images --header --footer`,
  como extracción inicial. Se contrastó con `pdftotext -layout` de Poppler.
  Ambos omiten muchas fórmulas del original.
- Se revisaron visualmente las 42 páginas renderizadas con `pdftoppm`, escala
  máxima 1800 píxeles. Recuperación manual de fórmulas a LaTeX y del texto
  omitido, manteniendo números, orden y erratas.
- Para las figuras de Fourier se conservaron recortes del render original con
  Pillow del runtime de Codex. El gráfico de ecuaciones diferenciales procede de
  la extracción referenciada de PyMuPDF4LLM.
- Formato con mdformat, extensiones GFM y MyST, ajuste a 80 columnas y tablas
  compactas. Validador de transcripción del repo sobre estos cuatro Markdown:
  formato, markdownlint, enlaces/imágenes, caracteres defectuosos y KaTeX. Los
  resultados se registran con el informe de este lote.
- El formato y KaTeX verifican sintaxis; la fidelidad se evaluó contra las
  páginas, incluidas las erratas que renderizan pero no son correctas.
