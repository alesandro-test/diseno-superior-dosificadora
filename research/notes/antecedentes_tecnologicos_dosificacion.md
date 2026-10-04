# Antecedentes tecnológicos de dosificación para panificación

**Estado:** fuentes originales verificadas; material preparado para el estado del arte o marco teórico  
**Fecha de consulta:** 2026-09-09

**Actualización de acceso, 2026-09-10:** se reconsultó el PDF original completo de Humaira et al. en `https://jurnal.polinema.ac.id/index.php/elkolind/article/download/3298/3482`. La tabla 6, página 93, identifica las cantidades de recetas utilizadas en la comparación del planteamiento. Rumapea devolvió 403 durante esta ronda: la ficha previa se conserva como historial, pero ese trabajo no se cita en la nueva introducción. No se trasladan resultados de desempeño de ningún antecedente al caso San Miguel.

## Criterio de uso

### Verificación de Farihin, 13/09/2026

Se leyó el artículo publicado completo, páginas F121–F126, en la [copia del PDF alojada por Semantic Scholar](https://pdfs.semanticscholar.org/a050/25275bf710c395f752afb6fa9f14789cc9e8.pdf). El título, autores, revista, volumen y páginas coinciden con `farihin2021premix`. Copia local: `docs/thesis/bibliography/farihin2021premix.pdf` (los PDF bibliográficos están excluidos de Git).

- **F123, sección III.A:** el control acciona las compuertas de las tolvas y recibe realimentación del sensor de peso.
- **F124, sección III.C:** cinco tolvas, mecanismo deslizante accionado por motor paso a paso NEMA 23, celda de carga de 1 kg y servomotores para tamizado y descarga.
- **F124, sección III.B, y F125, conclusiones:** la configuración final utiliza PI; no atribuirle un controlador PID final con término derivativo activo.

La cita respalda mecanismos de alimentación, pesaje y control de ingredientes de panificación. Los ingredientes de la premezcla enumerados en F121/F124 no incluyen harina; no atribuirle ensayo de dosificación de harina ni trasladar resultados a San Miguel. La frase general de la Introducción conserva ese alcance. Verificación de componentes cerrada; no equivale a validar todos los resultados del artículo.

La nota de acceso del 10/09/2026 sobre la exclusión de Rumapea describe aquella versión de la Introducción. La versión aceptada el 13/09/2026 conserva su cita para identificar un antecedente de dosificación de harina, sin adoptar sus parámetros o resultados.

Los trabajos siguientes orientan la identificación de arquitecturas, componentes y variables de evaluación. Sus escalas y condiciones experimentales difieren del procedimiento registrado en la Panadería San Miguel. En consecuencia, sus resultados no constituyen tolerancias, valores esperados ni demostraciones de desempeño para el proyecto.

## Comparación

| Antecedente | Aplicación | Configuración relevante | Límite de comparación con San Miguel |
|---|---|---|---|
| Farihin, Priambodo y Al Khindi (2021) | Dosificación de premezcla para pan dulce | Tolvas, sensores de masa, actuadores y control proporcional-integral | Equipo multingrediente de escala experimental |
| Humaira, Dewatama y Al Azhar (2024) | Dosificación de harina, azúcar y leche en polvo | Celda de carga, controlador y accionamiento regulado | Consignas inferiores a las masas de los lotes observados en San Miguel |
| Rumapea et al. (2026) | Dosificación de harina para panaderías pequeñas y medianas | Tolva, compuerta, celda de carga y alimentación en dos etapas | Ensayos de laboratorio con masas de 10, 30 y 50 g |

## Síntesis para desarrollo posterior

Los antecedentes revisados presentan configuraciones de escala reducida para automatizar la dosificación de ingredientes de panificación. Farihin, Priambodo y Al Khindi integraron tolvas, sensores de masa y actuadores para preparar una premezcla de pan dulce. Humaira, Dewatama y Al Azhar utilizaron una celda de carga como realimentación de un sistema destinado a harina, azúcar y leche en polvo. Rumapea et al. estudiaron una dosificadora de harina compuesta por tolva, compuerta, medición de masa y dos etapas de alimentación. Estos trabajos aportan componentes y estrategias para el análisis de alternativas. Sin embargo, las escalas, formulaciones y condiciones experimentales difieren del procedimiento observado en San Miguel; por esta razón, los requerimientos del proyecto se establecen a partir de los registros internos del caso.

## Referencias verificadas

1. Farihin, M. M., Priambodo, J. y Al Khindi, B. (2021). *Sistem Penakar Bahan Baku Premix Roti Manis Menggunakan Metode PID*. **Jurnal Teknik ITS, 10**(2), F121–F126. DOI: [10.12962/j23373539.v10i2.68131](https://doi.org/10.12962/j23373539.v10i2.68131).
2. Humaira, N., Dewatama, D. y Al Azhar, G. (2024). *Optimalisasi Sistem Penakar Bahan Baku Roti Otomatis Menggunakan Kontrol PID*. **Jurnal Elektronika dan Otomasi Industri, 11**(1), 85–94. DOI: [10.33795/elkolind.v11i1.3298](https://doi.org/10.33795/elkolind.v11i1.3298).
3. Rumapea, E. S. E., Robbani, H., Anugrah, I., Pertiwi, E. P. y Wijayanti, W. (2026). *Design and Development of An Optimized Automatic Flour Dosing Machine for SME Bakeries*. **Jurnal INTECH Teknik Industri Universitas Serang Raya, 12**(1), 44–54. DOI: [10.30656/intech.v12i1.12030](https://doi.org/10.30656/intech.v12i1.12030).

Las entradas BibLaTeX correspondientes se encuentran en `docs/thesis/bibliography/referencias.bib` con las claves `farihin2021premix`, `humaira2024optimalisasi` y `rumapea2026flour`.
