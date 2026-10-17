# Cobertura de Integrales_AM

- Fuente canónica:
  `OneDrive-FacultadRegionalResistencia/Facultad/Materias Homogeneas/Analisis Matemático II/2020/14-teorema de Stockes y Divergencia/Integrales_AM.pdf`.
- SHA-256: `a5b25ccaf48d5b3930ed873bcbfb5f0a1eae705a83aac7174c53a730ff118a04`.
- Archivo: 306067 bytes; 32 páginas, numeradas 1/32–32/32.
- Fecha impresa: septiembre 2011; curso 2011-12. El año 2020 corresponde a su
  ubicación de archivo y no se atribuye a la edición.
- Autor: no consta en la portada ni en las diapositivas. El emblema original se
  conserva sin inferir su institución.
- Transcripción:
  [Lectura 3. Integrales de línea y de superficie](../../notes/2020/teoria/integrales-am.md).
- Estado: completa; las 32 páginas fueron cotejadas visualmente, incluidas
  portada, fórmulas, figuras, comentarios, ejemplos y ejercicios.
- Conteos: 32 diapositivas; tres ejemplos de motivación física; seis ejemplos
  matemáticos (incluidas las dos parametrizaciones de la página 15); dos
  ejercicios sin resolver; tres grupos de diagramas con cinco curvas/dibujos; un
  emblema repetido. Cuatro medios referenciados.

## Extracción y revisión

El preflight materializó una copia del original, verificó SHA-256 y contó
páginas. Se mantuvo intacto el archivo de OneDrive.

Se aplicaron PyMuPDF4LLM 1.28.2 con Markdown y extracción de imágenes,
`pdftotext -layout` y render de las 32 páginas mediante `pdftoppm`. Las
expresiones matemáticas de ambas extracciones necesitaron recomponer orden,
subíndices, integrales de circulación y letras vectoriales; se transcribieron en
LaTeX comparándolas con cada diapositiva. El PDF tiene texto y no necesitó OCR.

Los diagramas se recortaron del PDF original con PyMuPDF, sin redibujarlos. Se
revisaron sus etiquetas y sentidos de flechas. Los encabezados repetidos se
registran mediante los títulos de sección y página; el emblema repetido se
conserva una vez junto a la portada. Los iconos de navegación de la presentación
no son contenido docente y no se incorporan al apunte.

Se preservan las erratas señaladas al final de la nota, entre ellas la dimensión
indicada en las páginas 12 y 29 y el producto
$`\boldsymbol T_u\times\boldsymbol T_u`$ de la página 27. No se resuelven los
ejercicios de las páginas 28 y 32. No hay texto ni fórmulas pendientes de
lectura.

## Validación

Pasaron los controles de formato con mdformat GFM + MyST, lint con la
configuración del repo, enlaces y medios locales, caracteres defectuosos y
render de las expresiones con KaTeX mediante `.github/transcription/check.py`
sobre estos dos archivos. La excepción local MD036 preserva los rótulos
destacados de la fuente. La validación técnica complementa el cotejo de las 32
páginas.
