# Cobertura de documentos Office — archivo 2022

Una transcripción por SHA-256. El año de archivo no se considera año impreso.
Los duplicados entre años se referencian desde el inventario general. Los
originales se preservaron; las conversiones y PDF de comparación se generaron
fuera del repositorio.

Se compararon todas las páginas/diapositivas publicadas con la exportación de
LibreOffice, el XML del original y la extracción. Las fórmulas OMML y OLE se
recuperaron a LaTeX; las figuras DrawingML omitidas por Pandoc se recuperaron
del render. Los errores de representación de LibreOffice se señalan en las
notas. No se verificó la corrección matemática de las respuestas del material.

Herramientas: mise; Pandoc 3.12.1; LibreOffice con perfil temporal aislado;
MarkItDown; Poppler; XML OOXML. Validación: mdformat GFM+MyST,
markdownlint-cli2, enlaces e imágenes y KaTeX. La regla MD036 se desactiva en
las transcripciones para conservar énfasis del original; la numeración se
escribe explícitamente.

| Fuente | SHA-256 | Páginas/diapositivas revisadas | Estado y salida |
| -- | -- | -- | -- |
| Series de Fourier.docx | `06f15262bcf5c45da99dfb95c58722ce209571199a972d57a9d280f882e71bf2` | 5 | [transcribed-reviewed](../../notes/2022/practica/series-de-fourier.md) |
| TEMARIO PARA COLOQUIO TEÓRICO.docx | `a32af611313cde7f6d35957179933cc117a44a950d0e4f1c0fe756898a19e95a` | 4 | [transcribed-attribution-pending](../../notes/2022/teoria/temario-para-coloquio-teorico.md) |
| Trabajo práctico 1.docx | `62164cd928eef07e4d32b48321041151fd535da795cb89a14c2b58249be3d101` | 1 | [transcribed-reviewed](../../notes/2022/practica/trabajo-practico-1.md) |
| repaso.docx | `2e04ae39143c8140e4fe929fdb906bbcbc1ccd7fee495d07912b8cf56e918830` | 1 | [transcribed-reviewed](../../notes/2022/practica/repaso.md) |

## Límites y atribución

- TEMARIO PARA COLOQUIO TEÓRICO.docx: Pendiente: temario de álgebra sin
  identificación AMII. Su ubicación en la carpeta no demuestra pertenencia a
  ISI.

## Revisión final de notación

Las expresiones que la extracción conservó como texto o superíndices/subíndices
HTML se pasaron a LaTeX, manteniendo sus valores, letras y signos. La
comprobación integral registra el estado final.
