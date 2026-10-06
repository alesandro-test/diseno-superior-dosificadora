# PLANTILLA — DISEÑO SUPERIOR (perfil de proyecto mecatrónico)

> Plantilla del documento de Diseño Superior entregada como modelo (ejemplo: brazo robótico, HP Medical).
> Guardada el 2026-10-06 tal como fue recibida. Las marcas `[cite: N]` provienen de la extracción del original.
> Uso: define **estructura, numeración y recursos** de cada sección. El contenido del ejemplo NO se copia.
> Defectos del ejemplo a no replicar: secciones 4.2 y 4.3 duplicadas; numeración 7.1.3 repetida;
> RNF-11 («embalar focos») pegado de otro proyecto; valores técnicos sin respaldo (p. ej., MTBF).
> Lectura aplicada al proyecto: `context/THESIS_STRUCTURE.md`. Ejemplo completo con esta plantilla:
> `research/referencias_estructurales/04_Referencia_Microsistema_Hidrostatico.md`.

---

# ÍNDICE DE CONTENIDOS

| Sección | Página |
| :--- | :---: |
| **1. Introducción** | **4** |
| **1.1. Metas de la empresa** | **4** |
| **1.2. Objetivos de la empresa alineados al proyecto (Problemática de solución)** | **4** |
| **1.3. Problema y Justificación del Proyecto** | **5** |
| **1.4. Objetivos del proyecto** | **6** |
| **1.4.1. Objetivo General del proyecto** | **6** |
| **1.4.2. Objetivos Específicos (Metodología Modelo V, Demming, RUP, etc)** | **7** |
| **1.5. Alcance del Proyecto** | **7** |
| **1.6. Metodología de Desarrollo del proyecto** | **8** |
| **2. Estudios preliminares** | **8** |
| **3. Estado del arte** | **9** |
| **4. Diseño y Desarrollo Técnico Mecatrónico** | **10** |
| **4.1. Árbol de Objetivos del Producto** | **10** |
| **4.2. Diagrama de caja negra & caja transparente** | **12** |
| **4.3. Requerimientos del producto** | **13** |
| **4.3.1. Requerimientos Funcionales (RF)** | **13** |
| **4.3.2. Requerimientos No Funcionales (RNF)** | **14** |
| **5. Diseño de Alto Nivel** | **16** |
| **5.1. Casa de Calidad** | **16** |
| **5.2. Matriz Morfológica** | **16** |
| **5.3. Diagrama de Bloques** | **17** |
| **5.4. Estudio de Alternativas** | **17** |
| **5.5. Definición de Componentes** | **19** |
| **6. Diseño Detallado** | **19** |
| **6.1. Modelos formales de cinemática** | **19** |
| **6.2. Modelos de diseños CAD** | **21** |
| **6.3. Especificación de Protocolos de Control** | **21** |
| **7. Verificacion y Validacion** | **22** |
| **7.1. Verificación del Diseño** | **22** |
| **7.1.1. Pruebas Unitarias** | **22** |
| **7.1.2. Pruebas Integrales o de equipos (prototipo físico)** | **22** |
| **7.1.3. Pruebas Funcionales (prototipo físico)** | **22** |
| **7.1.3. Pruebas de Calidad y Cumplimiento Normativo** | **22** |
| **7.1.4. Análisis de resultados de la simulación o el prototipo** | **22** |
| **7.1.5. Análisis Comparativo entre Diseño y Resultados Reales** | **23** |
| **7.2. Validación del Sistema** | **23** |
| **8. Implementación y Prototipado** | **23** |
| **8.1. Fabricación del Prototipo** | **23** |
| **8.2. Integración de Componentes Electrónicos y de Control** | **23** |
| **8.3. Evaluación del Funcionamiento** | **23** |
| **9. Conclusiones y Recomendaciones** | **24** |
| **9.1. Conclusiones del Proyecto** | **24** |
| **9.2. Recomendaciones para Futuros Desarrollos** | **24** |
| **10. Bibliografía** | **24** |
| **11. Apéndices/Anexos** | **24** |

---

# ÍNDICE DE TABLAS

| Tabla | Página |
| :--- | :---: |
| **Tabla 1 Factibilidad, Viabilidad, Deseabilidad del Proyecto** | **8** |
| **Tabla 2. Matriz morfológica** | **21** |
| **Tabla 3 Matriz cualitativa para la evaluación de conceptos.** | **22** |
| **Tabla 4.Matriz cuantitativa para la evaluación de conceptos.** | **22** |
**Proyecto: *Brazo Robótico para Rehabilitación de Personas con Discapacidad en HP Medical en cumplimiento de la ISO 13482***

*(QUE? QUIEN? CONQUE? PARA QUE?)*

## 1. Introducción

El presente documento describe el desarrollo de un brazo robótico para rehabilitación y fisioterapia, diseñado para personas con discapacidad, en el contexto de la empresa HP Medical[cite: 2]. Este proyecto responde a la necesidad de mejorar la calidad de los tratamientos fisioterapéuticos mediante la integración de tecnologías avanzadas de asistencia robótica[cite: 2].

El diseño y desarrollo del sistema se fundamenta en principios de seguridad funcional, ergonomía y fiabilidad, alineándose con los requisitos establecidos en la ISO 13482 para robots de asistencia personal[cite: 2]. Se abordan los aspectos de factibilidad técnica, viabilidad económica y deseabilidad social, asegurando que el producto final sea seguro, eficiente y adaptable a las necesidades de los usuarios[cite: 2].

### 1.1. Metas de la empresa

HP Medical tiene como meta principal consolidarse como una empresa líder en el desarrollo de tecnologías para rehabilitación y fisioterapia, ofreciendo soluciones innovadoras que mejoren la calidad de vida de los pacientes[cite: 2]. El presente proyecto se alinea con esta meta al desarrollar un dispositivo robótico que optimiza la recuperación funcional y promueve la autonomía de los usuarios[cite: 2].

### 1.2. Objetivos de la empresa alineados al proyecto (Problemática de solución)

El brazo robótico desarrollado busca solucionar la problemática de accesibilidad a terapias especializadas, optimizando los procesos de rehabilitación mediante tecnología avanzada[cite: 2]. Los principales desafíos identificados incluyen:

* Limitaciones en la rehabilitación manual debido a la disponibilidad de fisioterapeutas y la variabilidad en la calidad del tratamiento[cite: 2].
* Falta de dispositivos accesibles que ofrezcan terapias personalizadas y adaptativas para diferentes niveles de discapacidad[cite: 2].
* Necesidad de monitoreo preciso y evaluación objetiva del progreso del paciente, lo que requiere sensores avanzados e integración con sistemas de análisis de datos[cite: 2].

El proyecto responde a estas problemáticas mediante el diseño de un sistema seguro, ergonómico y automatizado, con capacidad de adaptar los movimientos del brazo robótico a las necesidades específicas de cada paciente[cite: 2].

### 1.3. Problema y Justificación del Proyecto

> Experimental: [Variable independiente] + [Efecto en la variable dependiente] + [Condiciones experimentales] + [Contexto del estudio].

La rehabilitación asistida con robótica representa un avance significativo en el tratamiento de personas con discapacidad motriz, permitiendo terapias personalizadas y controladas con precisión[cite: 2]. Este proyecto responde a la necesidad de HP Medical de incorporar soluciones tecnológicas avanzadas para mejorar la efectividad de los tratamientos fisioterapéuticos[cite: 2].

La justificación del desarrollo del brazo robótico se fundamenta en tres ejes principales:

* **Beneficio clínico:** Facilita la recuperación muscular y mejora la movilidad de los pacientes[cite: 2].
* **Eficiencia operativa:** Reduce la carga de trabajo del personal fisioterapéutico mediante automatización parcial del tratamiento[cite: 2].
* **Cumplimiento normativo:** Garantiza la seguridad y fiabilidad del dispositivo según estándares internacionales[cite: 2].

La descripción del problema está especificado en tres formas de representación:

* Descriptiva textual:
  > Las personas con dificultades de movimiento articular superior derecho, que es causado por varias condiciones, afrontan un conjunto de incompatibilidades con el ecosistema de máquinas y recursos disponibles en clínicas o instituciones dedicadas a la rehabilitación fisiológica[cite: 2].
  > Entre los causales de esta condición están los precios no accesibles para los interesados, así como para las instituciones[cite: 2].
  > Los tiempos de parada para el mantenimiento de los recursos en clínicas de fisioterapia y rehabilitación no son flexibles para los pacientes, porque los procesos de mantenimiento exigen cumplir con protocolos de mantenimiento estrictos de los proveedores[cite: 2].
  En periodos de mantenimiento de los equipos en las clínicas, los repuestos y materiales necesarios no están al alcance local, porque deben ser componentes importados y autorizados por el proveedor[cite: 3].

* **Diagrama causa - efecto:**

### Análisis del Diagrama de Ishikawa (Causa - Efecto)

El diagrama analiza las causas raíz que generan el efecto/problema principal expresado en la cabeza del pescado[cite: 3].

* **Efecto (Problema Central):**
  * Los recursos y modelos de rehabilitación para personas con discapacidad motriz en el brazo derecho, no cumplen con las expectativas de los interesados[cite: 3].

* **Causas Principales (Espinas superiores e inferiores):**
  * **Económicas:**
    * Presupuestos no son adecuados para la adquisición de equipos[cite: 3].
  * **Mantenimiento:**
    * Herramientas de mantenimiento no disponibles en Bolivia[cite: 3].
    * Repuestos autorizados y únicos del proveedor[cite: 3].
  * **Personal e instituciones:**
    * Personal no cualificado para el mantenimiento[cite: 3].
    * Personal no certificado para la operación[cite: 3].
  * **Materiales y repuestos:**
    * Precio de repuestos no accesibles[cite: 3].

**Diagrama de Ishikawa**

* **Tabla de inconformidades a solucionar:**

| Causal | Valor |
| :--- | :--- |
| Fiabilidad, cumplimiento a la fiabilidad | Los recursos de equipos de rehabilitación en clínicas, no son conformes a las necesidades de los interesados[cite: 3] |
| Usabilidad, operabilidad | La cantidad entre fisioterapeutas y pacientes, no mantiene una relación adecuada a las necesidades de los interesados.[cite: 3] |
| Mantenibilidad, cambiabilidad | Los repuestos solo son los proporcionados por el proveedor, no se admiten otros modelos o fabricantes.[cite: 3] |

## 1.4. Objetivos del proyecto

### 1.4.1. Objetivo General del proyecto

> **verbo:** diseñar[cite: 3]
> **que:** sistema articulación hidrostático[cite: 3]
> **paraque:** apoyo de manejo carga en articulaciones mecánicas[cite: 3]
> **conque:** científica: sistemas hidráulicos, técnica, normativa[cite: 3]

Desarrollar un brazo robótico para rehabilitación y fisioterapia, capaz de asistir a personas con discapacidad motriz en la recuperación de movilidad, mediante la integración de tecnologías de control de movimiento, monitoreo sensorial y automatización segura, cumpliendo con los estándares de la ISO 13482[cite: 3].

### 1.4.2. Objetivos Específicos (Metodología Modelo V, Demming, RUP, etc)

* Especificar los requerimientos del sistema mediante el análisis de necesidades médicas, normativas y funcionales, asegurando el cumplimiento de la ISO 13482 y otras regulaciones aplicables a dispositivos de asistencia robótica[cite: 3].
* Diseñar la arquitectura del sistema mediante la creación de modelos estructurales, mecánicos y electrónicos del brazo robótico, asegurando que la distribución de cargas y movimientos sea segura y eficiente para la rehabilitación[cite: 3].
* Desarrollar el sistema de control y software embebido, estableciendo algoritmos para la gestión de movimiento, adaptación a la fuerza del paciente y monitoreo de datos clínicos en tiempo real[cite: 3].
* Integrar los subsistemas eléctricos, electrónicos y mecánicos, asegurando la compatibilidad y funcionamiento óptimo del hardware y software[cite: 3].
* Verificar el sistema completo mediante pruebas de funcionalidad, ergonomía y seguridad[cite: 3].
* Validar el desempeño del brazo robótico en condiciones clínicas y garantizando la eficacia del tratamiento fisioterapéutico[cite: 3].

## 1.5. Alcance del Proyecto

El proyecto abarca el diseño, desarrollo, implementación y validación de un brazo robótico para rehabilitación, considerando los siguientes alcances:

* **Alcance Técnico:** Diseño mecánico y estructural del brazo, implementación de motores eléctricos, desarrollo de firmware y software de control, integración de sensores biomédicos y pruebas de rendimiento[cite: 3].
* **Alcance Funcional:** El sistema ajusta la resistencia y velocidad, registrando datos del paciente y garantizar la seguridad en los movimientos[cite: 3].
* **Alcance Normativo:** Cumplimiento de estándares de seguridad y calidad según ISO 13482 (Robots de Asistencia Personal), ISO 12100 (Seguridad de maquinaria) e IEC 60601 (Equipos electromédicos)[cite: 3].
* **Alcance Temporal:** Desarrollo en un período de 8 meses, incluyendo etapas de diseño, fabricación, integración y pruebas de validación clínica[cite: 4].
* **Alcance de Usuarios:** Diseñado para personas con discapacidad motriz parcial o en proceso de recuperación física, bajo supervisión médica[cite: 4].
* **Alcance de Limitaciones:** No incluye desarrollo de algoritmos de inteligencia artificial avanzada para aprendizaje adaptativo ni integración con bases de datos hospitalarias en la primera fase[cite: 4].

## 1.6. Metodología de Desarrollo del proyecto

El desarrollo del brazo robótico sigue un enfoque basado en metodologías de ingeniería, priorizando la calidad, la validación progresiva y la integración de requisitos funcionales y de seguridad[cite: 4].

* **Modelo en V:** Se emplea para garantizar un desarrollo estructurado, donde cada fase de diseño es validada antes de avanzar a la siguiente etapa[cite: 4].
* **Ciclo de Deming (PDCA):** Aplicado en la fase de optimización y mejoras, permitiendo ajustes continuos en el diseño y funcionalidad del dispositivo[cite: 4].
* **Metodología RUP (Rational Unified Process):** Se implementa para el desarrollo del software de control, asegurando iteraciones progresivas con pruebas constantes[cite: 4].

Las principales etapas del desarrollo incluyen:

* **Definición de requisitos** $\rightarrow$ Recopilación de necesidades clínicas y normativas[cite: 4].
* **Diseño conceptual y simulaciones** $\rightarrow$ Creación de modelos CAD y evaluación de cargas mecánicas[cite: 4].
* **Desarrollo de hardware y software** $\rightarrow$ Implementación del sistema de control y firmware embebido[cite: 4].
* **Integración y pruebas** $\rightarrow$ Verificación del cumplimiento de normas de seguridad, eficiencia y ergonomía[cite: 4].
* **Validación con usuarios finales** $\rightarrow$ Evaluación en entornos clínicos para optimizar la experiencia del usuario[cite: 4].

## 2. Estudios preliminares

* **Factibilidad:** El equipo investigador cumple con características técnicas, recursos, cronograma. **(Cumple / No cumple)**[cite: 4]
* **Viabilidad:** EL cliente tiene capacidad económica, operativa y cronograma para aplicar y operar el entregable. **(Cumple / No cumple)**[cite: 4]
* **Deseabilidad:** El entregable aporta valor social, ambiental, de competencia u otro. **(Cumple / No cumple)**[cite: 4]

## 3. Estado del arte

(Proyectos o productos similares con enfoque académico, comercial, patentes en total 30)[cite: 4]

Criterios de inclusión/exclusión:

* posterior al año 2020[cite: 4]
* costos fabricación <= USD12000[cite: 4]
* tiempo de parada <= 2 días[cite: 4]
* etc[cite: 4]

Desde 2020, la rehabilitación robótica ha experimentado avances significativos, integrando tecnologías emergentes para mejorar la recuperación funcional de las extremidades superiores[cite: 4]. A continuación, se detallan las tendencias y desarrollos más destacados en este ámbito:

* Proyecto de Grado Brazo Robótico para personal de la fábrica NexTel[cite: 4]
  * Problema, objetivo, resultados[cite: 4].
* Brazo Robótico Honda HPF8500[cite: 4]
  * Objetivo, garantías, costos, tiempos de mtto, tiempos de importación[cite: 4].
* **Exoesqueletos Suaves Basados en Inteligencia Artificial.**
  * Los exoesqueletos tradicionales, caracterizados por estructuras rígidas, han evolucionado hacia diseños más flexibles y adaptativos[cite: 4]. Los exoesqueletos suaves, confeccionados con materiales flexibles, ofrecen mayor comodidad y adaptabilidad al usuario[cite: 4]. La incorporación de algoritmos de inteligencia artificial permite que estos dispositivos se ajusten dinámicamente a las necesidades específicas de cada paciente, optimizando el proceso de rehabilitación[cite: 4]. Esta combinación de flexibilidad y adaptabilidad mejora la experiencia del usuario y potencia la eficacia terapéutica[cite: 4].
* **Integración de Realidad Virtual e Interfaces Robóticas.**
  * La fusión de la realidad virtual (RV) con sistemas robóticos ha abierto nuevas posibilidades en la rehabilitación de las extremidades superiores[cite: 4]. Esta integración crea entornos inmersivos que motivan a los pacientes y facilitan la realización de ejercicios terapéuticos[cite: 4]. Estudios recientes han demostrado que la combinación de RV con dispositivos robóticos y sensores[cite: 4]
  portátiles mejora la adherencia a la terapia y proporciona datos precisos para monitorear el progreso del paciente[cite: 5].

* **Avances en Prótesis Controladas por Interfaces Cerebro-Computadora.**
  * La empresa Neuralink ha obtenido autorización para probar implantes cerebrales que permiten a personas parapléjicas controlar brazos robóticos mediante señales neuronales[cite: 5]. Este enfoque promete restaurar la movilidad en individuos con lesiones medulares o enfermedades neurodegenerativas, ofreciendo una solución avanzada para la interacción directa entre el cerebro y dispositivos protésicos[cite: 5].

* **Mecanismos de Actuación Basados en Tecnología Magnética.**
  * Investigaciones recientes han introducido mecanismos de actuación basados en tecnología magnética para plataformas robóticas de rehabilitación[cite: 5]. Estos sistemas proporcionan una retroalimentación háptica más suave y precisa, mejorando la interacción entre el usuario y el dispositivo[cite: 5]. La aplicación de algoritmos avanzados, como el Filtro de Kalman Extendido, permite un control más preciso y una experiencia de rehabilitación más efectiva[cite: 5].

* **Robots Sociales en Entornos de Atención**
  * La implementación de robots sociales, como Temi y Copito, en residencias de ancianos ha demostrado ser beneficiosa para la atención de personas mayores (fuente)[cite: 5]. Estos robots facilitan actividades físicas, cognitivas y de entretenimiento, además de servir como herramientas de trabajo para los profesionales de la salud (fuente)[cite: 5]. Su integración ha sido bien recibida, aunque se han identificado áreas de mejora para aumentar su atractivo y funcionalidad[cite: 5].

* **Revisión Sistemática de la Eficacia de la Robótica en Terapia Ocupacional.**
  * Una revisión sistemática publicada en 2023 evaluó la efectividad de la terapia robótica en comparación con la terapia ocupacional convencional para la recuperación funcional del miembro superior en pacientes que han sufrido un accidente cerebrovascular[cite: 5]. Los resultados sugieren que la combinación de ambas terapias optimiza la funcionalidad e independencia de los pacientes (apéndice), aunque se requiere más investigación para determinar las competencias específicas en las que la robótica ofrece mayores beneficios[cite: 5].

## 4. Diseño y Desarrollo Técnico Mecatrónico

### 4.1. Árbol de Objetivos del Producto

Descripción extensa y desglosada del árbol de objetivos[cite: 5].

---

### Análisis del Diagrama Hierárquico de Relación entre Objetivos (Figure 6.1)

#### **Estructura y Componentes del Diagrama:**

* **Nivel Principal / Objetivo Raíz:**
  * **Machine must be safe** (*La máquina debe ser segura*)[cite: 5].
* **Sub-objetivos Directos (Segundo Nivel):**
  * **Low risk of injury to operator** (*Bajo riesgo de lesiones para el operador*)[cite: 5].
  * **Low risk of operator mistakes** (*Bajo riesgo de errores del operador*)[cite: 5].
  * **Low risk of damage to workpiece or tool** (*Bajo riesgo de daños en la pieza de trabajo o herramienta*)[cite: 5].
* **Sub-objetivo Derivado (Tercer Nivel - Rama Derecha):**
  * **Automatic cut-out on overload** (*Corte automático por sobrecarga*), el cual se desprende de *Low risk of damage to workpiece or tool*[cite: 5].

#### **Relaciones Causal/Jerárquica (Flechas Laterales):**
* **Dirección Descendente ('How' / Cómo):** Expresa el medio o la forma de lograr el objetivo superior (ej. Para lograr que *Machine must be safe*, se reduce el riesgo al operador, errores y daños; y para reducir daños, se implementa *Automatic cut-out on overload*)[cite: 5].
* **Dirección Ascendente ('Why' / Por qué):** Expresa la justificación o propósito del sub-objetivo (ej. Se busca *Automatic cut-out on overload* para garantizar *Low risk of damage...*, lo que a su vez responde a *Machine must be safe*)[cite: 5].

**Figure 6.1 Hierarchical diagram of relationships between objectives.**  
Fuente: (Cross, 2024)[cite: 5]

---

### Análisis del Árbol de Objetivos para un Banco de Pruebas (Figura 6.3)

#### **Estructura Jerárquica y Desglose por Ramas:**

* **Objetivo General / Raíz Central:**
  * **Reliable and simple testing device** (*Dispositivo de prueba confiable y simple*)[cite: 5].

* **Desglose en Categorías Principales y Sub-objetivos:**

  1. **Reliable operation (*Operación confiable*):**[cite: 5]
     * **Good reproducibility of torque-time curve** (*Buena reproducibilidad de la curva torque-tiempo*)[cite: 5]:
       * *Low wear of moving parts* (*Bajo desgaste de partes móviles*)[cite: 5].
       * *Low susceptibility to vibration* (*Baja susceptibilidad a vibraciones*)[cite: 5].
     * **Tolerance of overloading** (*Tolerancia a sobrecargas*)[cite: 5]:
       * *Few disturbing factors* (*Pocos factores de perturbación*)[cite: 5].

  2. **High safety (*Alta seguridad*):**[cite: 5]
     * **High mechanical safety** (*Alta seguridad mecánica*)[cite: 5].
     * **Few possible operator errors** (*Pocos errores de operador posibles*)[cite: 5].

  3. **Simple production (*Producción simple*):**[cite: 5]
     * **Simple component production** (*Producción simple de componentes*)[cite: 5]:
       * *Small number of components* (*Pequeño número de componentes*)[cite: 5].
       * *Low complexity of components* (*Baja complejidad de componentes*)[cite: 5].
     * **Simple assembly** (*Ensamble simple*)[cite: 5]:
       * *Many standard and bought-ought parts* (*Muchas partes estándar y comerciales*)[cite: 5].

  4. **Good operating characteristics (*Buenas características operativas*):**[cite: 5]
     * **Easy maintenance** (*Fácil mantenimiento*)[cite: 5]:
       * *Quick exchange of test connections* (*Intercambio rápido de conexiones de prueba*)[cite: 5].
     * **Easy handling** (*Fácil manejo*)[cite: 5]:
       * *Good access of measuring systems* (*Buen acceso a sistemas de medición*)[cite: 5].

**Figura 6.3. Árbol de objetivos para un banco de pruebas de carga por impulso**  
Fuente: (Cross, 2024)[cite: 5]
### 4.2. Diagrama de caja negra & caja transparente

Descripción extensa y desglosada del diagrama de caja negra[cite: 6]

---

### Análisis del Modelo de Sistema de Caja Negra (Figure 7.1)

#### **Estructura y Componentes del Diagrama:**
* **Entradas (Inputs):** Representadas por tres flechas horizontales hacia la derecha a la izquierda del bloque, simbolizando las variables de entrada al sistema (energía, materia y señales)[cite: 6].
* **Proceso / Función (Function - 'BLACK BOX'):** Un bloque rectangular central rotulado como `'BLACK BOX'`. Representa la función global del sistema donde se desconocen o abstraen los mecanismos internos[cite: 6].
* **Salidas (Outputs):** Representadas por tres flechas horizontales hacia la derecha a la derecha del bloque, simbolizando las variables de salida resultantes del proceso[cite: 6].

**Figure 7.1 The 'black box' systems model.**  
Fuente: (Cross, 2024)[cite: 6]

---

Descripción extensa y desglosada del diagrama de caja transparente[cite: 6]

---

### Análisis del Modelo de Caja Transparente (Figure 7.2)

#### **Estructura y Componentes del Diagrama:**
* **Entradas (Inputs):** Dos líneas de entrada principales que ingresan al límite del sistema desde la izquierda[cite: 6].
* **Límite del Sistema ('TRANSPARENT BOX'):** Un recuadro grande que delimita el sistema y deja visibles las subfunciones internas y sus interconexiones[cite: 6].
* **Subfunciones (Sub-function):**
  * Cuatro bloques internos distribuidos e interconectados:
    1. **Sub-función inferior izquierda:** Recibe una entrada externa directa[cite: 6].
    2. **Sub-función superior izquierda:** Recibe la segunda entrada externa y una conexión directa desde la sub-función inferior izquierda[cite: 6].
    3. **Sub-función inferior central:** Conectada desde la sub-función inferior izquierda[cite: 6].
    4. **Sub-función superior derecha:** Conectada desde la sub-función superior izquierda y la sub-función inferior central[cite: 6].
* **Salida (Output):** Una línea de salida principal que emerge de la sub-función superior derecha cruzando el límite hacia el exterior[cite: 6].

**Figure 7.2 A 'transparent box' model.**  
Fuente: (Cross, 2024)[cite: 6]

---

### 4.3. Requerimientos del producto

#### 4.3.1. Requerimientos Funcionales (RF)

| ID | Requerimiento Funcional | O/D | Descripción | Valor Técnico Esperado |
| :--- | :--- | :---: | :--- | :--- |
| **RF-01** | Grados de Libertad (DOF) | O | El brazo robótico debe tener múltiples grados de libertad para realizar movimientos precisos. | 6 DOF o más |
| **RF-02** | Capacidad de Carga | O | El brazo debe ser capaz de levantar y manipular objetos de un peso determinado. | 3-5 kg (según aplicación) |
| **RF-03** | Precisión Posicional | O | Debe alcanzar posiciones con alta precisión en sus movimientos. | $\pm 0.1 \text{ mm}$ |
| **RF-04** | Velocidad de Movimiento | O | Cada articulación debe moverse con rapidez controlada. | 0.5 - 2 rad/s |
| **RF-05** | Alcance Máximo | O | El brazo debe poder extenderse hasta una determinada longitud desde su base. | 700 mm - 1000 mm |
| **RF-06** | Tipo de Actuadores | O | Debe utilizar actuadores adecuados para lograr movimientos fluidos y eficientes. | Motores servo o motores paso a paso con reductores |
| **RF-07** | Material de Construcción | O | Los materiales deben proporcionar rigidez, ligereza y resistencia. | Aluminio aeronáutico o polímeros reforzados |
| **RF-08** | Interfaz de Control | O | Debe ser compatible con sistemas de programación y control de fácil acceso. | ROS, Python, LabVIEW o MATLAB |
| **RF-09** | Sistema de Sensado | O | Debe incorporar sensores para mejorar su desempeño. | Encoders en motores, sensores de fuerza y cámara de visión |
| **RF-10** | Capacidad de Interacción Humano-Robot (HRI) | O | El brazo debe poder operar de forma segura en entornos compartidos con humanos. | Sensores de proximidad y detección de colisiones |
| **RF-11** | Fuente de Alimentación | O | El sistema debe operar con una fuente de energía adecuada para su funcionamiento. | 24V DC - 48V DC |
| **RF-12** | Modos de Control | O | Debe admitir diferentes tipos de control según la aplicación. | Control de torque, control de posición, control de velocidad |
| **RF-13** | Tiempo de Respuesta | O | El sistema debe reaccionar en un tiempo determinado a las órdenes del usuario o sensores. | <100 ms |
| **RF-14** | Compatibilidad con Herramientas Finales (EOAT) | O | Debe permitir el uso de diferentes tipos de efectores finales. | Pinza mecánica, ventosa neumática, herramienta personalizada |
| **RF-15** | Protección y Seguridad | O | Debe contar con mecanismos de seguridad para evitar fallos y accidentes. | Paro de emergencia, limitación de torque, carcasas protectoras |
### 4.2. Diagrama de caja negra & caja transparente

Descripción extensa y desglosada del diagrama de caja negra[cite: 6]

---

### Análisis del Modelo de Sistema de Caja Negra (Figure 7.1)

#### **Estructura y Componentes del Diagrama:**
* **Entradas (Inputs):** Representadas por tres flechas horizontales hacia la derecha a la izquierda del bloque, simbolizando las variables de entrada al sistema (energía, materia y señales)[cite: 6].
* **Proceso / Función (Function - 'BLACK BOX'):** Un bloque rectangular central rotulado como `'BLACK BOX'`. Representa la función global del sistema donde se desconocen o abstraen los mecanismos internos[cite: 6].
* **Salidas (Outputs):** Representadas por tres flechas horizontales hacia la derecha a la derecha del bloque, simbolizando las variables de salida resultantes del proceso[cite: 6].

**Figure 7.1 The 'black box' systems model.**  
Fuente: (Cross, 2024)[cite: 6]

---

Descripción extensa y desglosada del diagrama de caja transparente[cite: 6]

---

### Análisis del Modelo de Caja Transparente (Figure 7.2)

#### **Estructura y Componentes del Diagrama:**
* **Entradas (Inputs):** Dos líneas de entrada principales que ingresan al límite del sistema desde la izquierda[cite: 6].
* **Límite del Sistema ('TRANSPARENT BOX'):** Un recuadro grande que delimita el sistema y deja visibles las subfunciones internas y sus interconexiones[cite: 6].
* **Subfunciones (Sub-function):**
  * Cuatro bloques internos distribuidos e interconectados:
    1. **Sub-función inferior izquierda:** Recibe una entrada externa directa[cite: 6].
    2. **Sub-función superior izquierda:** Recibe la segunda entrada externa y una conexión directa desde la sub-función inferior izquierda[cite: 6].
    3. **Sub-función inferior central:** Conectada desde la sub-función inferior izquierda[cite: 6].
    4. **Sub-función superior derecha:** Conectada desde la sub-función superior izquierda y la sub-función inferior central[cite: 6].
* **Salida (Output):** Una línea de salida principal que emerge de la sub-función superior derecha cruzando el límite hacia el exterior[cite: 6].

**Figure 7.2 A 'transparent box' model.**  
Fuente: (Cross, 2024)[cite: 6]

---

### 4.3. Requerimientos del producto

#### 4.3.1. Requerimientos Funcionales (RF)

| ID | Requerimiento Funcional | O/D | Descripción | Valor Técnico Esperado |
| :--- | :--- | :---: | :--- | :--- |
| **RF-01** | Grados de Libertad (DOF) | O | El brazo robótico debe tener múltiples grados de libertad para realizar movimientos precisos. | 6 DOF o más |
| **RF-02** | Capacidad de Carga | O | El brazo debe ser capaz de levantar y manipular objetos de un peso determinado. | 3-5 kg (según aplicación) |
| **RF-03** | Precisión Posicional | O | Debe alcanzar posiciones con alta precisión en sus movimientos. | $\pm 0.1 \text{ mm}$ |
| **RF-04** | Velocidad de Movimiento | O | Cada articulación debe moverse con rapidez controlada. | 0.5 - 2 rad/s |
| **RF-05** | Alcance Máximo | O | El brazo debe poder extenderse hasta una determinada longitud desde su base. | 700 mm - 1000 mm |
| **RF-06** | Tipo de Actuadores | O | Debe utilizar actuadores adecuados para lograr movimientos fluidos y eficientes. | Motores servo o motores paso a paso con reductores |
| **RF-07** | Material de Construcción | O | Los materiales deben proporcionar rigidez, ligereza y resistencia. | Aluminio aeronáutico o polímeros reforzados |
| **RF-08** | Interfaz de Control | O | Debe ser compatible con sistemas de programación y control de fácil acceso. | ROS, Python, LabVIEW o MATLAB |
| **RF-09** | Sistema de Sensado | O | Debe incorporar sensores para mejorar su desempeño. | Encoders en motores, sensores de fuerza y cámara de visión |
| **RF-10** | Capacidad de Interacción Humano-Robot (HRI) | O | El brazo debe poder operar de forma segura en entornos compartidos con humanos. | Sensores de proximidad y detección de colisiones |
| **RF-11** | Fuente de Alimentación | O | El sistema debe operar con una fuente de energía adecuada para su funcionamiento. | 24V DC - 48V DC |
| **RF-12** | Modos de Control | O | Debe admitir diferentes tipos de control según la aplicación. | Control de torque, control de posición, control de velocidad |
| **RF-13** | Tiempo de Respuesta | O | El sistema debe reaccionar en un tiempo determinado a las órdenes del usuario o sensores. | <100 ms |
| **RF-14** | Compatibilidad con Herramientas Finales (EOAT) | O | Debe permitir el uso de diferentes tipos de efectores finales. | Pinza mecánica, ventosa neumática, herramienta personalizada |
| **RF-15** | Protección y Seguridad | O | Debe contar con mecanismos de seguridad para evitar fallos y accidentes. | Paro de emergencia, limitación de torque, carcasas protectoras |
#### 4.3.2. Requerimientos No Funcionales (RNF)

| ID | Categoría | O/D | Requerimiento No Funcional | Descripción | Valor Técnico / Normas Aplicables |
| :--- | :--- | :---: | :--- | :--- | :--- |
| **RNF-01** | Usabilidad | O | Facilidad de operación | La interfaz debe ser intuitiva y fácil de aprender para operadores sin formación técnica. | Interfaz táctil con GUI simple, ISO 9241 (Ergonomía) |
| **RNF-02** | Usabilidad | O | Accesibilidad del sistema | La interfaz debe ser adaptable a distintos niveles de experiencia del usuario. | Modos de usuario: básico y avanzado |
| **RNF-03** | Mantenibilidad | O | Bajo mantenimiento | Las tareas de mantenimiento deben ser mínimas y fáciles de ejecutar. | Mantenimiento preventivo mensual, ISO 9283 (Performance de robots industriales) |
| **RNF-04** | Mantenibilidad | O | Disponibilidad de repuestos | Todos los repuestos deben ser de fácil adquisición en el mercado local. | Tiempo máximo de reposición: 7 días |
| **RNF-05** | Confiabilidad | O | Tiempo medio entre fallos (MTBF) | El brazo debe operar de forma continua sin fallos frecuentes. | MTBF $\ge 10,000$ horas |
| **RNF-06** | Seguridad Operativa | O | Protección ante colisiones | Debe incluir sensores de proximidad para evitar impactos con objetos o personas. | Sensores de detección, ISO 10218 (Seguridad de robots) |
| **RNF-07** | Seguridad Operativa | O | Paro de emergencia | Debe contar con un botón de parada de emergencia de fácil acceso. | Botón rojo con desconexión total, ISO 12100 (Seguridad de maquinaria) |
| **RNF-08** | Seguridad Operativa | O | Reducción de riesgos mecánicos | Los actuadores y mecanismos móviles deben minimizar riesgos para el personal. | Carcasas de protección y bordes redondeados |
| **RNF-09** | Ergonomía | O | Altura y diseño optimizado | La instalación y operación deben ajustarse a estándares ergonómicos industriales. | Altura ajustable, ISO 11226 (Ergonomía postural) |
| **RNF-10** | Ergonomía | O | Interacción intuitiva | Los controles deben ser accesibles y entendibles sin necesidad de capacitación extensa. | Uso de íconos gráficos y colores |
| **RNF-11** | Automatización | O | Operación autónoma | El brazo debe embalar focos de manera completamente automática. | Sin intervención humana directa |
| **RNF-12** | Automatización | O | Integración con sistemas industriales | Compatible con líneas de producción y otros sistemas automatizados. | Comunicación Modbus, OPC-UA |
| **RNF-13** | Eficiencia Energética | O | Consumo de energía optimizado | La operación debe minimizar el gasto energético sin afectar el rendimiento. | $\le 500\text{W}$, ISO 50001 (Gestión Energética) |
| **RNF-14** | Costo | O | Bajo costo de implementación | Debe tener un costo accesible sin comprometer calidad y seguridad. | Presupuesto máximo: \$10,000 USD |
| **RNF-15** | Costo | O | Bajo costo de operación y mantenimiento | Debe minimizar costos de consumo energético y repuestos. | Mantenimiento $\le 5\%$ del costo anual |
| **RNF-16** | Normas y Certificación | O | Cumplimiento de estándares internacionales | Debe ser certificable bajo normativas de calidad y seguridad. | ISO 9001, CE, UL |
| **RNF-17** | Escalabilidad | O | Expansión del sistema | Debe permitir la integración de nuevas herramientas finales y accesorios. | Módulo de expansión con conexión rápida |
| **RNF-18** | Ruido Operacional | O | Nivel de ruido bajo | Debe operar en entornos de trabajo sin generar contaminación acústica. | $\le 60\text{ dB}$, ISO 11688 (Reducción de ruido en maquinaria) |
| **RNF-19** | Disponibilidad | O | Tiempo de parada | Tiempo de parada por mantenimiento correctivo, preventivo, operativo | |
## 5. Diseño de Alto Nivel

### 5.1. Casa de Calidad

Descripción extensa y desglosada del diagrama de casa de calidad[cite: 8].

---

### Análisis de la Casa de Calidad (Figure 9.6)

#### **1. Atributos del Cliente (Customer Attributes / Requerimientos - Qué):**
* **Warms air rapidly** (*Calienta el aire rápidamente*) – Importancia: 16[cite: 8]
* **Maintains comfortable air temp** (*Mantiene temperatura de aire confortable*) – Importancia: 12[cite: 8]
* **Provides variable air movement** (*Proporciona movimiento de aire variable*) – Importancia: 10[cite: 8]
* **Safe for home use** (*Seguro para uso doméstico*) – Importancia: 20[cite: 8]
* **Does not burn skin to touch** (*No quema la piel al tacto*) – Importancia: 16[cite: 8]
* **Easily moved** (*Fácilmente movible*) – Importancia: 8[cite: 8]
* **Easy to use controls** (*Controles fáciles de usar*) – Importancia: 4[cite: 8]
* **Clearly visible control settings** (*Ajustes de control claramente visibles*) – Importancia: 4[cite: 8]
* **Not too big** (*No demasiado grande*) – Importancia: 6[cite: 8]
* **Attractive appearance** (*Apariencia atractiva*) – Importancia: 4[cite: 8]

#### **2. Características de Ingeniería (Engineering Characteristics - Cómo):**
* Wire resistance (*Resistencia del cable*)[cite: 8]
* Current (*Corriente*)[cite: 8]
* Voltage (*Voltaje*)[cite: 8]
* Heat output (*Salida de calor*)[cite: 8]
* No. heater settings (*N° de ajustes de calentador*)[cite: 8]
* Exit air velocity (*Velocidad del aire de salida*)[cite: 8]
* Volume flow air rate (*Flujo volumétrico de aire*)[cite: 8]
* Fan speed (*Velocidad del ventilador*)[cite: 8]
* No. speed settings (*N° de ajustes de velocidad*)[cite: 8]
* Casing insulation (*Aislamiento de la carcasa*)[cite: 8]
* Casing film & colour (*Película y color de la carcasa*)[cite: 8]
* Outlet grill spacings (*Espaciado de la rejilla de salida*)[cite: 8]
* Switch design (*Diseño del interruptor*)[cite: 8]
* Overall mass (*Masa total*)[cite: 8]
* Overall dimensions (*Dimensiones totales*)[cite: 8]
* Stability (*Estabilidad*)[cite: 8]

#### **3. Matriz de Relaciones (Matriz Central):**
* **Leyenda de símbolos:**
  * $\bullet$ **Fuerte** (*Strong*)[cite: 8]
  * $\circ$ **Media** (*Medium*)[cite: 8]
  * $\triangle$ **Débil** (*Weak*)[cite: 8]

#### **4. Evaluación de la Competencia (Comparisons 1-5):**
* Muestra la comparación del producto frente al **Competidor A** ($\square$) y **Competidor B** ($\square$) en cada atributo del cliente en una escala del 1 al 5[cite: 8].

#### **5. Importancia Técnica / Metas (Fila Inferior):**
* **Importancia EC (EC Importance):** Valores ponderados para cada característica técnica ($5, 9, 7, 7, 3, 6, 10, 10, 7, 10, 7, 3, 2, 3, 5, 5$)[cite: 8].
* **Unidades (Units):** $\Omega, \text{A}, \text{V}, \text{l}^2\text{R}, \text{m/s}, \text{m}^3/\text{s}, \text{1/s}, \text{n}, \%, \text{mm}, \text{Kg}, \text{mm}$[cite: 8].

**Figure 9.6 House of quality for a domestic fan heater.**  
Fuente: (Cross, 2024, página 133)[cite: 8]

---

### 5.2. Matriz Morfológica

Descripción extensa y desglosada de la matriz morfológica + la descripción de los caminos y justificación del camino elegido[cite: 8].

#### **Tabla 2. Matriz morfológica**

| N° | FUNCIÓN | ALTERNATIVA 1 | ALTERNATIVA 2 | ALTERNATIVA 3 |
| :---: | :--- | :--- | :--- | :--- |
| **1** | **ACCIONAMIENTO** | MANUAL *(Imagen de palanca manual)* | BOTONERA COLGANTE *(Imagen de botonera)* | BOTONERA INALÁMBRICA *(Imagen de control inalámbrico)* |
| **2** | **SUJETAR** | GANCHO *(Imagen de gancho de carga)* | ESLINGA *(Imagen de eslinga de carga)* | GRILLETE *(Imagen de grillete metálico)* |
| **3** | **LEVANTAR** | POLEA Y CADENA *(Imagen de polipasto manual)* | MOTOR ELÉCTRICO *(Imagen de motor eléctrico azúl)* | MOTOR ELÉCTRICO *(Imagen de motor eléctrico verde)* |
| **4** | **TRANSPORTAR** | RUEDA MONOBLOQUE CON PESTAÑA *(Imagen de rueda metálica)* | RUEDA MONOBLOQUE CON RANURA - C *(Imagen de rueda ranurada)* | RUEDA MONOBLOQUE CON CANAL - V *(Imagen de rueda en V)* |
| **5** | **DESCARGAR** | POLEA Y CADENA *(Imagen de polipasto manual)* | MOTOR ELÉCTRICO *(Imagen de motor eléctrico azúl)* | MOTOR ELÉCTRICO *(Imagen de motor eléctrico verde)* |
| **6** | **SOLTAR** | GANCHO *(Imagen de gancho de carga)* | ESLINGA *(Imagen de eslinga de carga)* | GRILLETE *(Imagen de grillete metálico)* |

Fuente: Elaboración propia[cite: 8]  
Fuente: (Cross, 2024)[cite: 8]

#### **Análisis de Opciones y Caminos trazados en la Matriz:**
* **Camino Rojo (Solución seleccionada A):** 
  * *Accionamiento:* Manual $\rightarrow$ *Sujetar:* Grillete $\rightarrow$ *Levantar:* Motor eléctrico (Azul) $\rightarrow$ *Transportar:* Rueda monobloque con canal - V $\rightarrow$ *Descargar:* Polea y cadena $\rightarrow$ *Soltar:* Eslinga[cite: 8].
* **Camino Verde (Solución alternativa B):**
  * *Accionamiento:* Botonera colgante $\rightarrow$ *Sujetar:* Eslinga $\rightarrow$ *Levantar:* Polea y cadena $\rightarrow$ *Transportar:* Rueda monobloque con pestaña $\rightarrow$ *Descargar:* Polea y cadena $\rightarrow$ *Soltar:* Gancho[cite: 8].

---

### 5.3. Diagrama de Bloques

Descripción extensa y desglosada del diagrama de bloques[cite: 8].

* Representación de la interacción entre subsistemas[cite: 8]

---

### Análisis del Diagrama de Bloques (Figura 1)

#### **Componentes y Flujo del Sistema:**
1. **Punto de Comparación / Sumador:** Recibe la señal de entrada y la señal de realimentación proveniente del bloque de **Sensores**[cite: 8].
2. **Controlador:** Recibe la señal de error corregida y procesa la ley de control[cite: 8].
3. **Sistema de potencia:** Transmite la potencia requerida accionada por el controlador[cite: 8].
4. **Salida (Velocidad y dirección):** Variable de salida deseada del sistema mecánico/robótico[cite: 8].
5. **Sensores (Lazo de Realimentación):** Mide la velocidad y dirección de salida y la reenvía al sumador inicial para cerrar el lazo de control[cite: 8].

**Figura 1. Diagrama de bloques**  
Fuente: (Cross, 2024)[cite: 8]

---

### 5.4. Estudio de Alternativas

Descripción extensa y desglosada del estudio de alternativas[cite: 8].
#### **Tabla 3 Matriz cualitativa para la evaluación de conceptos.**

| Criterios de Selección | Conceptos | | | | | |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| | **01** | **02** | **03** | **04** | **05** | **06** |
| Carga de trabajo | + | + | - | + | + | - |
| Alcance máximo | + | + | + | + | + | + |
| Masa total | 0 | 0 | - | 0 | + | - |
| Tiempo requerido para manufactura | 0 | - | + | 0 | - | 0 |
| Tiempo requerido para mantenimiento | 0 | - | + | 0 | - | 0 |
| Costo de partes | 0 | 0 | 0 | 0 | 0 | 0 |
| Intercambiabilidad de efector final | + | + | + | + | + | + |
| Buena apariencia | + | 0 | 0 | + | 0 | 0 |
| Capacidad de traslado | 0 | 0 | 0 | 0 | 0 | 0 |
| Rigidez con respecto a la posición ideal | 0 | 0 | 0 | 0 | 0 | 0 |
| Factor de seguridad en las partes | + | + | + | + | + | + |
| Volumen de trabajo | 0 | 0 | + | 0 | 0 | + |
| **Evaluación neta** | **5** | **2** | **4** | **6** | **3** | **2** |
| **¿Continuar?** | **SÍ** | **NO** | **NO** | **SÍ** | **NO** | **NO** |

Fuente: Elaboración propia[cite: 9]  
Fuente: (Cross, 2024)[cite: 9]

---

#### **Tabla 4.Matriz cuantitativa para la evaluación de conceptos.**

| Criterios de Selección | Peso (%) | Concepto 01 | | Concepto 04 | |
| :--- | :---: | :---: | :---: | :---: | :---: |
| | | **Calificación** | **Ponderación** | **Calificación** | **Ponderación** |
| Carga de trabajo | 10,4 | 5 | 0,52 | 5 | 0,52 |
| Alcance máximo | 10,4 | 5 | 0,52 | 5 | 0,52 |
| Masa total | 8,3 | 3 | 0,24 | 4 | 0,33 |
| Tiempo requerido para manufactura | 6,2 | 3 | 0,18 | 3 | 0,18 |
| Tiempo requerido para mantenimiento | 6,2 | 3 | 0,18 | 3 | 0,18 |
| Costo de partes | 6,2 | 3 | 0,18 | 3 | 0,18 |
| Intercambiabilidad de efector final | 8,3 | 4 | 0,33 | 4 | 0,33 |
| Buena apariencia | 4,1 | 2 | 0,08 | 3 | 0,12 |
| Capacidad de traslado | 8,3 | 3 | 0,24 | 3 | 0,24 |
| Rigidez con respecto a la posición ideal | 10,4 | 4 | 0,41 | 4 | 0,41 |
| Factor de seguridad en las partes | 10,4 | 5 | 0,52 | 5 | 0,52 |
| Volumen de trabajo | 10,4 | 4 | 0,41 | 4 | 0,41 |
| **Total** | | | **3,81** | | **3,94** |
| **¿Continuar?** | | | **NO** | | **SI** |

Fuente: Elaboración propia[cite: 9]  
Fuente: (Cross, 2024)[cite: 9]

---

### 5.5. Definición de Componentes

* Selección de materiales, sensores, actuadores y software[cite: 9]

## 6. Diseño Detallado

### 6.1. Modelos formales de cinemática

* **Matriz de Traslación Homogénea (1):**

$$Tras = \begin{pmatrix} 1 & 0 & 0 & a \\ 0 & 1 & 0 & b \\ 0 & 0 & 1 & c \\ 0 & 0 & 0 & 1 \end{pmatrix}$$

* **Matriz de Rotación en el Eje X (2):**

$$Rot_x = \begin{pmatrix} 1 & 0 & 0 & 0 \\ 0 & \cos(\alpha) & -\text{sen}(\alpha) & 0 \\ 0 & \text{sen}(\alpha) & \cos(\alpha) & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix}$$

* **Matriz de Rotación en el Eje Y (3):**

$$Rot_y = \begin{pmatrix} \cos(\beta) & 0 & \text{sen}(\beta) & 0 \\ 0 & 1 & 0 & 0 \\ -\text{sen}(\beta) & 0 & \cos(\beta) & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix}$$

* **Matriz de Rotación en el Eje Z (4):**

$$Rot_z = \begin{pmatrix} \cos(\gamma) & -\text{sen}(\gamma) & 0 & 0 \\ \text{sen}(\gamma) & \cos(\gamma) & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{pmatrix}$$

---

### Análisis del Diagrama de Arquitectura de Control y Hardware

#### **Estructura y Componentes:**
1. **Interfaz Computacional:**
   * **Interfaz gráfica:** Módulo superior de interacción con el usuario[cite: 9].
   * **Control cinemático:** Módulo inferior encargado de procesar los algoritmos cinemáticos[cite: 9].
2. **Módulo de Comunicación / Interfaz Intermedia:**
   * **Conversor USB a UART-TTL:** Transmite las señales entre la interfaz computacional y la tarjeta de control[cite: 9].
3. **Tarjeta de Control:**
   * **Sistema de potencia:** Recibe comandos y gestiona el suministro eléctrico hacia los actuadores[cite: 9].
   * **Control de potencia:** Controla los niveles de potencia aplicados al brazo robótico[cite: 9].
4. **Brazo Robótico (Pegasus II Amatrol) & Sensores:**
   * **Pegasus II Amatrol:** Brazo robótico físico que recibe la alimentación/control desde el sistema de potencia[cite: 9].
   * **Encoders:** Sensores montados en el brazo que capturan la posición articular real y envían la información de realimentación a la tarjeta de control[cite: 9].

#### **Tabla de parámetros DH**

| i | $\theta_i$ | $d_i$ | $a_i$ | $\alpha_i$ |
| :---: | :---: | :---: | :---: | :---: |
| **1** | $\theta1$ | $L1$ | $0$ | $90^\circ$ |
| **2** | $\theta2$ | $0$ | $L2$ | $0$ |
| **3** | $\theta3$ | $0$ | $L3$ | $0$ |
| **4** | $\theta4$ | $0$ | $L4$ | $0$ |

---

### Análisis de los Diagramas Cinemáticos del Manipulador (Izquierda)

#### **1. Asignación de Sistemas de Coordenadas Denavit-Hartenberg (DH) en Manipulador Articulado:**
* **Estructura:** Muestra el robot manipulador físico con los ejes de coordenadas Cartesianas $(X_i, Y_i, Z_i)$ fijados en cada una de sus articulaciones (desde $i=0$ hasta $i=4$)[cite: 10].
* **Longitudes de eslabón:**
  * $L_1$: Distancia vertical de la base a la primera articulación rotacional[cite: 10].
  * $L_2$: Longitud del brazo/eslabón principal[cite: 10].
  * $L_3$: Longitud del antebrazo/segundo eslabón[cite: 10].
  * $L_4$: Longitud de la muñeca/efector final[cite: 10].
* **Sentidos de rotación:** Flechas curvas que indican el sentido de rotación articular para $\theta_1, \theta_2, \theta_3, \theta_4$[cite: 10].

#### **2. Diagrama Esquemático Vectorial/Geométrico:**
* Representación en un sistema cartesiano $X, Y, Z$ de las proyecciones vectoriales de los eslabones $L1, L2, L3$ y los ángulos articulación $\theta1 - \frac{\pi}{2}, \theta2, \theta3, \theta4$[cite: 10].
* Puntos de coordenadas en el espacio: $(x1, y1, z1)$ y $(x, y, z)$[cite: 10].

* **Deducción geométrica del ángulo $\theta1$ (11):**

$$\tan\left(\theta1 - \frac{\pi}{2}\right) = \frac{-y}{x}, \text{ entonces}$$

$$\theta1 = -\tan^{-1}\left(\frac{x}{y}\right)$$

---

## 6.2. Modelos de diseños CAD

* Diseño en software como SolidWorks, AutoCAD, Fusion 360[cite: 10]

---

### Análisis del Esquema de Estructura Básica del Manipulador (Figura 1)

#### **Componentes e Indicadores:**
* **Base (fija):** Soporte plano que fija el robot a la superficie[cite: 10].
* **Articulaciones (joint) y Coordenadas Articulares:**
  * $q_1$: Rotación sobre el eje vertical de la base (Cintura)[cite: 10].
  * $q_2$: Rotación del primer eslabón/hombro[cite: 10].
  * $q_3$: Rotación del segundo eslabón/codo[cite: 10].
  * $q_4$: Rotación/Giro de la muñeca[cite: 10].
* **Eslabones o vínculos (link):** Estructuras rígidas entre cada articulación[cite: 10].
* **Efector final:** Herramienta o pinza instalada al extremo $X$[cite: 10].

**Figura 1. Estructura básica manipulador**

---

### Análisis de Parámetros de Configuración (Figura 2)

#### **Estructura y Tipos de Articulaciones:**
* **Sistema de Coordenadas de Base:** Definido por ejes cartesianos $(x, y, z)$ en el origen[cite: 10].
* **Cadena Cinemática:** Muestra un esquema antropomórfico compuesto por **1 eslabón fijo + n eslabones móviles**[cite: 10].
* **Tipos de Grados de Libertad / Articulaciones:**
  * **Articulación revoluta (1 DOF):** Representada por un círculo con eje de rotación en el hombro/codo[cite: 10].
  * **Articulación prismática (1 DOF):** Representada por un cilindro deslizante en la sección del brazo/antebrazo[cite: 10].

**Figura 2. Parámetros de configuración**

---

### Análisis de Estructura Angular / Robot Antropomórfico (Figura 4)

#### **Tipos y Representaciones de Robots Articulados:**
* **Robot angular o antropomórfico:**
  * Muestra una estructura cinemática con 3 grados de libertad rotacionales que imitan el brazo humano (Cintura, Hombro, Codo)[cite: 10].
  * Incluye diagrama en ejes $X, Y, Z$ con representación angular $3G$ y boceto del robot antropomórfico físico[cite: 10].

**Figura 4. Estructura angular**  
Fuente: (Cross, 2014)[cite: 10]

---

## 6.3. Especificación de Protocolos de Control

* Definición de estrategias de control embebido[cite: 10]

## 7. Verificación y Validación

### 7.1. Verificación del Diseño

| ID RF, RNF | Descripción del requerimiento | Diseño final | Cumple/ No cumple |
| :---: | :--- | :--- | :---: |
| RF01. | Brazo robótico con 5 grados de libertad | Ver diseño fig 5.6. | Cumple |
| | | | |

---

### 7.1.1. Pruebas Unitarias

### 7.1.2. Pruebas Integrales o de equipos (prototipo físico)

### 7.1.3. Pruebas Funcionales (prototipo físico)

### 7.1.3. Pruebas de Calidad y Cumplimiento Normativo
* Certificación de estándares

### 7.1.4. Análisis de resultados de la simulación o el prototipo
* Indicadores de Evaluación del Proyecto
* Cumplimiento de objetivos técnicos
* Satisfacción de usuarios y stakeholders
* Eficiencia operativa

---

### 7.1.5. Análisis Comparativo entre Diseño y Resultados Reales
* Diferencias entre predicciones y pruebas finales

#### **Análisis de las Simulaciones Tridimensionales (Columna Derecha):**
* Muestra cuatro etapas o configuraciones cinemáticas sucesivas del brazo manipulador en un entorno de simulación 3D (p. ej., MATLAB / Simulink / Robotics System Toolbox).
* En cada gráfico se observa el volumen de trabajo/espacio alcanzable del robot delimitado por una trayectoria elíptica/circular superior y la base sobre el plano horizontal $(X, Y, Z)$.
* Se aprecia la evolución del movimiento articular desde una posición inicial hasta la extensión completa del efector final.

---

### 7.2. Validación del Sistema
* Comparación de desempeño con los requerimientos iniciales
* Ajustes finales antes de implementación

---

## 8. Implementación y Prototipado

### 8.1. Fabricación del Prototipo
* Métodos de manufactura empleados

### 8.2. Integración de Componentes Electrónicos y de Control
* Montaje y calibración del sistema

### 8.3. Evaluación del Funcionamiento
* Comparación con simulaciones previas

---

## 9. Conclusiones y Recomendaciones

### 9.1. Conclusiones del Proyecto
* Síntesis de hallazgos clave

### 9.2. Recomendaciones para Futuros Desarrollos
* Mejoras para optimizar el sistema[cite: 12]

---

## 10. Bibliografía
* Formato ISO690[cite: 12]
* Cross, N. (2024). *Engineering Design Methods 5th Edition*. Wiley.[cite: 12]

---

## 11. Apéndices/Anexos
* Planos, cálculos detallados, esquemas de código[cite: 12]