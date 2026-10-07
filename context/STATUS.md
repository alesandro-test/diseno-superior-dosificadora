# STATUS — Diseño Superior

**Última actualización:** 2026-10-07

## Estado actual

Documento de Diseño Superior iniciado a partir del contenido de Taller de Grado I.
Contexto reorganizado para DS el 06/10/2026 según la revisión del docente (Ing. Ivan Mendoza) del 29/09/2026.
Estructura LaTeX reorganizada según `THESIS_STRUCTURE.md` (00B, 07/10/2026): un archivo por capítulo en `docs/thesis/chapters/ds/` (01–09); `marcoref.tex` queda como respaldo sin incluir en `main.tex`. Secciones nuevas vacías marcadas con `% PENDIENTE`; puntos a revisar tras el traslado marcados con `% REVISAR`.
Trabajo activo: **01C — Introducción**.

## Completado

- Revisión escrita del docente (29/09/2026) y extracción de la clase guardadas en `research/docente/`.
- `PROFESSOR_NOTES.md` reemplazado por criterios de DS; criterios de Taller I archivados en `research/docente/criterios_taller_I.md` como complementarios.
- `THESIS_STRUCTURE.md` rehecho sobre la plantilla DS (`docs/template/Template_Diseno_Superior.md`, guardada el 06/10/2026); la de Taller I archivada en `research/docente/estructura_taller_I.md`.
- **00B — Reestructuración LaTeX (07/10/2026):** contenido de `marcoref.tex` reubicado sin reescribir texto: Antecedentes → 4.0 Contextualización (numerada 4.0); Formulación, Árbol de problemas y Justificación → 1.3; Delimitación → 1.5 Alcance del proyecto; secciones 1.1, 1.2, 1.3.3 (tabla de inconformidades), 1.6 y capítulos 2–9 creados vacíos. Etiquetas conservadas (`sec:problema` → 1.3; `subsec:antecedentes_problema` → 4.0). Comentario del docente en `main.tex` corregido a Diseño Superior.
- Heredado de Taller I (vigente como base): relevamiento del 02/09 y 05/09/2026, diagnóstico, proyecciones, figuras de Antecedentes, tabla comparativa RUICHUAN / Trust-Long.

## En curso

- **01C — Introducción, 1.1 y 1.2:** conservar párrafos actuales; agregar bloque macro (rubro panadero, 1–2 párr.) y micro (San Miguel: productos, mercados, datos externos, 1–2 párr.); trasladar el párrafo de registros de campo fuera de la Introducción; redactar 1.1 Metas de la empresa y 1.2 Objetivos de la empresa alineados. Requiere búsqueda de fuentes externas (estudiante: Perplexity, Scopus, Google Scholar → NotebookLM) y datos de la panadería.

## Próximos pasos

1. **01C — Introducción, 1.1 y 1.2:** búsqueda de fuentes (Bolivia → región → internacional), redacción macro → micro, metas y objetivos de la empresa.
2. **01A — 1.3 Problema y 4.0 Contextualización:** reubicar Antecedentes en 4.0; descripción textual con la fórmula VI + efecto VD + condiciones + contexto; Ishikawa desde el árbol actual; tabla de inconformidades con especificación de referencia; oración del problema sobre el proceso; justificación económica.
3. **01B — 1.4 Objetivos, 1.5 Alcance por ejes, 1.6 Metodología:** OE por etapa del Modelo en V (7 etapas); OG con fórmula verbo + qué + para qué + con qué; alcance por ejes solo con valores sustentados.
4. **04 — 2. Estudios preliminares:** tabla factibilidad / viabilidad / deseabilidad.
5. **02 — Investigación:** precios puestos en Bolivia; mantenibilidad y eficiencia de competidores; OIML R60 / R76 / R61 y su aplicabilidad; reglamentación municipal citada por el docente (peso de pan); ISO 9126 vs. ISO/IEC 25010.
6. **03 — Diagramas y presentación:** Ishikawa; figura del Modelo en V; gráfica de tiempo acumulado medición/proyección; láminas con fachada e imágenes agrupadas.
7. **Portada:** fecha diciembre según el docente (actualmente automática; no modificada en 00B). Etiqueta del docente en `main.tex` corregida. Queda el texto de portada en `packages/ucbimt.sty` («…habilitación a Taller de Grado I»), no modificado por indicación del estudiante.
8. Después: Estado del arte, Contextualización completa, Requerimientos (caja negra, QFD, RF/RNF).

## Bloqueos / pendientes de validación

- Título: la sugerencia del docente («ingredientes secos», «en cumplimiento de OIML R60/R76») choca con D-002 (solo harina) y con afirmar cumplimiento sin verificación (A-001, A-005, A-006).
- Los valores numéricos de la revisión (1000/800 und/h, recipientes 50 L = 200 und, 60 g por pieza, −200 und) no provienen del relevamiento; no usarlos como datos del caso sin verificación con la panadería o fuente.
- Las no conformidades requieren una especificación de referencia (receta, tolerancia, norma); la tolerancia de aceptación sigue abierta (A-004).
- El límite actual «no se realizará el modelamiento matemático» contradice la etapa de diseño detallado que pide el docente (A-007).
- Alcances actuales de `marcoref.tex` (5–15 kg, 5 g, ±0,5 %, 50 kg) contradicen D-009 / A-004.
- Contextualización pide tamaño de grano, densidad y proporciones de receta: no medidos ni documentados; requieren fuente o relevamiento.
- La duración de la jornada no está registrada; un porcentaje respecto de la jornada requiere nuevo dato.
- 1.1 Metas de la empresa requiere información de la Panadería San Miguel (no documentada aún).
- Ubicación de Contextualización (4.0 propuesto) por confirmar: la plantilla no la incluye y la revisión sí.
- Bibliografía en ISO 690: el preámbulo ya usa `biblatex` con `style=iso-authoryear`; falta revisar la salida contra lo pedido por la plantilla.
- Compilación 00B verificada con pdflatex en entorno parcial (sin biber); confirmar compilación completa con biber en el equipo del estudiante.
- Transiciones a revisar tras 00B (`% REVISAR`): cierre de la Introducción («La sección siguiente…») y cifras de 1.3.1 que ahora se calculan en 4.0.
- Estado del arte: la plantilla pide 30 elementos con criterios de inclusión/exclusión.
- Formulación y diapositiva presentan 1 h 59 min sin explicitar que es proyección.

## Archivos activos

- `docs/thesis/chapters/ds/01_introduccion.tex` … `09_conclusiones.tex`
- `docs/thesis/chapters/marcoref.tex` (respaldo, no incluido)
- `docs/thesis/main.tex`
- `context/PROFESSOR_NOTES.md`
- `context/THESIS_STRUCTURE.md`
- `docs/template/Template_Diseno_Superior.md`
- `research/docente/revision_DS_2026-09-29.md`
