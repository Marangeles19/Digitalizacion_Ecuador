# 📊 Índice de Digitalización Económica del Ecuador (IDE-EC)

## Descripción General

**IDE-EC** es una plataforma interactiva web que calcula y visualiza el **Índice de Digitalización Económica del Ecuador**, una métrica integral que mide el nivel de modernización tecnológica y su impacto en la productividad y desarrollo sostenible del país.

---

## 🎯 Objetivo del Proyecto

Proporcionar una herramienta de **análisis y seguimiento** de cuatro pilares clave de la digitalización ecuatoriana:

- **GOV** (Gobierno Digital): Capacidad institucional y servicios electrónicos del sector público
- **ACC** (Acceso Tecnológico): Cobertura de conectividad e inclusión digital
- **ECO** (Economía Digital): Participación de sectores digitales en el PIB
- **PAY** (Pagos Electrónicos): Adopción de sistemas de pago digital y reducción del efectivo

Estos cuatro indicadores se combinan mediante **pesos ponderados** para calcular un índice sintético (IDE-EC) que refleja la transformación digital del país.

---

## 📁 Estructura del Repositorio
Digitalizacion_Ecuador/ │ ├── IDE-EC.html # 🎯 ARCHIVO PRINCIPAL (Interfaz Web) │ ├── dataIDE-EC/ # 📚 DOCUMENTACIÓN TÉCNICA IDE-EC │ ├── Justificacion_Tecnica_IDE-EC_Ecuador.pdf │ ├── nri-2025.pdf │ └── Sustento Metodológico de las Fórmulas del IDE.pdf │ ├── dataGOV/ # 🏛️ FUENTES DE GOBIERNO DIGITAL │ ├── Metodologia_GOV_Años_Impares.pdf │ ├── 15.2.1_Ficha-Metodologica_Indice-Gobierno-Electronico.pdf │ └── Technical Appendix 2024_SP Web R2.pdf (Naciones Unidas) │ ├── dataACC/ # 📡 FUENTES DE ACCESO TECNOLÓGICO │ ├── 202407_Tecnologia_de_la_Informacion_y_Comunicacion-TICs.pdf │ └── DATOS_CALCULADOS.xlsx │ ├── dataECO/ # 💰 FUENTES DE ECONOMÍA DIGITAL │ ├── 5_Servicios.xlsx (Datos de exportaciones) │ ├── ID_Rama.xlsx (Datos de IDE por rama) │ ├── retropolacion_1965_2023.xlsx (Valor agregado bruto histórico) │ ├── Calculos ECO, hasta desde 2020.xlsx │ └── PIB Nominal Anual.pdf │ └── dataPAY/ # 💳 FUENTES DE PAGOS ELECTRÓNICOS │ ├── Sistema Pagos Interbancarios _ PIB.pdf (Giro digital) │ ├── POS/ (Puntos de venta electrónicos) │ ├── Puntos de Venta Electrónicos AÑO 2020 (1).xlsx │ ├── Puntos de Venta Electrónicos AÑO 2021.xlsx │ ├── Puntos de Venta Electrónicos AÑO 2022.xlsx │ └── Puntos de Venta Electrónicos AÑO 2023.xlsx │ └── RETIROS/ (Retiros de efectivo) ├── retiros-dinero-dic-2020.xlsx ├── retiros-dinero-dic-2021.xlsx ├── retiros-dinero-dic-2022.xlsx ├── retiros-dinero-dic-2023.xlsx └── Retiros de Dinero DICIEMBRE 2024.xlsx

---

## 📄 Descripción de Archivos

### 🎯 Raíz del Proyecto

#### **IDE-EC.html**
**Ubicación:** `/IDE-EC.html`

Archivo HTML principal y **único archivo de interfaz web**. Contiene:

- **Frontend completo** (HTML + CSS + JavaScript)
- **Interfaz interactiva** con temas claro/oscuro
- **Calculadora de indicadores** en tiempo real
- **Gestión de datos** (almacenamiento local en localStorage)
- **Visualización de gráficos** mediante Chart.js
- **Sistema de navegación** por 6 pestañas (IDE-EC, GOV, ACC, ECO, PAY, Beneficios)

**Características principales:**
- ✅ Cálculo automático de IDE-EC según la fórmula: `IDE-EC = wGOV×GOV + wACC×ACC + wECO×ECO + wPAY×PAY`
- ✅ Edición de pesos para cada componente
- ✅ Gestión de múltiples años
- ✅ Tabla resumen con tendencias históricas
- ✅ Gráficos de barras con gradientes
- ✅ Panel de beneficios de la digitalización

---

### 📚 Carpeta: `dataIDE-EC/` - Justificación Técnica

**Ubicación:** `/dataIDE-EC/`

Contiene la **documentación técnica del marco metodológico** del IDE-EC:

| Archivo | Propósito |
|---------|-----------|
| `Justificacion_Tecnica_IDE-EC_Ecuador.pdf` | **Documento principal** explicando la definición, justificación y pesos asignados a cada componente |
| `nri-2025.pdf` | Referencia a índices internacionales de digitalización (Network Readiness Index 2025) |
| `Sustento Metodológico de las Fórmulas del IDE.pdf` | Detalles matemáticos y derivación de las fórmulas de cálculo |

**Cómo se usan:**
- Se enlazan en la sección IDE-EC de la herramienta bajo "Links / fuentes (PDF)"
- Son referencias para entender por qué se eligieron estos indicadores

---

### 🏛️ Carpeta: `dataGOV/` - Gobierno Digital (GOV)

**Ubicación:** `/dataGOV/`

Contiene **fuentes para el indicador GOV** (escala 0-1), que mide la capacidad de gobierno electrónico:

| Archivo | Propósito |
|---------|-----------|
| `Metodologia_GOV_Años_Impares.pdf` | Explicación de metodología aplicada a años impares (2021, 2023, 2025) |
| `15.2.1_Ficha-Metodologica_Indice-Gobierno-Electronico.pdf` | Ficha técnica del índice de gobierno electrónico |
| `Technical Appendix 2024_SP Web R2.pdf` | Documento técnico de Naciones Unidas (E-Government Index) |


**Rango:** 0 a 1 (donde 1 = máximo desarrollo digital)

---

### 📡 Carpeta: `dataACC/` - Acceso Tecnológico (ACC)

**Ubicación:** `/dataACC/`

Contiene **fuentes para el indicador ACC** (escala 0-1), que mide penetración de tecnología e inclusión digital:

| Archivo | Propósito |
|---------|-----------|
| `202407_Tecnologia_de_la_Informacion_y_Comunicacion-TICs.pdf` | Encuesta Nacional de TICs (julio 2024) con datos de hogares y empresas |
| `DATOS_CALCULADOS.xlsx` | Hoja de cálculo con indicadores ya procesados y validados |


**Rango:** 0 a 1 (donde 1 = máxima inclusión tecnológica)

---

### 💰 Carpeta: `dataECO/` - Economía Digital (ECO)

**Ubicación:** `/dataECO/`

Contiene **fuentes para el indicador ECO** (en porcentaje %), que mide el peso de sectores digitales en la economía:

| Archivo | Propósito |
|---------|-----------|
| `5_Servicios.xlsx` | Exportaciones de servicios digitales (por rama económica) |
| `ID_Rama.xlsx` | Inversión en Digitalización por rama industrial |
| `retropolacion_1965_2023.xlsx` | Serie histórica del Valor Agregado Bruto (VAB) desde 1965 |
| `Calculos ECO, hasta desde 2020.xlsx` | Hojas de trabajo con cálculos del ECO desde 2020 |
| `PIB Nominal Anual.pdf` | Tabla del PIB nominal anual del Ecuador |


**Rango:** 0% a ∞% (típicamente 10%-40%, representa la "intensidad digital" de la economía)

---

### 💳 Carpeta: `dataPAY/` - Pagos Electrónicos (PAY)

**Ubicación:** `/dataPAY/`

Contiene **fuentes para el indicador PAY** (en porcentaje %), que mide la adopción de sistemas de pago digital:

#### 📊 Archivo Principal
| Archivo | Propósito |
|---------|-----------|
| `Sistema Pagos Interbancarios _ PIB.pdf` | Datos de volumen de transacciones interbancarias (Giro Digital = GD) |

#### 🛒 Subcarpeta: `POS/` - Puntos de Venta Electrónicos

Contiene **datos anuales de POS** (terminales de venta):
POS/ ├── Puntos de Venta Electrónicos AÑO 2020 (1).xlsx ├── Puntos de Venta Electrónicos AÑO 2021.xlsx ├── Puntos de Venta Electrónicos AÑO 2022.xlsx └── Puntos de Venta Electrónicos AÑO 2023.xlsx


**Uso:** Número de transacciones exitosas (POS) anualmente

#### 🏧 Subcarpeta: `RETIROS/` - Retiros de Efectivo

Contiene **datos anuales de retiros de efectivo**:

RETIROS/ ├── retiros-dinero-dic-2020.xlsx ├── retiros-dinero-dic-2021.xlsx ├── retiros-dinero-dic-2022.xlsx ├── retiros-dinero-dic-2023.xlsx └── Retiros de Dinero DICIEMBRE 2024.xlsx

**Uso:** Número de transacciones de retiro de efectivo (RET) anualmente

**Fórmula de PAY:**
PAY = sqrt((GD/2) × (POS / (POS + RET))) × 100

Donde:

GD = Giro Digital (volumen de transacciones interbancarias)
POS = Transacciones en punto de venta
RET = Retiros de efectivo
(POS + RET) = Total de transacciones de pago
POS/(POS+RET) = Ratio de "cashlessness" (menor efectivo)

    ⬇️ VISUALIZACIÓN
---

## 🚀 Cómo Usar la Herramienta

### 1️⃣ Acceder a la herramienta
Abre **IDE-EC.html** en tu navegador web:
```bash
Haz doble clic en IDE-EC.html



