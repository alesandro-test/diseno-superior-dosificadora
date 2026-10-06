# PROFESSOR_NOTES — Diseño Superior

> Criterios del docente de Diseño Superior (Ing. Ivan Mendoza) para el documento de DS.
> No contiene cifras del proyecto, decisiones ni estado de avance.
>
> **Fuentes y confiabilidad:**
> - **(R)** revisión escrita del 29/09/2026 — `research/docente/revision_DS_2026-09-29.md`. Fuente principal.
> - **(C)** clase del 29/09/2026, extracción automática NotebookLM — `research/docente/notebooklm_DS_clase_2026-09-29.md`. Útil para matices; cifras y números de normas pueden estar mal transcritos.
>
> - **(P)** plantilla DS — `docs/template/Template_Diseno_Superior.md`. Define estructura y recursos.
>
> **Criterios de Taller de Grado I:** `research/docente/criterios_taller_I.md`. Mismo proyecto, otra materia:
> son complementarios y se aplican cuando aportan (rigor de evidencia, redacción, trazabilidad).
> Si contradicen un criterio de aquí, señalar el conflicto en lugar de elegir en silencio.

## Título y portada

- **Título (sugerencia, no aprobado):** el docente cuestiona «bajo costo» y «diseño» y sugiere orientarlo a «dosificadora gravimétrica automatizada para ingredientes secos en cumplimiento de la normativa OIML R60 / R76 (metrología legal)». (R) Ver A-001, A-005 y A-006 en `DECISIONS.md`.
- **Fecha de portada:** diciembre. (R)

## Estructura y fórmulas de la plantilla

- **Estructura:** seguir la numeración de la plantilla DS (1.1 Metas de la empresa … 11. Anexos), aplicada en `THESIS_STRUCTURE.md`. (P)
- **Título:** responder ¿qué? ¿quién? ¿con qué? ¿para qué? (P)
- **Objetivo general:** verbo + qué + para qué + con qué (base científica, técnica, normativa). (P)
- **Problema:** [variable independiente] + [efecto en la variable dependiente] + [condiciones] + [contexto]. (P)
- **Empresa:** incluir metas de la empresa y objetivos de la empresa alineados al proyecto. (P)
- **Alcance:** por ejes — técnico, funcional, normativo, temporal, de usuarios y de limitaciones. (P)
- **Estudios preliminares:** factibilidad, viabilidad y deseabilidad con cumple / no cumple. (P)
- **Estado del arte:** 30 proyectos o productos (académicos, comerciales, patentes) con criterios de inclusión y exclusión. (P)
- **Requerimientos:** tablas RF/RNF con ID, O/D (obligatorio/deseable), descripción y valor técnico o norma. (P)
- **Verificación:** tabla requerimiento → diseño final → cumple / no cumple. (P)
- **Bibliografía:** ISO 690. (P)

## Introducción

- **De macro a micro:** partir del rubro y llegar a la empresa o unidad funcional. (R)
- **Macro (1–2 párrafos):** panaderías y pastelerías, su finalidad y su papel para la población. (R)
- **Micro (1–2 párrafos):** Panadería San Miguel — tipos de productos, mercados y datos externos a la panadería. (R)
- **Fuera de la Introducción:** descripción técnica operativa, flujos de planta, recetas y mediciones; corresponden a Contextualización. (C)

## Problema

- **Tres capas:** descripción textual → diagrama causa-efecto → no conformidades. (R)
- **No conformidades:** usar ISO 9126 u otra técnica de calidad. (R) Nota: ISO/IEC 9126 fue sustituida por ISO/IEC 25010; confirmar con el docente cuál emplear.
- **Oración del problema:** condensar el problema en una oración que integre imprecisión, falta de estandarización y uso no óptimo de recursos. (R)(C)
- **Correspondencia:** el objetivo general responde directamente a esa oración; si no hay correspondencia, no hay proyecto. (R)(C)
- **Procesos, no personas:** formular problema y causas sobre el proceso, no sobre el operario. (C)
- **Datos:** toda afirmación del diagnóstico se respalda con datos y toda cifra muestra su cálculo o fuente; sin datos es una opinión. (C)
- **Indicadores relativos:** expresar desvíos de tiempo también como porcentaje respecto de una referencia definida. (C)
- **Ejemplos del docente:** los valores numéricos de la revisión (und/h, recipientes, peso por pieza, −200 und) ilustran el formato; no se usan como datos del caso sin verificación.

## Objetivos y metodología

- **Metodología:** Modelo en V. (R)
- **Objetivos específicos por etapa:** (R)
  1. Contextualizar el modelo del sistema actual.
  2. Determinar los requerimientos.
  3. Diseñar los modelos detallados (CAD, P&ID, modelos matemáticos, SolidWorks).
  4. Implementar (prototipar, modelo funcional, simular).
  5. Verificar (normas internas, externas, locales, científicas).
  6. Validar.
  7. Mantener / controlar / operar.
- **Objetivo general:** respuesta directa a la oración del problema. (R)

## Desarrollo según Modelo en V

- **Contextualizar:** procesos de elaboración del pan; proporciones de ingredientes; características de la harina (tamaño de grano, densidad); máquinas existentes. (R)
- **Argumento (datos):** evidencia cuantitativa del sistema actual. (R)
- **Requerimientos:** caja negra → QFD → lista de requerimientos funcionales y no funcionales. (R)
- **Diseño detallado:** mockup o bosquejo, planos, modelos matemáticos. (R)
- **Implementación → Verificación → Validación → Transferencia y operación.** (R)

## Justificación, alcance y estado del arte

- **Justificación:** económica; no plantear justificación tecnológica salvo que se desarrolle una tecnología nueva. (C)
- **Comparación económica:** precios de competidores puestos en Bolivia (transporte, aduana, importación). (C)
- **Alcance:** capacidad útil, dimensiones y número de pruebas de funcionamiento; no repetir objetivos. (C)
- **Límites:** declarar explícitamente lo que no se hará. (C)
- **Estado del arte:** comparar con la competencia en precio, mantenibilidad y eficiencia y demostrar la ventaja de la propuesta. (C)

## Normativa

- **Metrología legal:** OIML R60 y OIML R76 señaladas por el docente. (R)
- **Mencionadas en clase:** inocuidad alimentaria, seguridad de máquinas (Directiva 2006/42/CE, ISO 12100), grado IP, protección antiexplosión, HACCP y una norma «193/2004» no identificable en la transcripción. (C)
- **Cumplimiento:** no afirmar cumplimiento normativo sin verificarlo; distinguir norma de referencia de norma verificada.

## Presentación oral

- Láminas ordenadas y poco cargadas; incluir fotografía de la fachada; agrupar imágenes relacionadas en una sola lámina. (C)
- Preferir gráfica de tiempo acumulado a tablas extensas, diferenciando por color medición y proyección. (C)
