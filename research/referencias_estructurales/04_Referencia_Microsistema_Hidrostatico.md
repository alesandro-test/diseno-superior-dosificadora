# REFERENCIA ESTRUCTURAL — Microsistema hidrostático de transmisión de potencia para aplicaciones servoasistidas (Carhuaz, 2025)

> Documento de **Diseño Superior** (UCB Santa Cruz, junio 2025), no capítulo 1 de Taller de Grado. A diferencia de las referencias 01–03, cubre el perfil completo del proyecto.
> El archivo disponible contiene **texto solo hasta la sección 2 (Estudios preliminares)**; de las secciones 3–13 solo se conoce el índice. Lo que se dice de ellas se basa en títulos y paginación, no en su contenido.

## Estructura del documento

1. **Introducción** (sin numeración interna en el cuerpo)
   - 1.1 Problema y Justificación del Proyecto
     - 1.1.1 Metas de la empresa
     - 1.1.2 Objetivos de la empresa alineados al proyecto (Problemática de solución)
   - 1.2 Objetivos del proyecto
     - 1.2.1 Objetivo General
     - 1.2.2 Objetivos Específicos
   - 1.3 Alcance del Proyecto
   - 1.4 Metodología de Desarrollo del proyecto
2. **Estudios preliminares** (factibilidad / viabilidad / deseabilidad)
3. **Estado del Arte**
4. **Alcance del Proyecto** (repetido; ya existe 1.3)
5. **Diseño y Desarrollo Técnico Mecatrónico**
   - Árbol de objetivos del producto
   - Diagrama de caja negra
   - Requerimientos del producto: RF y RNF
   - Diseño de alto nivel: Casa de Calidad → Matriz morfológica → Diagrama de bloques → Estudio de alternativas → Definición de componentes
6. **Diseño Detallado**: modelos formales (cinemática), CAD, protocolos de control
7. **Verificación y Validación**: pruebas unitarias → integrales → funcionales → calidad y cumplimiento normativo → análisis de resultados → comparación diseño vs. real → validación del sistema
8. **Implementación y Prototipado**: fabricación → integración electrónica/control → evaluación del funcionamiento
9. **Conclusiones y Recomendaciones**
10. **Bibliografía**, **Anexos**, **Cronograma**

No existen apartados independientes de **Antecedentes**, **Motivación**, **Formulación del problema** ni **Límites** separados de Alcances. No hay **árbol de problemas**: su función la cumple un **diagrama de Ishikawa (6M)** más una **tabla de inconformidades**.

---

## Cómo construye cada sección

### 1. Introducción

- **Función:** contexto técnico, antecedentes tecnológicos y adelanto de objetivos y justificación.
- **Orden:** definición de la tecnología (HST) → aplicaciones industriales → funcionamiento básico y tipos de circuito → sistemas avanzados (regulación secundaria, recuperación de energía, control, digitalización) → salto a microescala (microbombas, aplicaciones biomédicas/robóticas) → resumen de objetivo general y específicos → justificación científica/tecnológica breve.
- **Evidencia:** exclusivamente bibliografía científica (citas autor-año en cadena). Sin estadísticas de mercado ni datos propios.
- **Recursos:** 2 figuras de circuitos tomadas/adaptadas de la literatura.
- **Conexión:** termina anticipando objetivos y justificación, que luego se repiten en 1.1 y 1.2.
- **Profundidad:** **media** (≈2 páginas). Embudo técnico: macro-HST → micro-HST.

### Antecedentes / Estado del arte

- **No aparecen en el capítulo 1** como sección propia; los antecedentes viven en la Introducción.
- Existe un **Estado del Arte separado (sección 3, ≈3 páginas)**, ubicado *después* de los estudios preliminares. Contenido no disponible en el archivo.

### 1.1 Problema y Justificación del Proyecto

Sección híbrida y la más extensa del capítulo (≈4 páginas). Orden interno:

1. **Justificación primero**, en tres ejes con viñetas: innovación tecnológica → cumplimiento normativo → fundamentación científica.
2. **Propósito del estudio** (un párrafo).
3. **Descripción del problema** con tres enfoques:
   - **Descriptiva textual:** viñetas cortas (ventajas, pérdidas, parámetros, repuestos, costos).
   - **Diagrama causa–efecto (Ishikawa 6M):** métodos, materiales, mano de obra, medio ambiente, máquinas, mediciones; cada M explicada en una viñeta y luego la figura de elaboración propia.
   - **Tabla de inconformidades:** filas = *característica: subcaracterística* de calidad (Funcionalidad, Fiabilidad, Usabilidad, Eficiencia, Mantenibilidad, Portabilidad) con la inconformidad concreta del sistema. Estas categorías coinciden con el modelo ISO/IEC 9126-1, pero **el documento no lo cita** (por verificar si el docente lo exige así).
- **Evidencia:** argumentos cualitativos; sin mediciones ni cifras.
- **Conexión:** cierra con un párrafo que propone el enfoque multidisciplinario y pasa a las metas de la empresa.

### 1.1.1 Metas de la empresa

- **Función:** situar el proyecto dentro de la visión de una empresa (aquí genérica, no nombrada).
- **Orden:** meta de la empresa → cómo el proyecto se alinea → atributos que aporta → posicionamiento.
- **Profundidad:** **baja** (2 párrafos).

### 1.1.2 Objetivos de la empresa alineados al proyecto

- **Función:** traducir las metas a **cualidades técnicas** que el producto debe tener.
- **Recurso:** lista de 5 cualidades (precisión, transmisión de potencia, velocidad, repetitividad, sostenibilidad), cada una con una frase.
- **Conexión:** estas cualidades anticipan los requerimientos y la Casa de Calidad de la sección 5.
- **Profundidad:** **baja**.

### 1.2.1 Objetivo General

- **Estructura:** verbo + producto + aplicación. Una línea, sin resultado medible.
- **Profundidad:** **muy baja**.

### 1.2.2 Objetivos Específicos

- **Orden:** **conceptualizar → determinar parámetros → diseñar → implementar → verificar**.
- **Lógica:** sigue el lado izquierdo y derecho del **Modelo en V** (requisitos/diseño → implementación → verificación). Cada objetivo incluye su finalidad ("con el fin de…").
- **Conexión:** se corresponde con las etapas de la metodología (1.4) y con las secciones 5–9.
- **Profundidad:** **baja** (5 viñetas largas).

### 1.3 Alcance del Proyecto

- **Función:** delimitar por **ejes**, no por Límites/Alcances.
- **Ejes:** técnico → funcional → normativo → temporal → de aplicación → de limitaciones.
- **Rasgo útil:** el eje de aplicación distingue **validación en laboratorio** de **aplicación comercial**; el eje de limitaciones dice qué *no* se hará (control adaptativo, embebidos complejos).
- **Profundidad:** **baja-media**.

### 1.4 Metodología de Desarrollo

- **Función:** declarar el Modelo en V y sus etapas.
- **Orden:** definición de requisitos → diseño conceptual y simulaciones → desarrollo de hardware/software → integración y pruebas → validación técnica (formato "Etapa → descripción").
- **Recursos:** no incluye figura del modelo en V en el texto disponible.
- **Profundidad:** **baja**.

### 2. Estudios preliminares

- **Función:** evaluar si el proyecto es posible, conveniente y deseado antes del diseño.
- **Recurso único:** **tabla de tres columnas** — Categoría | Pregunta de evaluación | Base de cumplimiento.
- **Organización:**
  - **Factibilidad (yo):** técnica, recursos, legal/normas, temporal.
  - **Viabilidad (empresa o cliente):** económica, operativa, riesgos, cronograma.
  - **Deseabilidad:** social, mercado/prioritario.
- **Evidencia:** declaraciones del autor; sin costos, cotizaciones ni datos de mercado.
- **Profundidad:** **media** (≈2 páginas, toda en tabla).

### 3–9. Secciones de desarrollo (solo índice)

- El peso del documento está en **Diseño y Desarrollo Técnico (≈16 páginas)**, más que en el capítulo 1 (≈9 páginas).
- La cadena de diseño es la típica de Diseño Superior: **árbol de objetivos → caja negra → RF/RNF → Casa de Calidad → matriz morfológica → diagrama de bloques → alternativas (matriz cualitativa y cuantitativa) → componentes**.
- V&V se ordena según el lado derecho del Modelo en V: unitarias → integrales → funcionales → normativas → comparación diseño/real → validación.

---

## Recursos utilizados

| Recurso | Uso estructural |
|---|---|
| Bibliografía científica en cadena | Contexto y antecedentes tecnológicos de la Introducción |
| Figuras de la literatura | Mostrar arquitecturas de referencia (circuitos) |
| Diagrama de Ishikawa 6M | Sintetizar causas del problema (en lugar del árbol de problemas) |
| Tabla de inconformidades por característica de calidad | Traducir el problema a deficiencias evaluables |
| Lista de cualidades de la empresa | Puente entre problema y requerimientos |
| Objetivos ligados al Modelo en V | Correspondencia objetivo ↔ etapa ↔ sección |
| Alcance por ejes | Delimitación técnica, normativa, temporal y de aplicación |
| Tabla factibilidad/viabilidad/deseabilidad | Estudios preliminares en un solo recurso |
| Herramientas de diseño (QFD, morfológica, bloques, alternativas) | Diseño de alto nivel (sección 5) |

---

## Patrones estructurales destacables

- **Formato de perfil de Diseño Superior**, no de capítulo de tesis: problema → empresa → objetivos → alcance → metodología → preliminares → estado del arte → diseño → V&V → implementación.
- **Introducción embudo técnico:** tecnología general → variantes avanzadas → microescala → propuesta.
- **Problema diagnosticado en tres capas:** texto → Ishikawa → tabla de inconformidades.
- **Capa "empresa":** metas y objetivos de la empresa convierten el problema en cualidades del producto, que luego alimentan los requerimientos.
- **Objetivos específicos alineados al Modelo en V**, con verbo distinto por etapa.
- **Alcance por ejes** que incluye las limitaciones dentro del mismo apartado.
- **Estudios preliminares como tabla de preguntas** con tres lentes: yo / empresa-cliente / sociedad-mercado.
- **Estado del arte separado y posterior** a los preliminares, no dentro de la Introducción.

---

## Particularidades y defectos a no replicar

- Numeración inconsistente en el índice (5.2 → 6.2.3 → 6.3; 7.4 sin 7.3; secciones que empiezan en 8.4, 9.4, 10.4) y marcadores rotos ("¡Error! Marcador no definido").
- **Alcance duplicado** (1.3 y sección 4).
- Objetivos y justificación **adelantados en la Introducción** y repetidos después.
- **Justificación antes del problema**, dentro del mismo apartado.
- "Cumplimiento normativo" afirmado en la justificación, mientras el Alcance normativo dice que las normas solo "se consideran" para una etapa posterior: **contradicción**. No afirmar cumplimiento sin demostrarlo.
- Fila "Riesgos" de la tabla 2.1 repite la pregunta y respuesta de "Operativa" (error de copia).
- Referencia residual "(Figura 8)" en el texto de la Figura 1.2.
- Empresa genérica sin nombre ni datos.
- Problema sin ninguna cifra ni medición propia.

---

## Esquema estructural condensado

```text
1. INTRODUCCIÓN
├── Tecnología general y aplicaciones
├── Funcionamiento y variantes
├── Desarrollos avanzados
├── Microescala / aproximación al proyecto
└── (adelanto de objetivos y justificación)

1.1 PROBLEMA Y JUSTIFICACIÓN
├── Justificación: innovación / normativa / científica
├── Propósito
└── Descripción del problema
    ├── Descriptiva textual
    ├── Ishikawa 6M
    └── Tabla de inconformidades (características de calidad)

1.1.1 METAS DE LA EMPRESA
1.1.2 OBJETIVOS DE LA EMPRESA → cualidades del producto

1.2 OBJETIVOS
├── General
└── Específicos: conceptualizar → determinar → diseñar → implementar → verificar

1.3 ALCANCE (por ejes)
└── técnico / funcional / normativo / temporal / aplicación / limitaciones

1.4 METODOLOGÍA → Modelo en V (5 etapas)

2. ESTUDIOS PRELIMINARES
└── Tabla: factibilidad (yo) / viabilidad (empresa) / deseabilidad

3. ESTADO DEL ARTE
5. DISEÑO: árbol de objetivos → caja negra → RF/RNF → QFD → morfológica → bloques → alternativas → componentes
6. DISEÑO DETALLADO: modelos, CAD, control
7. V&V: unitarias → integrales → funcionales → normativas → comparación → validación
8. IMPLEMENTACIÓN: fabricación → integración → evaluación
9. CONCLUSIONES Y RECOMENDACIONES
```