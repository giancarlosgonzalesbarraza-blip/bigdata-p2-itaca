# Proyecto N · [Título del proyecto]

> **Plantilla.** Sustituye todo lo que va entre corchetes y borra las indicaciones en cursiva a medida que completes cada sección. Borra también las secciones de bloques que tu proyecto no trabaje.

## Descripción y objetivo

Se extraen datos de una base relacional, utilizamos este tipo de base para probar con datos rigidos, ademas estas utilizan tablas que seran organizadas para poder ser entendidas por MongoDB. Luego de la limpieza, cálculo de indicadores con Spark y la orquestación automatica con Airflow.
El objetivo es tratar con una base diferente a la anterior y lograr un dashboard interactivo.

## Arquitectura



```mermaid
graph LR
    A[Fuente de datos (tablas)] --> B[Ingesta desde PSQL]
    B --> C[Almacenamiento en Data Lake]
    C --> D[Procesamiento con Spark]
    D --> E[Visualización / modelo (Power BI)]