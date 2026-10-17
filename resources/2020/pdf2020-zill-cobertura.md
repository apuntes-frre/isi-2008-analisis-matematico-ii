# Extracto de Zill: cobertura de las 91 páginas

Fuente archivada en 2020:
`15-EDO 2do Orden/Ecuaciones diferenciales con aplicaciones de modelado - Zill.pdf`.

SHA-256 del original:
`4373f88aeb43912f458f3c255587f7a4e7bc4516e309cfd99a6a2b59070fea64`.

La atribución a Zill procede del nombre del archivo. El extracto no contiene
portada editorial; no se identifican edición ni año de publicación. Se conserva
como lectura bibliográfica y no se atribuye a la cátedra ISI.

Se revisaron visualmente las páginas PDF 1–91, que corresponden a las páginas
impresas 117–207. La numeración impresa se conserva, junto con los ejercicios,
ejemplos, tablas, notas al pie y figuras. El archivo empieza en el capítulo 4 y
termina durante la sección 5.3; no se completa contenido que queda fuera del
original disponible.

La transcripción se divide en 15 notas y conserva 56 archivos de medios
extraídos o recortados del PDF original.

## Notas y páginas

| Páginas PDF | Páginas impresas | Notas |
| -- | -- | -- |
| 1–30 | 117–146 | [Nota 1](../../notes/2020/teoria/pdf2020-zill-01-a-teoria-lineal.md); [Nota 2](../../notes/2020/teoria/pdf2020-zill-01-b-reduccion-orden.md); [Nota 3](../../notes/2020/teoria/pdf2020-zill-01-c-coeficientes-constantes.md); [Nota 4](../../notes/2020/teoria/pdf2020-zill-01-d-superposicion.md) |
| 31–60 | 147–176 | [Nota 1](../../notes/2020/teoria/pdf2020-zill-02-44-superposicion.md); [Nota 2](../../notes/2020/teoria/pdf2020-zill-02-45-anulador.md); [Nota 3](../../notes/2020/teoria/pdf2020-zill-02-46-variacion.md); [Nota 4](../../notes/2020/teoria/pdf2020-zill-02-47-cauchy-euler.md); [Nota 5](../../notes/2020/teoria/pdf2020-zill-02-48-eliminacion.md); [Nota 6](../../notes/2020/teoria/pdf2020-zill-02-49-no-lineales.md) |
| 61–91 | 177–207 | [Nota 1](../../notes/2020/teoria/pdf2020-zill-03-01-no-lineales-repaso.md); [Nota 2](../../notes/2020/teoria/pdf2020-zill-03-02-modelos-valores-iniciales.md); [Nota 3](../../notes/2020/teoria/pdf2020-zill-03-03-ejercicios-modelos.md); [Nota 4](../../notes/2020/teoria/pdf2020-zill-03-04-valores-frontera.md); [Nota 5](../../notes/2020/teoria/pdf2020-zill-03-05-modelos-no-lineales.md) |

## Extracción y revisión

Se contrastaron PyMuPDF4LLM, el texto de Poppler con disposición de página y las
páginas renderizadas. Las fórmulas se repararon contra la imagen original y se
validaron con KaTeX. Los diagramas se conservaron como medios originales con
referencias locales, sin base64.

En una muestra de PDF 2–3 se evaluó Docling con enriquecimiento de fórmulas.
Recuperó siete bloques matemáticos, pero degradó expresiones en línea y alteró
el orden de una figura. Se mantuvo la combinación de extracción y revisión
visual para el lote completo. La comparación se conserva en el directorio
temporal de trabajo, fuera de Git.

## Límites de la fuente

Las continuaciones entre los tres rangos se enlazan mediante la numeración de
sección y de página. Se conserva el corte del final del archivo en la sección
5.3. Las erratas se mantienen y se señalan en las notas; no se resuelven
ejercicios propuestos.

## Validación

Los tres rangos tienen revisión visual de todas sus páginas y medios, control de
LaTeX, mdformat GFM+MyST, markdownlint y enlaces locales. La unión de los
resultados abarca exactamente PDF 1–91, sin huecos ni páginas duplicadas.
