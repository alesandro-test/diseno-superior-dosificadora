# STATUS

**Última actualización:** 2026-09-16

## Estado actual

Marco Referencial / Capítulo 1 en revisión a partir de las observaciones docentes más recientes.  
Introducción, diagnóstico, problema/árbol, objetivos, alcance/límites y el criterio de `bajo costo` no están cerrados. Trabajo activo: **Antecedentes del problema / diagnóstico**.

## Completado

- Resultados del diagnóstico condensados: tabla consolidada, explicación directa de cantidades y tiempos y proyecciones con repetición de ciclos explícita. Por solicitud del estudiante, se retiró la gráfica de barras y se redujo el texto a cuatro párrafos; sin incorporar tabla por ciclos. PDF compilado y páginas afectadas revisadas el 16/09/2026.

- Fotografías de Antecedentes maquetadas junto a sus explicaciones; diagrama, croquis y tabla ajustados. PDF compilado y páginas afectadas revisadas visualmente el 14/09/2026.

- `PROJECT_CONTEXT.md`, `DECISIONS.md`, `PROFESSOR_NOTES.md` y `THESIS_STRUCTURE.md` consolidados.
- Relevamiento disponible del 02/09/2026 y 05/09/2026 documentado y centralizado en `research/notes/contexto_tesis_san_miguel.md`.
- Introducción propuesta en la revisión de redacción incorporada; compilación LaTeX correcta el 13/09/2026.
- Componentes de Farihin verificados en el artículo original; respaldo y límites de uso registrados en `research/notes/antecedentes_tecnologicos_dosificacion.md`.
- `redacción.md` depurado como guía reutilizable, con las adaptaciones pertinentes de referencias externas.

## En curso

- Organizar **Antecedentes del problema / diagnóstico** con la evidencia existente, mejorar la presentación del impacto y calcular proyecciones acumuladas diaria, semanal y mensual, identificándolas expresamente como proyecciones.
- Completar la auditoría del respaldo del diagnóstico; la explicación de la tabla consolidada y la distribución temporal ya fueron revisadas.

## Próximos pasos

1. **01C — Introducción y antecedentes:** presentar primero la problemática/necesidad y después la solución; trasladar la revisión detallada de dosificadoras al estado del arte; revisar paráfrasis, citas, atribuciones y repeticiones.
2. **01A — Diagnóstico y problema:** consolidar proceso → DFD → distribución/recorridos → cantidades/tiempos/diferencias → proyecciones → análisis; integrar tiempo/intervención + diferencia/exceso de harina y revisar el árbol con la estructura causas → problema → efectos. Representar el problema central en un único cuadro.
3. **01B — Objetivos y alcance:** simplificar el objetivo general y el objetivo específico de evaluación; comprobar medibilidad, logro verificable y secuencia; mantener la validación después del desarrollo; volver a revisar el primer OE, cuya aprobación no puede establecerse.
4. **01B — Alcances y límites:** rehacer los alcances como fronteras funcionales/técnicas y depurar los límites para conservar solo exclusiones reales, sin adoptar `50 kg` ni otro rango sin sustento.
5. **02 — Investigación:** obtener precios o cotizaciones verificables de soluciones comerciales de funcionalidad comparable y reunir sus prestaciones para sustentar el criterio de `bajo costo`; preparar una comparación explícita de prestaciones y costo, preferentemente mediante tabla.
6. **03 — Diagramas y tablas:** conectar la descripción del procedimiento manual con el diagrama correspondiente; asegurar contexto, títulos, unidades, leyendas, atribución e interpretación; revisar específicamente la referencia al inciso señalado de la Figura 1.1 y corregir el tamaño de fuente de la tabla de registro de tiempos del apéndice, manteniendo consistencia con las demás tablas.
7. Verificar que el documento use el template oficial de Taller de Grado I.

## Bloqueos / pendientes de validación

- La formulación y el árbol presentan cifras mensuales sin explicitar su carácter proyectado; revisión pendiente fuera de la edición de resultados. Las notas de campo consideran provisional la asociación entre fechas temporales y lecturas de harina: confirmar trazabilidad sin alterar cifras por suposición.

- Problema, árbol y objetivos presentados el 11/09/2026 aún no tienen aprobación definitiva.
- `D-004` requiere revisión después de reconstruir `01A`; no debe reemplazarse todavía.
- El título de `main.tex` usa **“bajo costo / panaderías artesanales”**, pero el título definitivo continúa **NO DECIDIDO** y `bajo costo` aún debe demostrarse mediante un criterio comparativo.
- La revisión de Introducción no implica aprobación docente del capítulo; debe reestructurarse para presentar primero la problemática.
- Alcances y límites requieren revisión sustancial: los primeros no deben formularse como objetivos/entregables y los segundos deben contener solo exclusiones reales.
- Tablas y figuras requieren revisión de contexto, unidades, leyendas, explicación e interpretación; la evidencia principal debe permanecer en el cuerpo.
- Debe verificarse el uso del template oficial de Taller de Grado I.
- Persisten los conflictos de estilo sobre títulos con «problema» y límites simultáneos de líneas/palabras registrados en `redacción.md`.
- Problema, árbol y objetivos aún no cuentan con aprobación definitiva.
- La situación del primer objetivo específico permanece pendiente de validación; la evidencia disponible no permite establecer su aprobación o rechazo definitivo.
- Debe confirmarse con el docente el tipo de diagrama requerido; no asumir que la expresión `flujo de datos` exige formalmente un DFD.

## Archivos activos

- `docs/thesis/chapters/marcoref.tex`
- `docs/thesis/main.tex`
- `research/notes/contexto_tesis_san_miguel.md`
- `context/DECISIONS.md`
- `context/PROFESSOR_NOTES.md`
