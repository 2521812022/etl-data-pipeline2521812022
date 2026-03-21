# etl-data-pipeline2521812022

[cite_start]Este proyecto implementa un pipeline ETL (Extracción, Transformación y Carga) en la nube utilizando las siguientes tecnologías [cite: 396-401]:
* **Archivos de origen:** CSV Dataset
* **Almacenamiento de datos crudos y procesados:** GitHub
* **Procesamiento y limpieza:** Python (Google Colab)
* **Data Warehouse destino:** PostgreSQL Cloud (Render)

## Arquitectura del Pipeline
[cite_start]El flujo de los datos sigue esta estructura [cite: 402-403, 944]:
**CSV → GitHub → Python ETL → PostgreSQL Cloud**

## [cite_start]Estructura del Repositorio [cite: 359-376]
* [cite_start]**`data/raw/`**: Contiene los archivos originales sin procesar (`C_clientes.csv`, `C_pagos.csv`, `C_ventas.csv`) [cite: 362-364].
* [cite_start]**`data/curated/`**: Almacena los registros que pasaron las validaciones de calidad y fueron transformados (`clientes_curated.csv`, `pagos_curated.csv`, `ventas_curated.csv`) [cite: 366, 862, 871-877].
* [cite_start]**`data/rejects/`**: Contiene los registros descartados durante la limpieza (`clientes_rejects.csv`), documentando el motivo del rechazo para futuras auditorías [cite: 368, 863, 888-895].
* [cite_start]**`notebooks/`**: Incluye el cuaderno de Jupyter (`.ipynb`) con el código fuente en Python utilizado en Google Colab para ejecutar el proceso ETL [cite: 370-371, 1108-1110].
