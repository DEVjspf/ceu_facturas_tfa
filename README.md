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
3. Extracción de texto desde PDFs. Coloca los PDFs de las facturas en la carpeta data/facturas/.

4. Ejecuta el notebook principal dev_facturas.ipynb que realiza:

* Extracción de texto desde PDFs.
* Fragmentación semántica y generación de embeddings.
* Almacenamiento en ChromaDB.
* Consulta y extracción estructurada mediante modelos LLM.
* Validación con Pydantic.
* Evaluación con métricas F1 y recall.
* Exportación de resultados a CSV y Excel.

## 🔩 Estructura JSON y esquema Pydantic

El esquema de datos validado con Pydantic es el siguiente:
```
{
  "numero_factura": "string",
  "fecha_emision": "YYYY-MM-DDTHH:MM:SS",
  "periodo_inicio": "YYYY-MM-DDTHH:MM:SS",
  "periodo_fin": "YYYY-MM-DDTHH:MM:SS",
  "consumo_total_kwh": float,
  "potencia_punta_kw": float,
  "potencia_valle_kw": float,
  "importe_total": float
}
```
## 📄 Licencia 
Este proyecto está bajo la Licencia [LICENSE.txt](https://github.com/DEVjspf/ceu_facturas_tfa/blob/main/LICENSE.txt) consulta el archivo para mas detalles 

## ✒️ Autores 
* Maria Angel Lobon Gonzalo
* Elisban Montañez Montalvo
* J. Samuel Porcayo Fraustro
* Cesar Damian Celis

