# Proyecto de Equipo - MLOps

Este repositorio contiene la estructura base y la pipeline inicial para el desarrollo de un modelo de **Machine Learning para la predicción de precios de venta de vehículos usados multimarca** para la actividad 1 - MLOps.

El proyecto utiliza **datos sintéticos reproducibles** diseñados con relaciones causales reales (depreciación por año y kilometraje, factores de marca y tipo de vehículo).

---

## 📁 Estructura del Repositorio

La arquitectura del repositorio se basa en un proyecto de Python administrado con Poetry, separando la lógica de código de los artefactos de datos y modelos:

```text
PROYECTO_DE_EQUIPO/
├── configs/                # Archivos de configuración de hiperparámetros y pipelines
├── data/                   # Almacenamiento local de datasets (car_sales_dataset.csv)
├── flows/                  # Almacenamiento local de datasets (car_sales_dataset.csv)
│   ├── prueba_flow.py      # Script de prueba
├── model/                  # Modelos entrenados, métricas y artefactos
├── services/               # Servicios 
│   ├── docker-compose.yml  # Servicios para levantar docker compose para MLflow y Prefect
├── src/                    # Código fuente del proyecto
│   ├── generate_data.py    # Script reproducible para la generación del dataset sintético
├── .gitignore              # Ignorar archivos
├── poetry.lock             # Bloqueo de versiones exactas de dependencias
├── pyproject.toml          # Configuración del proyecto y gestión de dependencias con Poetry
└── README.md               # Documentación general del proyecto
```

## 🛠️ Tecnologías Utilizadas
Lenguaje: Python 3.14

Gestión de Entorno y Dependencias: Poetry

Procesamiento de Datos: Pandas, NumPy

Manejo de Rutas del Sistema: Pathlib

Control de Versiones: Git / GitHub
