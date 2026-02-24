# Proyecto: Digitalización e Índice de Desarrollo Electrónico (IDE-EC)

Este repositorio consolida documentación, insumos y resultados asociados a la construcción y análisis del Índice de Desarrollo Electrónico de Ecuador (IDE-EC), así como componentes relacionados con Gobierno Electrónico (GOV), Tecnologías de la Información y Comunicación (TICs), pagos digitales (PAY) e indicadores económicos (ECO). El objetivo es centralizar fuentes, metodologías, cálculos y salidas para facilitar el seguimiento, la trazabilidad y la actualización del índice y sus dimensiones.


Resumen ejecutivo
- Propósito: Integrar fuentes y metodologías oficiales para estimar y documentar el IDE-EC y dimensiones relacionadas (GOV, TICs, pagos y economía), con trazabilidad de insumos y resultados.
- Cobertura: Fuentes primarias (PDF metodológicos y fichas técnicas) y secundarias (hojas de cálculo con cálculos y series) de 1965–2025 según disponibilidad.
- Estructura: Carpeta raíz con documentación general y subdirectorios temáticos: dataACC (TICs), dataECO (economía), dataGOV (gobierno electrónico), dataIDE-EC (metodologías y sustento del IDE-EC) y dataPAY (pagos electrónicos). Archivo IDE-EC.html como posible informe/visualización.
- Uso: Navegar por cada carpeta para identificar fuentes originales (PDF), plantillas y resultados (XLSX). El README detalla el contenido de arriba hacia abajo para orientar su consulta.


Estructura del repositorio (de arriba hacia abajo)

Carpeta raíz
- IDE-EC.html
  - Posible reporte o visualización HTML del IDE-EC. Útil para consulta rápida de resultados, gráficos o tableros exportados.
- Readme.md
  - Este documento. Guía principal para comprender el propósito, estructura, fuentes y cómo navegar el repositorio.

Subdirectorios temáticos

1) dataACC (TICs / Acceso y Conectividad)
- 202407_Tecnologia_de_la_Informacion_y_Comunicacion-TICs.pdf
  - Documento de referencia sobre indicadores TIC. Puede incluir definiciones, metodologías, clasificaciones y contexto sectorial.
- DATOS_CALCULADOS.xlsx
  - Hoja de cálculo con resultados procesados relacionados con TICs. Suele contener series normalizadas, índices parciales, agregaciones y limpieza.

2) dataECO (Indicadores Económicos)
- 5_Servicios.xlsx
  - Datos sobre el sector servicios (presumiblemente cuentas nacionales o indicadores sectoriales).
- Calculos ECO, hasta desde 2020.xlsx
  - Archivo de trabajo con series y cálculos económicos a partir de 2020 (limpieza, transformaciones, interpolaciones/retropolaciones, índices compuestos, etc.).
- ID_Rama.xlsx
  - Identificadores o codificación por rama/sector económico para consistencia y mapeo entre fuentes.
- Indicadores_ECO.pdf
  - Documento metodológico o informe con indicadores económicos relevantes para el IDE-EC (e.g., PIB, productividad, estructura sectorial).
- Justificacion_Indice_Compuesto_IDE_EC.pdf
  - Sustento metodológico del índice compuesto a nivel económico vinculado al IDE-EC (criterios de ponderación, normalización, escalas, validación).
- PIB Nominal Anual.pdf
  - Ficha/serie de referencia del PIB nominal anual, base para escalamiento, ponderaciones o control de consistencia.
- retropolacion_1965_2023.xlsx
  - Serie retroproyectada 1965–2023. Útil para continuidad histórica y análisis de tendencia de largo plazo.

3) dataGOV (Gobierno Electrónico)
- 15.2.1_Ficha-Metodologica_Indice-Gobierno-Electronico.pdf
  - Ficha metodológica del índice de gobierno electrónico (alineado a ODS o marcos internacionales). Incluye definiciones de indicadores, periodicidad y fuentes.
- Metodologia_GOV_Años_Impares.pdf
  - Documento que detalla la estimación del componente GOV en años impares (p.ej., cuando la fuente internacional actualiza bianualmente). Indica ajustes y supuestos.
- Technical Appendix 2024_SP Web R2.pdf
  - Apéndice técnico actualizado (2024), presumiblemente con definiciones, cambios metodológicos y notas técnicas para el componente GOV.

4) dataIDE-EC (Sustento del IDE-EC)
- Justificacion_Tecnica_IDE-EC_Ecuador.pdf
  - Documento base de justificación técnica del IDE-EC para Ecuador: definición del objetivo del índice, estructura por dimensiones, y alineación con estándares.
- nri-2025.pdf
  - Referencia al Network Readiness Index 2025 (o documento afín). Se usa para comparar, adaptar metodologías o validar el posicionamiento relativo.
- Sustento Metodológico de las Fórmulas del IDE.pdf
  - Nota técnica con la derivación formal de las fórmulas: normalización, escalado, manejo de faltantes, agregación (media aritmética/geométrica), y construcción del índice compuesto.

5) dataPAY (Pagos Electrónicos y Medios de Pago)
- Sistema Pagos Interbancarios _ PIB.pdf
  - Documento de relación conceptual o empírica entre el sistema de pagos interbancarios y el PIB, útil para medir digitalización en pagos.
- POS/ (Puntos de Venta Electrónicos)
  - Puntos de Venta Electrónicos AÑO 2020 (1).xlsx
  - Puntos de Venta Electrónicos AÑO 2021.xlsx
  - Puntos de Venta Electrónicos AÑO 2022.xlsx
  - Puntos de Venta Electrónicos AÑO 2023.xlsx
  - Contienen series de infraestructura/uso de POS por año: terminales activas, transacciones, montos, densidad por población o por comercio, etc.
- RETIROS/ (Extracciones de efectivo)
  - retiros de dinero año 2022.xlsx
  - Retiros de Dinero DICIEMBRE 2023.xlsx
  - Retiros de Dinero DICIEMBRE 2024.xlsx
  - retiros-dinero-dic-2020.xlsx
  - retiros-dinero-dic-2021.xlsx
  - Series de retiros de efectivo mensuales/anuales para evaluar sustitución efectivo–digital y adopción de pagos electrónicos.


Metodología y trazabilidad (alto nivel)
- Normalización y escalas: Los indicadores se transforman a una escala común (p.ej., min–max [0,1] o z-score), según lo definido en “Sustento Metodológico de las Fórmulas del IDE.pdf”.
- Agregación: Se combinan indicadores en subdimensiones y dimensiones (TICs, GOV, PAY, ECO) con ponderaciones justificadas en “Justificacion_Indice_Compuesto_IDE_EC.pdf” y “Justificacion_Tecnica_IDE-EC_Ecuador.pdf”.
- Manejo de faltantes y años impares: Para GOV y otros indicadores con periodicidad irregular, se aplican técnicas de interpolación/retropolación (“retropolacion_1965_2023.xlsx” y “Metodologia_GOV_Años_Impares.pdf”).
- Validación: Se contrasta con índices de referencia (p.ej., “nri-2025.pdf”) y coherencia macroeconómica (PIB, estructura sectorial, “Indicadores_ECO.pdf”).


Guía de uso
- Consulta rápida de resultados: Abrir IDE-EC.html en un navegador para revisar visualizaciones, tablas resumen y hallazgos clave.
- Revisión metodológica: Iniciar por dataIDE-EC para comprender la arquitectura del índice y sus fórmulas; luego dataGOV, dataACC, dataPAY y dataECO para el detalle por componente.
- Replicación de cálculos: Usar los archivos XLSX (dataACC, dataECO, dataPAY) como base de trabajo. Mantener la trazabilidad documentando cualquier ajuste en nuevas hojas/tablas y conservando copias de seguridad con fecha.
- Actualizaciones: Cuando existan nuevas publicaciones (e.g., GOV 2026, NRI, cuentas nacionales), añadir los PDF a su carpeta temática y extender las hojas XLSX con nuevas series y anotaciones metodológicas.


Buenas prácticas de mantenimiento
- Versionado: Si se utiliza control de versiones, acompañar cada actualización con un registro de cambios (changelog) indicando fuentes agregadas, fórmulas ajustadas y periodos ampliados.
- Nomenclatura: Estandarizar nombres de archivos y hojas en XLSX (p.ej., AAAA_mes, indicador_unidad, ámbito_geográfico) para facilitar merges y scripts futuros.
- Documentación: Incluir notas dentro de cada XLSX explicando transformación de variables, supuestos y validaciones intermedias.
- Control de calidad: Antes de publicar resultados, verificar consistencia entre dimensiones (TICs, GOV, PAY, ECO) y validar con fuentes oficiales.


Glosario mínimo
- IDE-EC: Índice de Desarrollo Electrónico – indicador compuesto que sintetiza capacidades de digitalización y adopción tecnológica.
- TICs: Tecnologías de la Información y Comunicación.
- GOV: Gobierno Electrónico – disponibilidad/uso de servicios públicos digitales y soporte institucional.
- PAY: Pagos Electrónicos – infraestructura y adopción de medios de pago digitales.
- ECO: Indicadores Económicos – contexto macroeconómico y sectorial para la digitalización.


Créditos y contacto
- Compilación y análisis: Equipo responsable del IDE-EC.
- Fuentes: Publicaciones oficiales, metodologías internacionales y bases administrativas citadas en cada documento PDF y XLSX.
- Contacto: Indicar correo institucional o punto focal para solicitudes y aclaraciones técnicas.


Licencia
- Si no se especifica lo contrario, asumir uso interno/educativo. Para difusión pública, completar esta sección con la licencia aplicable (p.ej., CC BY 4.0, MIT para código, o restricciones de uso para datos de terceros).