# Cobertura: Integrales de línea. Teorema de Green — Vallejo

- Fuente externa: José Antonio Vallejo, Departamento de Matemáticas, Facultad de
  Ciencias, Universidad Autónoma de San Luis Potosí.
- Fecha impresa: 16 Noviembre 2007.
- Archivo canónico:
  `OneDrive-FacultadRegionalResistencia/Facultad/Materias Homogeneas/Analisis Matemático II/2020/13-Teoriema de Green/T. Green.pdf`.
- SHA-256: `91b91b026cb4e2526d8808125d968eade0dac19b452cef318bab28874fd0316b`.
- Extensión: 369282 bytes, 19 páginas, numeradas 1–19.
- Año de archivo: 2020. No se atribuye la autoría ni la procedencia académica de
  este documento a ISI ni a UTN.
- Transcripción:
  [Integrales de línea. Teorema de Green](../../notes/2020/teoria/green-vallejo.md).
- Revisión: completa, 19/19 páginas cotejadas visualmente el 2026-10-16.
- Conteos: seis secciones, seis definiciones, diez ejemplos, cinco notas, una
  notación, un teorema, 30 problemas numerados, una tabla y siete figuras.

## Extracción y fidelidad

Se preservó el original de OneDrive. La copia de trabajo proviene del preflight
que verificó SHA-256 y contó las 19 páginas. Se aplicaron PyMuPDF4LLM 1.28.2
(Markdown y medios), `pdftotext -layout` y render de todas las páginas con
`pdftoppm`.

La extracción presenta ligaduras defectuosas y orden alterado de fracciones,
sistemas y radicales. Se reconstruyeron texto y LaTeX contrastando cada página
renderizada. Los siete diagramas originales se conservaron mediante recortes del
PDF con PyMuPDF y se revisaron sus etiquetas, flechas y valores.

Se conservaron completas las soluciones impresas, los ejemplos desarrollados, la
nota al pie de la página 11 y las erratas señaladas al final de la
transcripción. Los ejercicios sin solución impresa permanecen sin resolver. Se
incluyen, entre otras expresiones extrañas, `cot s`, el radical 75 del ejemplo
4, los intervalos 0–2π de las páginas 5–6, el factor 3t de la página 8, la
solución 60π de la página 16 y los índices ti del integrando de la página 19. No
hay texto, ecuaciones ni figuras pendientes de lectura.

## Validación

Los controles pasaron sobre la nota y este registro (checker: dos archivos, sin
errores): mdformat con GFM + MyST, markdownlint con la configuración del repo,
enlaces relativos, existencia de los siete medios, ausencia de caracteres
defectuosos y KaTeX mediante `.github/transcription/check.py`. Las excepciones
locales MD029 y MD036 permiten conservar numeración y rótulos de la fuente sin
cambiar la configuración general.
