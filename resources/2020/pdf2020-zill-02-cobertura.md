# Cobertura de Zill: páginas PDF 31–60

Fuente: `Ecuaciones diferenciales con aplicaciones de modelado - Zill.pdf`,
carpeta canónica `2020/15-EDO 2do Orden/` de Análisis Matemático II en Materias
Homogéneas de OneDrive. La atribución a Zill proviene del nombre del archivo; el
extracto no incluye portada, edición ni año verificables. Es bibliografía
externa, sin atribución a ISI. La carpeta 2020 indica ubicación de la fuente, no
año de publicación.

- SHA-256 del PDF original de 91 páginas:
  `4373f88aeb43912f458f3c255587f7a4e7bc4516e309cfd99a6a2b59070fea64`.
- Alcance de este lote: PDF 31–60, impresas 147–176, todas revisadas
  visualmente.
- El inicio continúa un ejemplo de la sección 4.4; el final corta la sección
  4.9. Son límites de este rango, no omisiones de contenido dentro de sus
  páginas.
- Los ejercicios permanecen sin resolver. Se conservan las soluciones impresas.

| Páginas PDF | Impresas | Nota | Contenido y conteo |
| -- | -- | -- | -- |
| 31–33 | 147–149 | [Superposición](../../notes/2020/teoria/pdf2020-zill-02-44-superposicion.md) | Continuación de ejemplo, ejemplos 10–11, comentarios, ejercicios 1–47, figuras 4.4.1–4 |
| 34–41 | 150–157 | [Anulador](../../notes/2020/teoria/pdf2020-zill-02-45-anulador.md) | Sección 4.5 completa, ejemplos 1–7, ejercicios 1–73 |
| 41–46 | 157–162 | [Variación](../../notes/2020/teoria/pdf2020-zill-02-46-variacion.md) | Sección 4.6 completa, ejemplos 1–3, ejercicios 1–34 |
| 46–52 | 162–168 | [Cauchy-Euler](../../notes/2020/teoria/pdf2020-zill-02-47-cauchy-euler.md) | Sección 4.7 completa, ejemplos 1–6, ejercicios 1–47, figura 4.7.1 con dos paneles |
| 53–57 | 169–173 | [Eliminación](../../notes/2020/teoria/pdf2020-zill-02-48-eliminacion.md) | Sección 4.8 completa, ejemplos 1–3, ejercicios 1–27, figuras 4.8.1–3 |
| 58–60 | 174–176 | [No lineales](../../notes/2020/teoria/pdf2020-zill-02-49-no-lineales.md) | Inicio de sección 4.9, ejemplos 1–3, nota al pie |

Las páginas compartidas en la tabla contienen finales y comienzos de secciones
distintas; cada fragmento se transcribe una sola vez. Total: seis notas, 228
ejercicios numerados, 24 ejemplos completos más una continuación, ocho figuras
numeradas (nueve paneles), ninguna tabla de datos y una nota al pie.

## Extracción y revisión

Se extrajeron estas 30 páginas con qpdf sobre una copia de trabajo. Se
compararon PyMuPDF4LLM (Markdown e imágenes) y Poppler `pdftotext -layout`.
Ambos pierden signos, derivadas y notación en línea en este PDF; no se adoptó su
salida sin reparación. Se cotejaron las 30 páginas renderizadas con `pdftoppm` a
2000 píxeles de lado mayor y se transcribió la matemática en LaTeX. La
evaluación común de Docling sobre dos páginas del mismo PDF no resolvió las
pérdidas en línea ni el orden de lectura; no se ejecutó un lote completo de ese
motor.

Las ocho figuras originales se recortaron directamente del PDF con PyMuPDF y se
conservaron con sus etiquetas y pies en
[el directorio de medios](pdf2020-zill-02/). Los recortes fueron inspeccionados.
Los cuadros y llamadas de igualdad entre coeficientes se transcribieron como
notación y texto, sin capturas de ecuaciones.

## Erratas conservadas y límites

- Página 147: referencia impresa a “tabla 4.1”.
- Página 152: redacción “pero también a los operadores”.
- Página 154: `n=1` en el ejemplo 5, aunque se usa el anulador al cuadrado.
- Página 157: ejercicio 67 muestra `y(0)` sin valor ni igualdad; ejercicios
  27–34 dicen “funciones […] que anulan el operador”.
- Página 162: ejercicios 23–24 piden la ecuación “homogénea” aunque muestran
  miembros derechos no nulos.
- Páginas 165–167: condiciones y referencias internas se mantienen como
  aparecen.
- Página 169: el traslado de `-4x` cambia de signo incorrectamente en el ejemplo
  de notación de operadores; se conserva la secuencia impresa.
- Página 171: se conservan el coeficiente de seno y su ecuación de constantes
  impresos en el ejemplo 2.
- Página 173: ejercicio 27 a) imprime `x_2(t)=10` y `x_3(t)=5`.
- Página 175: constante `c_1^2`, “segunda ecuación diferencial” y “específican”.
- Las figuras 3.3.1 y 3.3.7 sólo se citan; no se reproducen en estas páginas.

No queda texto ilegible o contenido interno pendiente identificado en el rango.
Las referencias a otros capítulos, tablas y respuestas se conservan sin inventar
las páginas ausentes del extracto.

## Validación

Pendiente de cierre: formato GFM y MyST, lint, vínculos locales, integridad
textual y renderizado KaTeX sobre estas seis notas y este informe
exclusivamente.
