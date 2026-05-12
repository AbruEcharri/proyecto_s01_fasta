# Análisis de Secuencias Proteicas: Proteoma de Escherichia coli (K-12 MG1655)

Este proyecto consiste en el procesamiento, estructuración y análisis exploratorio de datos (EDA) del proteoma de la bacteria _Escherichia coli_ (cepa K-12 MG1655), uno de los organismos modelo más importantes en la biología molecular.

El objetivo principal es transformar datos biológicos crudos (formato FASTA) en información estructurada para extraer _insights_ sobre los patrones ocultos en sus proteínas y cómo la bacteria optimiza sus recursos."

## 📌 Estructura del Proyecto

El análisis se divide en 6 bloques lógicos que guían el flujo de trabajo:

1. **Introducción y Exploración de Datos Crudos:** Inspección inicial del archivo FASTA descargado del NCBI.
2. **Extracción y Estructuración Manual:** Implementación de un algoritmo de parseo propio para separar IDs de secuencias sin librerías externas.
3. **Estructuración en Pandas:** Conversión de los datos procesados en un `DataFrame` para un manejo profesional y escalable.
4. **Ingeniería de Características (_Feature Engineering_):** Cálculo de métricas cuantitativas como la longitud de las proteínas y la frecuencia de cada aminoácido.
5. **Análisis Exploratorio Visual (EDA):** Visualización de la distribución de longitudes y la abundancia global de aminoácidos mediante histogramas y gráficos de barras.
6. **Validación (_Sanity Check_):** Comparación de los resultados obtenidos manualmente contra la librería estándar **BioPython** para asegurar la precisión del proceso.

## 💡 Insights Clave del Análisis

- **Optimización Energética:** Se identificó que la _E. coli_ prioriza la síntesis de proteínas cortas (0-500 aminoácidos) para minimizar el gasto de ATP y acelerar su ritmo de reproducción.
- **Preferencia de Aminoácidos:** Los datos muestran una clara abundancia de aminoácidos estructuralmente simples como la Leucina (L) y la Alanina (A). En contraste, los aminoácidos complejos y costosos de sintetizar, como el Triptófano (W) y la Cisteína (C), se reservan para funciones específicas.

## 🛠️ Tecnologías Utilizadas

- **Python 3**
- **Pandas:** Manipulación y limpieza de datos estructurados.
- **Matplotlib & Seaborn:** Visualizaciones estadísticas.
- **BioPython:** Validación y control de calidad de secuencias.
- **Lógica de Programación:** Desarrollo de algoritmos de procesamiento de texto.

## 📂 Organización de Carpetas

```text
├── data/
│   └── raw/              # Archivo FASTA original (sequence.fasta)
├── notebooks/
│   └── 01_analisis_secuencias.ipynb   # Notebook principal con el análisis
└── README.md             # Descripción del proyecto
```
