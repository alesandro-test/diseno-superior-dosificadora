# DECISIONS

> Registro compacto de decisiones del proyecto que afectan el trabajo futuro.
>
> No contiene datos experimentales detallados, estado de avance, notas del docente
> ni instrucciones operativas de los agentes.
>
> Estados utilizados:
>
> - **Confirmada:** decisión vigente.
> - **Reemplazada:** decisión anterior sustituida por otra.
> - **Descartada:** alternativa evaluada y rechazada.
> - **NO DECIDIDO:** asunto que no debe asumirse como resuelto.

---

## Decisiones vigentes

### D-001 — Función de las fuentes internas

**Estado:** Confirmada  
**Decisión:** Utilizar cada fuente según su función: `PROJECT_CONTEXT.md` como contexto canónico compacto; `research/notes/contexto_tesis_san_miguel.md` para registros y cálculos detallados; y el PDF presentado al docente como referencia de la versión académica efectivamente presentada.  
**Motivo:** Las fuentes tienen distinto nivel de detalle y fecha de elaboración.  
**Impacto:** Una fuente no debe sustituir automáticamente a otra fuera de su función. Si dos fuentes contienen datos incompatibles y no existe una corrección explícita, el conflicto debe señalarse y verificarse en lugar de resolverse por suposición.

---

### D-002 — Alcance técnico del proyecto

**Estado:** Confirmada  
**Decisión:** El desarrollo se delimita a la dosificación de harina previa al mezclado y amasado.  
**Motivo:** Es la operación específicamente seleccionada para el proyecto.  
**Impacto:** Mezclado, división, formado, fermentación, cocción y automatización integral de la panadería no forman parte del desarrollo principal. El proceso general de panificación puede utilizarse únicamente como contexto.

---

### D-003 — Versión académica de referencia

**Estado:** Confirmada  
**Decisión:** Para la formulación del problema, árbol de problemas y objetivos se toma como versión de referencia la presentada en el PDF del 11/09/2026.  
**Motivo:** Es la versión efectivamente preparada y presentada académicamente más reciente de estos apartados.  
**Impacto:** No regresar silenciosamente a formulaciones anteriores. Esta decisión establece precedencia de versión, pero NO implica que el contenido haya sido aprobado definitivamente por el docente.

---

### D-004 — Variable central de la formulación presentada

**Estado:** Confirmada  
**Decisión:** En la versión académica actualmente presentada, la intervención directa del operario y el tiempo asociado al procedimiento manual constituyen la línea central del planteamiento. La diferencia de harina permanece como variable de evaluación, no como sustituto automático del problema central.  
**Motivo:** Así se encuentra estructurado el planteamiento, árbol y formulación presentados.  
**Impacto:** No redefinir el problema únicamente alrededor de exceso, error o diferencia de harina sin nueva evidencia o revisión académica.

**Revisión requerida:** La observación docente más reciente exige reconsiderar la formulación y el árbol integrando conjuntamente tiempo/intervención del operario y diferencia/exceso de harina. Esta anotación no reemplaza la decisión vigente: primero debe reconstruirse `01A — Diagnóstico y problema` y verificarse su coherencia con la evidencia; solo después corresponde registrar una decisión actualizada.

---

### D-005 — Concepto general de la solución

**Estado:** Confirmada  
**Decisión:** La solución propuesta será un prototipo automatizado de dosificación gravimétrica de harina, capaz de trabajar con una cantidad objetivo y medir la cantidad dosificada para controlar el proceso de alimentación.  
**Motivo:** Es el principio funcional adoptado para el proyecto.  
**Impacto:** Esta decisión define el concepto de solución, pero NO define todavía mecanismo de alimentación, accionamiento, sensores, controlador, actuadores ni estrategia de control.

---

### D-006 — Tratamiento de la evidencia

**Estado:** Confirmada  
**Decisión:** Distinguir siempre entre medición de campo, cálculo derivado, proyección e hipótesis o requisito propuesto.  
**Motivo:** Cada categoría posee distinto nivel de evidencia.  
**Impacto:** No inventar mediciones faltantes, reconstruir datos mediante supuestos ni presentar cálculos o proyecciones como observaciones reales.

---

### D-007 — Terminología e interpretación

**Estado:** Confirmada  
**Decisión:** Para el ingrediente utilizar preferentemente `harina`, `cantidad objetivo de harina`, `cantidad dosificada` y `diferencia de harina`. Reservar `masa` para la masa de panificación cuando corresponda.  
**Motivo:** Evitar ambigüedad entre la harina dosificada y la masa elaborada posteriormente.  
**Impacto:** No denominar automáticamente `desperdicio` a una diferencia positiva de harina ni `tiempo perdido` al tiempo empleado por el operario sin evidencia que sustente esas interpretaciones.

---

### D-008 — Evaluación del prototipo

**Estado:** Confirmada  
**Decisión:** El desempeño del prototipo deberá evaluarse experimentalmente frente al procedimiento manual bajo condiciones comparables.  
**Motivo:** Las mejoras del sistema no pueden asumirse antes de construirlo y medirlo.  
**Impacto:** Tiempo, intervención del operario, diferencia respecto de la cantidad objetivo y repetibilidad deberán obtenerse mediante ensayos; no deben presentarse como mejoras garantizadas durante la etapa de diseño.

---

### D-009 — Parámetros técnicos todavía abiertos

**Estado:** Confirmada  
**Decisión:** Las selecciones técnicas y los requisitos numéricos que aún no estén fundamentados permanecen abiertos.  
**Motivo:** Deben derivarse del relevamiento, bibliografía, requerimientos de diseño y validación posterior.  
**Impacto:** No asumir como definitivos mecanismo de alimentación, accionamiento, capacidad de almacenamiento, rango final, sensores, controlador, actuadores, estrategia de control, tolerancia, tiempo objetivo, arquitectura mecánica/electrónica ni dimensiones.

Las referencias históricas de **5–15 kg**, **40–50 kg** y **+20 g** son únicamente antecedentes o propuestas previas y NO constituyen requisitos vigentes.

---

## Decisiones abiertas

Los siguientes asuntos están **NO DECIDIDOS** y ningún agente debe cerrarlos sin nueva evidencia, decisión del estudiante o indicación docente.

### A-001 — Título definitivo

**Estado:** NO DECIDIDO

Existen actualmente formulaciones diferentes entre `PROJECT_CONTEXT.md` y el PDF presentado.

También permanece abierto si las expresiones `bajo costo` y `panaderías artesanales`
formarán parte del título o de los requerimientos definitivos.

La revisión docente más reciente no aprueba definitivamente el título. Si se conserva
`bajo costo`, debe definirse previamente un criterio comparativo defendible frente a
soluciones comerciales de funcionalidad comparable, considerando prestaciones y precio.

---

### A-002 — Aprobación definitiva del problema, árbol y objetivos

**Estado:** NO DECIDIDO

El PDF del 11/09/2026 constituye la versión académica presentada de referencia,
pero no existe evidencia suficiente para registrarla como aprobación definitiva del docente.

La revisión docente más reciente requiere correcciones sustanciales en problema,
árbol y objetivos; por tanto, estos apartados deben permanecer abiertos.

---

### A-003 — Cobertura final del relevamiento

**Estado:** NO DECIDIDO

El plan previo contemplaba dos jornadas ordinarias y un sábado, mientras que la
versión presentada del objetivo específico utiliza una jornada ordinaria y una jornada
de sábado.

No asumir que el segundo día ordinario fue eliminado formalmente hasta disponer
de una confirmación o decisión explícita.

---

### A-004 — Selecciones y requisitos técnicos finales

**Estado:** NO DECIDIDO

Continúan abiertos, entre otros:

- mecanismo de alimentación;
- tipo de accionamiento;
- capacidad de almacenamiento;
- rango final de dosificación;
- sensores;
- controlador;
- actuadores;
- estrategia de control;
- tolerancia de aceptación;
- tiempo objetivo;
- arquitectura mecánica;
- arquitectura electrónica;
- dimensiones finales.

Una propuesta, ejemplo bibliográfico, valor observado o valor utilizado en un
borrador no convierte automáticamente ninguno de estos elementos en requisito.

El ejemplo docente de `50 kg` fue únicamente pedagógico y no constituye un
requerimiento del prototipo. El rango deberá derivarse de los datos de campo y del diseño.
