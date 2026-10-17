# Cobertura de documentos Office — archivo 2020

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
| 14-teorema de Stockes y Divergencia/Teorema de Stokes.ppsx | `ead627d9a3c38dde1088747f5580faca460c8570f440c4e9a57a94de71fa3085` | 5 | [transcribed-reviewed](../../notes/2020/teoria/office-teorema-de-stokes-ead627d9.md) |
| 5-Funciones de Varias Variables ( Campo Escalar)/Probelmas de Aplicacion Campo Escalar.docx | `cba1ebb523ca357d09be00fe124e3845810682ad5e7e48795842eafe810d3538` | 8 | [transcribed-reviewed](../../notes/2020/practica/office-probelmas-de-aplicacion-campo-escalar-cba1ebb5.md) |
| Documento identificatorio/administrativo excluido | `66f17d72d0c3e7fb81b7ed4c9c6a9848af8a3f4d169870024ea7d778cecf6a97` | — | Sin publicación de datos personales |
| clase practica - limites.docx | `3c5ba32634a50fb49497674c93144445b112fae7b9c383efbbfa14aeeaba22d4` | 1 | [transcribed-reviewed](../../notes/2020/practica/office-clase-practica-limites-3c5ba326.md) |

## Límites y atribución

- Probelmas de Aplicacion Campo Escalar.docx: Identificación ISI o varias
  carreras que incluyen ISI en fuente. Se omiten nombre y legajo de la portada y
  encabezados. Se preservan las respuestas y errores del trabajo entregado, sin
  validarlos como soluciones correctas.

## Revisión final de notación

Las expresiones que la extracción conservó como texto o superíndices/subíndices
HTML se pasaron a LaTeX, manteniendo sus valores, letras y signos. La
comprobación integral registra el estado final.
