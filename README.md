# Data Architecture: Cloud vs On-Premise

Este repositorio recoge una comparativa completa entre arquitecturas de datos modernas en los principales entornos cloud (AWS, Azure, GCP) y su equivalente on-premise basada en herramientas open source. El objetivo es mostrar cómo mantener una estructura modular y escalable independientemente del proveedor, siguiendo un enfoque tipo Medallion Architecture (bronze → silver → gold).

## 📐 Estructura modular por capas

Las arquitecturas están organizadas en las siguientes capas funcionales:

1. **Ingesta de datos**
2. **Almacenamiento por capas (bronze/silver/gold)**
3. **Procesamiento distribuido (Spark)**
4. **Catalogación y metadatos**
5. **Gobierno del dato**
6. **Orquestación de pipelines**
7. **Consumo analítico / visualización**

## ☁️ Arquitecturas Cloud incluidas:
- **AWS + Databricks**
- **Azure + Databricks**
- **Google Cloud (GCP) + Databricks**

Cada una incluye su propio diagrama y descripción.

## 🏠 Arquitectura On-Premise
Arquitectura basada en herramientas open source equivalentes:
- Apache NiFi, HDFS, Spark, Hive Metastore, Apache Iceberg, Apache Atlas, Apache Airflow, Apache Druid, Trino, Apache Superset.

Diseñada para replicar las funcionalidades cloud con independencia tecnológica y control local completo.

## 🔄 Comparativa de tecnologías por capa

| Capa | AWS | Azure | GCP | On-Premise |
|------|-----|-------|-----|------------|
| Ingesta | Lambda | Azure Functions | Cloud Functions | NiFi |
| Almacenamiento | S3 | ADLS Gen2 | GCS | HDFS |
| Procesamiento | Databricks (Spark) | Databricks (Spark) | Databricks (Spark) | Apache Spark |
| Catálogo | AWS Glue | Azure Purview | Dataplex | Hive Metastore |
| Gobierno del dato | Lake Formation | Purview | Dataplex | Apache Atlas |
| Orquestación | Step Functions | Data Factory | Cloud Composer | Apache Airflow |
| Analítica avanzada | Redshift | Synapse | BigQuery | Apache Druid |
| Visualización | QuickSight | Power BI | Looker | Apache Superset |

## 📎 Archivos incluidos
- Diagramas en PDF de cada arquitectura
- Tabla comparativa
- Este README como documentación explicativa

## 💬 ¿Por qué este proyecto?
Este repositorio no solo busca mostrar equivalencias técnicas, sino también demostrar cómo un ingeniero de datos puede pensar en términos arquitectónicos, entender el flujo completo del dato y adaptar soluciones de forma estratégica.


---

📌 *Autor: David González Ternero*

