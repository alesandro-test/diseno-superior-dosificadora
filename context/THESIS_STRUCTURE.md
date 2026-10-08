# THESIS_STRUCTURE — Diseño Superior

> Lectura aplicada al proyecto de la plantilla DS (`docs/template/Template_Diseno_Superior.md`).
> Complementos: revisión del docente del 29/09/2026 (`research/docente/revision_DS_2026-09-29.md`)
> y ejemplo completo `research/referencias_estructurales/04_Referencia_Microsistema_Hidrostatico.md`.
> Estructura de Taller I archivada en `research/docente/estructura_taller_I.md`.
>
> Principio: **mismo proyecto, otra organización** (DS-001). El contenido de `marcoref.tex`
> se reubica y adapta; no se reescribe desde cero ni se descarta evidencia.
> Etiquetas: **[P]** plantilla · **[R]** revisión del docente · **[A]** adaptación propuesta, por confirmar.

## Índice del documento

```text
Portada ............................................ fecha: diciembre [R]
1. Introducción .................................... ¿qué? ¿quién? ¿con qué? ¿para qué? [P]; macro → micro [R]
   1.1 Metas de la empresa
   1.2 Objetivos de la empresa alineados al proyecto (problemática de solución)
   1.3 Problema y justificación del proyecto
   1.4 Objetivos del proyecto
       1.4.1 Objetivo general
       1.4.2 Objetivos específicos (Modelo en V)
   1.5 Alcance del proyecto (por ejes)
   1.6 Metodología de desarrollo del proyecto
2. Estudios preliminares (factibilidad, viabilidad, deseabilidad)
3. Estado del arte
4. Diseño y desarrollo técnico mecatrónico
   4.0 Contextualización del sistema actual [R][A]
   4.1 Árbol de objetivos del producto
   4.2 Diagrama de caja negra y caja transparente
   4.3 Requerimientos del producto (4.3.1 RF · 4.3.2 RNF)
5. Diseño de alto nivel
   5.1 Casa de calidad · 5.2 Matriz morfológica · 5.3 Diagrama de bloques
   5.4 Estudio de alternativas · 5.5 Definición de componentes
6. Diseño detallado
   6.1 Modelos formales (matemáticos) · 6.2 Modelos CAD · 6.3 Protocolos de control
7. Verificación y validación
8. Implementación y prototipado
   (+ Transferencia y operación [R][A])
9. Conclusiones y recomendaciones
10. Bibliografía (ISO 690 [P])
11. Apéndices / anexos
```

## Capítulo 1

### 1. Introducción (texto inicial)
- **Función:** presentar qué se desarrolla, para quién, con qué base y para qué. [P]
- **Orden:** rubro de panaderías y pastelerías y su papel para la población (1–2 párr.) → Panadería San Miguel: productos, mercados, datos externos (1–2 párr.) → etapa estudiada (dosificación de harina) y concepto de solución gravimétrica, en forma breve. [R]
- **Evidencia:** fuentes externas y bibliografía; sin mediciones propias, recetas ni flujos de planta. [R]
- **Profundidad:** media (≈1,5–2 páginas).
- **No replicar (ref. 04):** adelantar y repetir objetivos o justificación.

### 1.1 Metas de la empresa
- **Función:** meta de la Panadería San Miguel y cómo se alinea el proyecto. [P]
- **Evidencia:** información de la propia panadería (entrevista o comunicación documentada). No inventar metas.
- **Profundidad:** baja (1–2 párr.).

### 1.2 Objetivos de la empresa alineados al proyecto
- **Función:** traducir las metas en desafíos y cualidades que el producto debe atender (p. ej., precisión, repetibilidad, menor intervención). [P]
- **Recurso:** lista breve de desafíos o cualidades; anticipa requerimientos y casa de calidad.
- **Profundidad:** baja.

### 1.3 Problema y justificación del proyecto
- **Fórmula del problema:** [variable independiente] + [efecto en la variable dependiente] + [condiciones] + [contexto]. [P]
- **Tres representaciones:** [P][R]
  1. **Descriptiva textual:** condiciones del proceso con cifras clave y su respaldo (remitir a 4.0 y anexos).
  2. **Diagrama causa-efecto (Ishikawa):** reutilizar causas y efectos del árbol de problemas actual.
  3. **Tabla de inconformidades:** característica: subcaracterística de calidad (ISO 9126 / ISO/IEC 25010 u otra) → inconformidad, con la especificación de referencia que se incumple.
- **Oración del problema:** imprecisión + falta de estandarización + uso no óptimo de recursos, sobre el proceso, no el operario. [R]
- **Justificación:** en ejes breves dentro de esta sección [P]; priorizar la económica con precios puestos en Bolivia; la tecnológica solo si hay tecnología nueva. [R]
- **No replicar (ref. 04):** afirmar cumplimiento normativo sin demostrarlo; problema sin cifras.

### 1.4 Objetivos
- **Objetivo general:** verbo + qué + para qué + con qué (base científica, técnica, normativa) [P]; responde a la oración del problema. [R]
- **Objetivos específicos por etapa del Modelo en V:** [R]
  contextualizar → determinar requerimientos → diseñar modelos detallados → implementar → verificar → validar → mantener/operar.
  (El ejemplo de la plantilla inicia en «especificar requerimientos»; prevalece la revisión del docente.)

### 1.5 Alcance (por ejes)
- **Ejes:** técnico · funcional · normativo · temporal · de usuarios · de limitaciones. [P]
- **Contenido:** capacidad útil, dimensiones, número de pruebas, condiciones de validación [R]; valores solo si están sustentados (D-009).
- **Limitaciones:** los límites actuales pasan a este eje.

### 1.6 Metodología de desarrollo
- Modelo en V (y, si aplica, PDCA/RUP como en la plantilla) [P]; etapas en formato «etapa → descripción»; correspondencia etapa ↔ objetivo ↔ capítulo. Figura del modelo recomendable.

## Capítulos 2–11

### 2. Estudios preliminares
- Tabla única: **factibilidad** (el autor: técnica, recursos, cronograma) · **viabilidad** (la panadería: económica, operativa, cronograma) · **deseabilidad** (valor social, ambiental, competitivo). [P] La columna «base de cumplimiento» resuelve el cumple / no cumple; sin columna de evaluación aparte (decisión del estudiante, 2026-10-08).

### 3. Estado del arte
- **30** proyectos o productos (académicos, comerciales, patentes). [P]
- **Criterios de inclusión/exclusión** explícitos (p. ej., año, costo, tiempo de parada). [P]
- Por elemento: problema, objetivo, resultados (académicos); objetivo, garantías, costos, mantenimiento, importación (comerciales). [P]
- Tabla comparativa de precio puesto en Bolivia, mantenibilidad, eficiencia y ventaja de la propuesta. [R]

### 4. Diseño y desarrollo técnico mecatrónico
- **4.0 Contextualización [R][A]:** proceso de elaboración del pan, proporciones, características de la harina (tamaño de grano, densidad), máquinas existentes, distribución de planta, procedimiento manual, mediciones del relevamiento («argumento con datos»). Ubicación por confirmar con el docente.
- **4.1 Árbol de objetivos del producto** (cómo / por qué). [P]
- **4.2 Caja negra y caja transparente** (energía, materia, señales; subfunciones). [P]
- **4.3 RF y RNF:** tablas ID | requerimiento | O/D (obligatorio/deseable) | descripción | valor técnico o norma. [P]

### 5. Diseño de alto nivel
- Casa de calidad (QFD) → matriz morfológica con caminos y justificación → diagrama de bloques → matriz cualitativa y cuantitativa de alternativas → definición de componentes. [P]

### 6. Diseño detallado
- Modelos formales (matemáticos del proceso de dosificación) · CAD · protocolos y estrategia de control. [P][R] Ver A-007.

### 7. Verificación y validación
- **Verificación:** tabla ID RF/RNF | requerimiento | diseño final | cumple / no cumple; pruebas unitarias, integrales, funcionales y de cumplimiento normativo; análisis de resultados; diseño vs. real. [P]
- **Validación:** frente a requerimientos y frente al procedimiento manual bajo condiciones comparables (D-008).

### 8. Implementación y prototipado
- Fabricación · integración electrónica y de control · evaluación del funcionamiento. [P]
- **Transferencia y operación [R][A]:** mantenimiento, operación y control.
- Nota: la plantilla numera Implementación después de V&V; aclarar el orden real del Modelo en V en 1.6 o consultar.

### 9–11.
- Conclusiones y recomendaciones · Bibliografía en ISO 690 [P] (verificar compatibilidad con el estilo biblatex actual) · Anexos: planos, cálculos, registros, código.

## Reubicación del contenido actual de `marcoref.tex`

| Contenido actual | Destino en DS |
|---|---|
| Introducción: caso de estudio, proceso general del pan (Cauvain), figura, OIML R 61-1, enfoque | 1. Introducción (se conserva; se agrega bloque macro) |
| Introducción: párrafo de registros de campo y diferencias | 1.3 Problema (textual) o 4.0 |
| Antecedentes: procedimiento, DFD, croquis, fotografías, recorridos | 4.0 Contextualización |
| Antecedentes: tablas de cantidades y tiempos, proyecciones | 4.0 (argumento con datos); cifras clave citadas en 1.3; registros a anexos |
| Formulación del problema | 1.3 Oración del problema (sobre el proceso) |
| Árbol de problemas | 1.3 Ishikawa (reutilizar causas y efectos) |
| Objetivos | 1.4 (reordenar según Modelo en V) |
| Justificación tecnológica / social / económica | 1.3 Justificación (revisar tecnológica; reforzar económica) |
| Límites y alcances | 1.5 Alcance por ejes (límites → eje de limitaciones) |
| Tabla RUICHUAN / Trust-Long | 1.3 justificación económica y 3. Estado del arte |

## Reglas transversales

- **medición → cálculo derivado → proyección → hipótesis/requisito** (D-006).
- Trazabilidad **problema → objetivo → requerimiento → verificación/validación**.
- No convertir tecnologías ni ausencia de automatización en el problema.
- No asumir parámetros técnicos abiertos (D-009, A-004); los «valores técnicos esperados» de RF/RNF deben derivarse de datos, normas o bibliografía.
- No copiar contenido ni valores del ejemplo de la plantilla.
- Registros extensos a anexos, con remisión expresa desde el cuerpo.
