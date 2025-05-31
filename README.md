# Extracción y Gestión de Datos de Facturas Eléctricas

## 📋 Descripción

El proyecto desarrolla un sistema para extraer datos estructurados de facturas eléctricas PDF, empleando técnicas de NLP, fragmentación semántica, embeddings para búsqueda eficiente y modelos LLM para generación y validación de respuestas. Se incluyen esquemas de datos validados con Pydantic, y se evalúan los resultados mediante métricas como F1 y recall para asegurar la precisión en la extracción. Además, se utilizan bases de datos vectoriales para almacenamiento y recuperación de contexto.

## 📦 Contenido del repositorio:

* Código fuente implementado en notebooks Jupyter que incluye:
* Extracción de texto desde PDFs de facturas eléctricas.
* Definición de esquema Pydantic para validar datos extraídos.
* Fragmentación semántica y generación de embeddings para búsqueda eficiente.
* Integración con modelos LLM para extracción estructurada de datos.
* Validación y evaluación con métricas de precisión (F1, recall).
* Documentación: Memoria en PDF con análisis de requisitos, diagramas, diseño, pruebas y evaluación.
* Datos de entrada: Conjunto de 4 a 6 facturas eléctricas en formato PDF para pruebas.
* Hojas de cálculo: Resultados de evaluación exportados en CSV y Excel.
* Licencia: Proyecto bajo licencia GNU GPL v3.

## ⚙️ Cómo ejecutar el proyecto

1. Clonar el repositorio.
2. Instalar dependencias con pip install -r  [requirements.txt](https://github.com/DEVjspf/ceu_facturas_tfa/blob/main/requirements.txt)
```
pip install -r requirements.txt
```

Ejecutar el notebook principal dev_facturas.ipynb que contiene:

* Extracción de texto desde PDFs.
* Procesamiento y generación de embeddings.
* Consulta y respuesta con modelos generativos.
* Validación y evaluación de resultados.


