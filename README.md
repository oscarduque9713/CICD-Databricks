
# ETL Ecommerce Brazilian

Arquitectura Medallion en Azure Databricks

Pipeline automatizado de datos para análisis de ordenes y la suma de las ventas en Brasil con arquitectura de tres capas y despliegue continuo.

🎯 Descripción
Pipeline ETL que transforma datos crudos de ordenes, clientes y vendedores de Brasil, implementando la Arquitectura Medallion (Bronze-Silver-Gold) en Azure Databricks y una capa extra(raw) en la cual se descargan los archivos de kaggle via API con CI/CD completo y Delta Lake para garantizar consistencia ACID.

✨ Características Principales
🔄 ETL Automatizado - Pipeline completo con despliegue automático via GitHub Actions
🏗️ Arquitectura Medallion - Separación clara de capas raw → Bronze → Silver → Gold
📊 Modelo Dimensional - One Big Table optimizado para análisis de negocio
🚀 CI/CD Integrado - Deploy automático en cada push a master
📈 Databricks Dashboards - Visualización
⚡ Delta Lake - ACID transactions y time travel capabilities
🔔 Monitoreo - Notificaciones automáticas y logs detallados

🏛️ Arquitectura

Flujo de Datos

📄 CSV (Raw Data)
↓
📄 Raw layer( Descarga archivos)
↓
🥉 Bronze Layer (Ingesta sin transformación)
↓
🥈 Silver Layer (Limpieza + Modelo Dimensional)
↓
🥇 Gold Layer (Agregaciones de Negocio)
↓
📊 BI Dashboards (Visualización)

![Gemini_Generated_Image_i6skvdi6skvdi6sk.png](./Imagenes/Gemini_Generated_Image_i6skvdi6skvdi6sk.png "Gemini_Generated_Image_i6skvdi6skvdi6sk.png")
