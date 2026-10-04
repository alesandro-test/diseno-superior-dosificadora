# Guía de redacción y revisión de la tesis

**Aplicación actual:** Marco Referencial / Capítulo 1.  
**Uso posterior:** adaptar la ficha de revisión a cada capítulo sin imponerle la función del Marco Referencial.  
**Estado:** guía operativa de redacción; no sustituye decisiones del proyecto ni una aprobación docente.

## 1. Fuentes y orden de consulta

1. Leer `AGENTS.md`, `context/PROJECT_CONTEXT.md`, `context/DECISIONS.md` y `context/STATUS.md` antes de revisar.
2. Para el Marco Referencial, consultar `context/PROFESSOR_NOTES.md`, `context/THESIS_STRUCTURE.md`, `docs/thesis/chapters/marcoref.tex`, `docs/thesis/main.tex`, `docs/thesis/preambles/imt_preamble.tex`, las figuras citadas y `docs/thesis/bibliography/referencias.bib`.
3. Abrir en `research/` únicamente el registro o la fuente original necesarios para comprobar una cifra, una atribución o una observación docente. Las tesis de referencia orientan la estructura; no fijan reglas obligatorias.
4. Ante discrepancias, aplicar la prioridad de `AGENTS.md`: instrucción actual del estudiante → decisiones vigentes → notas docentes → contexto canónico → fuente original → referencia estructural. Registrar las contradicciones sin resolverlas por suposición.

La revisión comprende **texto, tablas, figuras, ecuaciones, leyendas, citas y referencias cruzadas**. La plantilla institucional determina jerarquía de títulos, numeración, formato de figuras, bibliografía y presentación. Un cambio de estilo no justifica alterar cifras, objetivos, alcance ni decisiones abiertas.

## 2. Orden de trabajo recomendado

La guía `$thesis-writing` propone revisar primero el argumento y la estructura, y después la redacción de cada frase. En este proyecto, la secuencia operativa es:

1. **Función del apartado.** Comprobar que cada sección cumple el propósito descrito en `THESIS_STRUCTURE.md` y que la secuencia general es contexto → evidencia → formulación central → relaciones causales → objetivos → delimitación.
2. **Sustento.** Vincular cada afirmación cuantitativa con su registro, tabla, figura o fuente. Distinguir medición de campo, cálculo derivado, proyección e hipótesis o requisito propuesto. Mantener explícitos tamaño de muestra, condiciones y límites de inferencia.
3. **Coherencia transversal.** Comparar formulación, árbol, objetivo general, objetivos específicos, variables de evaluación y pruebas previstas. Una modificación de la formulación exige revisar todas esas piezas.
4. **Párrafos.** Identificar la idea principal de cada párrafo, su desarrollo con evidencia o razonamiento y un cierre técnico que conecte con el argumento. Dividir párrafos que mezclan funciones; unir fragmentos que no desarrollan una idea completa.
5. **Edición de frase.** Corregir sintaxis, léxico, semántica, puntuación, concordancia, referencias ambiguas y repetición. Aplicar las restricciones de estilo de la sección 3 sin perder precisión.
6. **Verificación final.** Revisar valores y unidades, consistencia entre texto y elementos gráficos, existencia de claves bibliográficas, referencias cruzadas y compilación de LaTeX si se modificó un `.tex`.

Trabajar una subsección por ciclo. La instrucción actual del estudiante determina el modo:

- **Diagnóstico o propuesta:** presentar una tabla breve con ubicación, fragmento original, hallazgo, propuesta, fundamento y validación pendiente; conservar el archivo fuente.
- **Edición autorizada:** aplicar las correcciones solicitadas, verificar citas y referencias y compilar. Una aprobación previa de la propuesta basta para incorporarla; no solicitar otra confirmación rutinaria.

Comparar original y propuesta para detectar cambios involuntarios en negaciones, orden de operaciones, condiciones, unidades, muestra y atribución de acciones. Mantener un único nombre para cada variable. Separar ajustes de redacción de cambios que afecten contenido o decisiones.

## 3. Criterios de redacción aportados por el estudiante

Estas reglas se aplican a la **prosa redactada de la tesis**. Una búsqueda automática produce candidatos para revisión, no errores confirmados: debe distinguir texto propio, nombres de fuentes, citas literales, títulos institucionales, expresiones técnicas, símbolos y código LaTeX.

| Aspecto | Revisión y acción |
|---|---|
| Adverbios y expresiones de cantidad | Señalar `absolutamente`, `apenas`, `mucho`, `bastante`, `casi`, `demasiado`, `extremadamente`, `justo`, `mitad`, `muy`, `nada`, `poco`, `tan`, `tanto`, `gran`, `altamente`, `suficiente`, `carece`, `no hay`, `no tiene`, `no existe`. Sustituir una valoración vaga por magnitud, criterio o descripción verificable. `Mitad` y otros vocablos de la lista pueden cumplir funciones gramaticales distintas; revisar el contexto. |
| Tiempo | Señalar `antes`, `después`, `luego`, `pronto`, `tarde`, `temprano`, `todavía`, `aún`, `aun`, `ya`, `ayer`, `hoy`, `mañana`, `anteayer`, `siempre`, `nunca`, `jamás`, `próximamente`, `prontamente`, `anoche`, `enseguida`, `ahora`, `anteriormente`. Cuando el orden del proceso importe, expresarlo con el nombre de las etapas o mediante una secuencia inequívoca. |
| Modo y duda | Señalar `así`, `bien`, `deprisa`, `de repente`, `súbitamente`, `despacio`, `difícilmente`, `especialmente`, `estupendamente`, `fácilmente`, `mal`, `mejor`, `peor`, `rápidamente`, `regular`, `sinceramente`, `solamente`, `probablemente`, `quizá`, `quizás`, `posiblemente`, `tal vez`, `acaso`, `a lo mejor`, `ojalá`, `creo`; revisar también `alto` y `bajo` cuando sean calificaciones vagas. Expresar alcance e incertidumbre mediante la evidencia y sus límites. |
| Modalidad, persona y posesión | Evitar `puede`, `debe`, `permite` y variantes modales; evitar `yo`, `tú`, `él`, `ella`, `nosotros`, `vosotros`, `ellos`, `ellas`, y posesivos como `mío`, `suyo`, `su`, `nuestro`. Nombrar el sistema, componente, procedimiento, registro o autor de la acción. No reemplazar una modalidad incierta con una afirmación categórica sin sustento. |
| Verbos y voz | Redactar en presente para descripción vigente y en pasado para observaciones y resultados registrados. Evitar futuro y gerundios. Priorizar sujeto técnico + verbo activo + objeto: «La balanza registró la cantidad final». La voz impersonal resulta admisible si identifica con claridad la acción y su alcance. |
| Calificativos | Eliminar elogios y publicidad (`revolucionario`, `innovador`, `el mejor del mercado`) y juicios como `elevado`, `excesivo`, `lento` o `deficiente` sin umbral o comparación. Conservar los adjetivos técnicos necesarios para identificar una variable o un componente. |
| Término «problema» | La regla compartida solicita evitarlo y usar `cumple/no cumple` o `conforme/no conforme`. **Existe un conflicto pendiente** con los títulos y criterios docentes del capítulo; ver sección 6. Esas parejas expresan el resultado de comparar con un requisito definido y no sustituyen automáticamente una condición central de investigación. |

La revisión léxica no consiste en cambiar una palabra prohibida por un sinónimo igual de vago. Se conserva el significado técnico: «Los siete ciclos registraron diferencias positivas» comunica un resultado; «el sistema no cumple» exigiría un criterio de aceptación que permanece abierto.

### Párrafos y conectores

Para cada párrafo de desarrollo, verificar tres movimientos: **oración principal → oraciones complementarias fundamentales → cierre técnico**. La oración principal enuncia una idea; el desarrollo aporta procedimiento, dato, fuente o relación; el cierre explica la consecuencia limitada por la evidencia o enlaza con la subsección. La conclusión no debe repetir la primera oración.

La indicación de aplicar esa estructura a párrafos de menos de ocho líneas se toma como **criterio de revisión**, no como una licencia para dejar párrafos más largos sin estructura. El conflicto entre límites de líneas y palabras se registra en la sección 6. Verificar la extensión en el PDF, no mediante las líneas del archivo `.tex`; no rellenar párrafos para alcanzar una cuota.

Usar conectores cuando expliciten una relación real. `De acuerdo con` introduce una fuente; `En consecuencia` expresa una inferencia sustentada; `Sin embargo` marca contraste; `A diferencia de` exige dos términos comparables. `Cabe destacar que` y `Esto implica que` pueden resultar redundantes: preferir la afirmación directa cuando el vínculo sea evidente. El ejemplo narrativo del «error» aportado por el estudiante ilustra la progresión idea → desarrollo → cierre, pero su tono personal y sus ejemplos literarios no constituyen modelo de prosa técnica para esta tesis.

### Modelo de párrafo ajustado al proyecto

> El relevamiento documentó siete ciclos del procedimiento manual de dosificación de harina. Los tiempos del procedimiento estuvieron entre 53,2 y 66,6 s por ciclo, de acuerdo con los registros de campo. Este intervalo caracteriza la muestra estudiada dentro de los límites definidos para cada ciclo.

El ejemplo usa mediciones ya documentadas; no afirma que el tiempo sea excesivo ni anticipa una mejora del prototipo. Al incorporarlo al documento, enlazar la afirmación con el registro, tabla o apéndice correspondiente.

## 4. Aplicación al Marco Referencial

Consultar la función, el orden y la profundidad de cada apartado en `context/THESIS_STRUCTURE.md`; no duplicar aquí esa estructura. Leer el capítulo y sus dependencias reales en cada revisión. El diagnóstico del borrador inicial fue retirado de esta guía porque incluía observaciones ya corregidas y referencias a una versión anterior del croquis.

Comprobar en especial:

- Que la Introducción sitúe empresa, proceso y dosificación; concentrar la evidencia detallada en Antecedentes.
- Que el procedimiento narrado coincida con el diagrama, el croquis, los límites de medición y los registros.
- Que formulación, árbol y objetivos mantengan la línea vigente de intervención del operario y tiempo asociado; la aprobación académica se consulta en `DECISIONS.md`.
- Que los antecedentes tecnológicos se presenten con el alcance que respalda cada fuente. Una premezcla de ingredientes no equivale a dosificación de harina; una celda de carga citada no constituye una selección del proyecto.
- Que tiempo total de ciclo y tiempo de intervención no se traten como equivalentes sin definición y respaldo, en especial al comparar el prototipo con el procedimiento manual.

Registrar resultados de revisiones y verificaciones en las notas pertinentes de `research/notes/`; actualizar `STATUS.md` cuando cambie el trabajo real. Esta guía contiene el método, no un historial de errores ni una certificación del capítulo.

## 5. Lista de aceptación para cada subsección

- [ ] Cumple la función y profundidad previstas en `THESIS_STRUCTURE.md`.
- [ ] El lector identifica la idea principal y su relación con la subsección siguiente.
- [ ] Cada afirmación técnica o cuantitativa tiene respaldo localizable y una interpretación proporcional a la evidencia.
- [ ] Mediciones, cálculos, proyecciones y requisitos propuestos están rotulados de manera distinta.
- [ ] Se mantienen coherentes terminología, cantidades, unidades, tabla, figura, leyenda, apéndice y texto.
- [ ] El párrafo contiene idea, desarrollo y cierre; no acumula hechos inconexos.
- [ ] Se revisaron adverbios, gerundios, modalidad, posesivos, persona, futuro, calificativos y repeticiones según la sección 3.
- [ ] Las citas respaldan las frases concretas a las que se adjuntan; las claves bibliográficas existen.
- [ ] Los títulos y referencias cruzadas siguen la plantilla; el documento compila si se cambió LaTeX.
- [ ] Los asuntos `NO DECIDIDO` permanecen abiertos y se anotan para validación.

## 6. Decisiones de estilo que requieren validación

1. **Uso de «problema».** La prohibición aportada por el estudiante entra en conflicto con la nomenclatura vigente del capítulo y los criterios del docente, que exigen formulación y árbol de problemas. `Cumple/no cumple` o `conforme/no conforme` solo describen una evaluación frente a un criterio explícito. Hasta aclarar el alcance de la prohibición, **conservar los títulos y conceptos estructurales actuales**, y evitar usos redundantes de la palabra en la prosa cuando la precisión no se pierda. Esta pauta de conservación es provisional; no registra una decisión académica nueva.
2. **Extensión en líneas y palabras.** Se aportaron 50–100 palabras con máximo cuatro líneas para párrafos introductorios/conclusivos y 100–200 palabras con máximo doce líneas para descriptivos, además de una referencia a ocho líneas. No se ha resuelto qué límite prevalece cuando resultan incompatibles en la plantilla. Registrar ambas medidas y señalar el conflicto; no declarar cumplimiento formal ni modificar tipografía o márgenes para forzarlo.
3. **Aplicación gramatical.** Los infinitivos de los objetivos (`determinar`, `diseñar`, `evaluar`) no son verbos en futuro. Nombrar al operario como sujeto de una acción observada respeta la tercera persona y conserva la trazabilidad. Aplicar las listas de la sección 3 según la función de cada palabra; no eliminarlas dentro de comandos, nombres bibliográficos o términos técnicos.

## 7. Instrucción reutilizable para próximas revisiones

> Revisa la subsección indicada de la tesis con `redacción.md`, `AGENTS.md`, las decisiones vigentes, las notas docentes, la estructura del capítulo, el LaTeX y sus figuras, tablas, apéndices y bibliografía relacionados. Primero informa los hallazgos de argumento, evidencia y coherencia; después presenta una propuesta de redacción en el formato existente. Conserva cifras, fuentes, decisiones abiertas, alcance, citas y referencias. Distingue medición, cálculo, proyección e hipótesis o requisito. Aplica las restricciones de estilo del estudiante con revisión contextual. Señala cada contradicción que requiera decisión y verifica la compilación si modificas LaTeX.

Para otros capítulos, reemplazar `THESIS_STRUCTURE.md` por la función aprobada del capítulo correspondiente y ajustar la revisión macro: marco teórico por síntesis de ideas y fuentes, metodología por reproducibilidad y justificación de decisiones, resultados por reporte verificable, y discusión por interpretación y límites. La plantilla y las decisiones del proyecto permanecen como referencias comunes.

## 8. Referencias externas de edición y adaptación al proyecto

**Consulta:** 13/09/2026. Estas referencias aportan criterios editoriales; no constituyen fuentes técnicas de la dosificadora ni sustituyen la jerarquía de la sección 1. Esta incorporación resume y adapta ideas; no instala los repositorios ni activa sus instrucciones completas. Para este proyecto se recomienda usar esta guía como punto de entrada, junto con `$thesis-writing`, disponible en el entorno. Instalar `academic-humanizer` es opcional y no aporta por sí mismo otra validación de datos o citas. Si se instala en el futuro, seguir las adaptaciones de esta sección y evitar dos revisiones consecutivas que repitan los mismos criterios.

| Referencia consultada | Aporte seleccionado | Adaptación |
|---|---|---|
| [academic-humanizer, AIScientists-Dev, v0.3.3](https://github.com/AIScientists-Dev/academic-humanizer/blob/94b88b2/SKILL.md) | Revisar la fuerza de cada afirmación frente a su evidencia y conservar incertidumbre, cifras y citas. | Base externa preferida para la edición académica. Mantener el estilo impersonal exigido en este proyecto. |
| [humanizer, blader, v3.0.0](https://github.com/blader/humanizer/blob/9862685/SKILL.md) | Detectar relleno, contrastes artificiales, cierres repetitivos y cambios de significado durante la reescritura. | Aplicar como revisión final de claridad. Mantener el registro técnico y la estructura institucional. |
| [manuscript-writing, YSLAB-ai](https://github.com/YSLAB-ai/manuscript-writing) | Distinguir revisión con observaciones de edición del texto; identificar evidencia pendiente. | Referencia complementaria para presentar propuestas. Sus ejemplos no validan el desempeño sobre esta tesis. |

`academic-humanizer` reconoce que reutiliza parte del catálogo de `blader/humanizer`; no son dos enfoques completamente independientes. [Procedencia declarada](https://github.com/AIScientists-Dev/academic-humanizer#acknowledgments).

### Reglas externas que no se adoptan literalmente

- La conservación de `we` indicada por `academic-humanizer` contradice el registro solicitado aquí. Además, su descripción de `we` como tercera persona plural contiene un error: corresponde a primera persona plural.
- La misma guía exige mantener el número de párrafos. En este proyecto se conserva la información sustentada y se justifica cualquier división o unión por la función del párrafo.
- El modo de propuestas NSF/NIH no determina la estructura de una tesis UCB.
- Ningún ejemplo externo aporta mediciones, comparaciones o citas al proyecto. Si falta respaldo, registrar la carencia de evidencia en el informe de revisión; una frase atenuada tampoco prueba una afirmación.
- Los catálogos en inglés requieren revisión contextual en español. No borrar signos de intervalos, términos técnicos o títulos por coincidir con un patrón estilístico.

### Cómo juzgar la utilidad de una guía

Las estrellas indican popularidad, pero no verifican fidelidad científica. Evaluar instrucciones legibles, historial de correcciones, ejemplos pertinentes, respeto por evidencia y formato, y compatibilidad con el español y los criterios docentes. Los repositorios consultados no aportan, en las páginas revisadas, una comparación que establezca cuál produce mejores tesis de ingeniería en español.

La prueba útil para este proyecto consiste en revisar un mismo fragmento con la guía vigente y con la adaptación propuesta. Comparar exactitud, trazabilidad, claridad, coherencia y adecuación al docente. Rechazar cambios que inventen respaldo, borren límites de la muestra, confundan tiempo total con intervención o conviertan proyecciones en resultados medidos. La cantidad de palabras eliminadas y una puntuación de detector de IA no son criterios de aceptación del capítulo.
