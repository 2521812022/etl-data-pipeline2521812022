# etl-data-pipeline2521812022

Este proyecto implementa un pipeline ETL (Extracción, Transformación y Carga) en la nube utilizando las siguientes tecnologías.
* **Archivos de origen:** CSV Dataset
* **Almacenamiento de datos crudos y procesados:** GitHub
* **Procesamiento y limpieza:** Python (Google Colab)
* **Data Warehouse destino:** PostgreSQL Cloud (Render)

## Arquitectura del Pipeline
El flujo de los datos sigue esta estructura.
**CSV → GitHub → Python ETL → PostgreSQL Cloud**

Estructura del Repositorio
**`data/raw/`**: Contiene los archivos originales sin procesar (`C_clientes.csv`, `C_pagos.csv`, `C_ventas.csv`).
**`data/curated/`**: Almacena los registros que pasaron las validaciones de calidad y fueron transformados (`clientes_curated.csv`, `pagos_curated.csv`, `ventas_curated.csv`).
**`data/rejects/`**: Contiene los registros descartados durante la limpieza (`clientes_rejects.csv`), documentando el motivo del rechazo para futuras auditorías.
**`notebooks/`**: Incluye el cuaderno de Jupyter (`.ipynb`) con el código fuente en Python utilizado en Google Colab para ejecutar el proceso ETL.
