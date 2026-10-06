# AGENTS.md

> Documento de **Diseño Superior** (docente: Ing. Ivan Mendoza). Mismo proyecto que la tesis de
> Taller de Grado I. El contenido heredado es base revisable: se reubica, adapta y amplía; no se
> descarta ni se reescribe desde cero (DS-001).

## Lectura inicial

Antes de trabajar:

1. `context/PROJECT_CONTEXT.md` — contexto estable del proyecto.
2. `context/DECISIONS.md` — decisiones vigentes, reemplazadas y asuntos no decididos.
3. `context/STATUS.md` — estado real, trabajo activo, pendientes y siguiente paso.

Según la tarea:

- `context/PROFESSOR_NOTES.md` — criterios del docente de Diseño Superior.
- `research/docente/criterios_taller_I.md` — criterios de Taller de Grado I, complementarios.
- `context/THESIS_STRUCTURE.md` — estructura DS: función, orden y profundidad de secciones.
- `research/referencias_estructurales/04_Referencia_Microsistema_Hidrostatico.md` — referencia estructural principal (documento DS).
- `redacción.md` — reglas de estilo y redacción académica del proyecto.
- `docs/template/Template_Diseno_Superior.md` — plantilla DS: estructura, numeración y recursos de cada sección.
- `docs/template/Template - Perfil de Proyecto- Final.md` — plantilla de Taller I; referencia de formato institucional donde DS no lo defina.
- `research/` — evidencia, registros, fuentes originales o referencias necesarias.

No leer `research/` completo por defecto.

## Prioridad ante conflictos

1. instrucción actual del usuario;
2. `context/DECISIONS.md`;
3. `context/PROFESSOR_NOTES.md` (DS);
4. `context/PROJECT_CONTEXT.md`;
5. fuentes originales de `research/`, incluidos los criterios de Taller I como aportes complementarios;
6. referencias estructurales (la 04 antes que las 01–03).

Si el conflicto no puede resolverse con estas fuentes, señalarlo. No elegir arbitrariamente.

Para estructura y numeración del documento DS prevalece `docs/template/Template_Diseno_Superior.md`,
aplicada al proyecto en `THESIS_STRUCTURE.md`. La revisión del docente puede ajustar la plantilla
(p. ej., objetivos por etapa del Modelo en V); si ambas difieren, señalarlo. El contenido del ejemplo
de la plantilla no se copia. La ref. 04 es un ejemplo de cómo se llena la plantilla.

Para redacción, aplicar `redacción.md` siempre que no contradiga decisiones,
criterios docentes o requisitos institucionales.

## Uso de `research/`

Consultar únicamente cuando la tarea requiera:

- datos, mediciones o cálculos detallados;
- verificar una afirmación o cifra;
- revisar la fuente original de una observación docente;
- obtener respaldo bibliográfico o técnico;
- resolver una inconsistencia;
- consultar referencias estructurales.

Las tesis de `research/referencias_estructurales/` son guía, no reglas obligatorias.

No trasladar contenido extenso de `research/` a `context/`.

## Reglas de trabajo

- No inventar datos, fuentes, mediciones, resultados ni decisiones.
- No cerrar asuntos marcados como abiertos o `NO DECIDIDO`.
- Distinguir **medición → cálculo derivado → proyección → hipótesis/requisito**.
- Consultar la fuente original cuando la precisión importe.
- Modificar solo archivos y secciones necesarios para la tarea.
- Preservar cambios existentes que no formen parte del encargo.
- Mantener coherencia entre texto, tablas, figuras, datos, referencias y decisiones vigentes.
- No redefinir problema, objetivos, alcance o solución técnica sin nueva evidencia o decisión explícita.
- No ejecutar `git commit`, `push`, `reset`, `rebase` ni operaciones destructivas salvo solicitud explícita.

## LaTeX

El documento fuente está en `docs/thesis/`.

Al modificar `.tex`:

- respetar la plantilla y estructura existentes;
- consultar `docs/template/Template_Diseno_Superior.md` y `context/THESIS_STRUCTURE.md` antes de cambiar estructura u organización;
- aplicar `redacción.md` cuando la tarea implique redacción académica;
- revisar antes patrones ya utilizados para figuras, tablas, ecuaciones, labels y referencias;
- usar `docs/thesis/bibliography/referencias.bib` como base bibliográfica;
- no añadir paquetes ni reorganizar archivos sin necesidad;
- comprobar referencias cruzadas y consistencia con figuras/tablas relacionadas;
- compilar cuando el entorno lo permita;
- corregir únicamente errores derivados del cambio realizado.

No modificar resultados o evidencia para hacerlos coincidir con una conclusión.

## Antes de terminar

Verificar:

- cumplimiento exacto de la solicitud;
- consistencia con `DECISIONS.md`;
- cumplimiento de criterios docentes aplicables;
- cumplimiento de requisitos institucionales aplicables;
- aplicación de `redacción.md` cuando corresponda;
- ausencia de datos o decisiones inventadas;
- coherencia de archivos relacionados;
- compilación LaTeX, si hubo cambios `.tex`;
- bloqueos, contradicciones o validaciones pendientes.

Informar brevemente:

- archivos modificados;
- cambios realizados;
- resultado de compilación, si aplica;
- pendientes o decisiones que requieran validación.

## Actualización de contexto

Después de una tarea, actualizar solo cuando corresponda:

- `STATUS.md` → cambió el estado real, trabajo activo, bloqueo o siguiente paso.
- `DECISIONS.md` → se tomó, reemplazó o descartó una decisión con impacto futuro.
- `PROJECT_CONTEXT.md` → cambió información estable y canónica del proyecto.
- `PROFESSOR_NOTES.md` → apareció un nuevo criterio docente activo y confirmado.
- `THESIS_STRUCTURE.md` → cambió una regla estructural vigente.

No actualizar contexto por cambios temporales ni duplicar información entre archivos.

Si el usuario restringió explícitamente la tarea a determinados archivos, respetar esa restricción y solo informar cualquier actualización de contexto que quede pendiente.

## Regla principal

**No inventar, no asumir y no modificar fuera del alcance solicitado.**