# Analisis de Accidentes de Transito de Colombia

Este repositorio contiene un proyecto completo de análisis de datos que aborda los accidentes de tránsito ocurridos en Colombia entre marzo de 2017 y diciembre de 2022. El objetivo es identificar patrones temporales, geográficos y por tipo de accidente para generar conocimientos que puedan apoyar estrategias de seguridad vial.

Este repositorio contiene un análisis completo de los accidentes de tránsito en Colombia. Incluye limpieza de datos, análisis exploratorio y visualizaciones interactivas mediante Power BI.

## Estructura del proyecto

- `data/raw/`: Datos originales (sin modificar)
- `data/processed/`: Datos limpios y transformados
- `notebooks/`: Análisis exploratorio en Jupyter Notebooks
- `scripts/`: Scripts de Python para limpieza y transformación
- `dashboards/`: Dashboard interactivo en Power BI
- `images/`: Imágenes y visualizaciones usadas en el README


## Objetivo

Identificar patrones en los accidentes de tránsito para proponer mejoras en la seguridad vial.

# Datos originales

Los datos de accidentes de tránsito en Colombia se obtuvieron del portal de Datos Abiertos del Gobierno de Colombia:

- Fuente: [Accidentalidad vial en Colombia](https://www.datos.gov.co/Transporte/ACCIDENTES-DE-TRANSITO-DESDE-MARZO-2017-A-DICIEMBR/wacd-xkg8/about_data)
- Formato: CSV
- Ubicación: `/data/raw/ACCIDENTES_DE_TRANSITO_DESDE_MARZO__2017_A_DICIEMBRE_DE_2022_20250527 (1)`


# 02 - Transformación de Datos para Power BI
Este notebook genera los archivos CSV agregados que alimentarán el dashboard en Power BI.

Tabla de hechos: hechos_accidentes.csv
Contendrá:

# ID (opcional)
# ID_fecha
# ID_departamento
# ID_municipio
# ID_tipo_accidente
# Número de heridos
# Número de muertos
# Total de accidentes (1 por fila o agregados)

🔹 Dimensiones:
# dim_fecha.csv: fecha, año, mes, día de semana, etc.
# dim_departamento.csv: ID, nombre del departamento
# dim_municipio.csv: ID, nombre del municipio
# dim_tipo_accidente.csv: ID, nombre del tipo de accidente