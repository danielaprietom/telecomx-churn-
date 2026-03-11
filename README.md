# TelecomX — Análisis de Evasión de Clientes

Este repositorio contiene mi análisis del Challenge 2 de Data Science de Alura LATAM. El objetivo del proyecto es entender por qué los clientes de Telecom X cancelan el servicio (lo que se conoce como "churn") y qué factores están detrás de esa decisión.

---

## ¿De qué trata el proyecto?

Telecom X tiene una tasa de cancelación alta y necesita entender a quiénes está perdiendo y por qué. En este análisis trabajé con datos reales de clientes, hice una limpieza completa, exploré las variables más relevantes y saqué conclusiones que el equipo de ciencia de datos puede usar para construir modelos predictivos o diseñar estrategias de retención.

El flujo que seguí fue:
1. Extraer los datos desde una API en formato JSON
2. Limpiarlos y transformarlos (ETL)
3. Analizar las variables numéricas y categóricas
4. Crear visualizaciones para entender los patrones
5. Escribir un informe con conclusiones y recomendaciones

---

## Archivos del repositorio

```
telecomx-churn/
├── TelecomX_Analisis_Churn.ipynb   ← notebook principal con todo el análisis
└── README.md                        ← este archivo
```

---

## Tecnologías usadas

- Python 3
- pandas
- numpy
- matplotlib
- seaborn
- requests

---

## Cómo ejecutarlo

Si querés correr el notebook vos mismo, la forma más simple es abrirlo en Google Colab sin instalar nada:

1. Entrá a [colab.research.google.com](https://colab.research.google.com)
2. File → Open notebook → pestaña GitHub
3. Pegá la URL de este repositorio
4. Abrí `TelecomX_Analisis_Churn.ipynb`
5. Ejecutar todo (`Ctrl + F9`)

Si preferís correrlo localmente:

```bash
git clone https://github.com/TU_USUARIO/telecomx-churn.git
cd telecomx-churn
pip install pandas numpy matplotlib seaborn requests
jupyter notebook TelecomX_Analisis_Churn.ipynb
```

---

## Principales hallazgos

Después de analizar los datos, estas fueron las cosas que más me llamaron la atención:

- Más del **26% de los clientes** cancela el servicio, lo que es una tasa bastante alta
- Los clientes con **contrato mes a mes** son los que más se van (más del 40% de evasión)
- El **primer año de relación** es el período más crítico: si el cliente llega al segundo año, la probabilidad de que se vaya baja mucho
- Los clientes con **cargos mensuales altos** tienden a irse más, lo que puede indicar que no perciben valor por lo que pagan
- Tener **soporte técnico o seguridad online** está asociado a menor evasión

---

## Fuente de los datos

Los datos vienen de la API del challenge oficial de Alura LATAM:  
https://raw.githubusercontent.com/ingridcristh/challenge2-data-science-LATAM/main/TelecomX_Data.json

---

Proyecto desarrollado como parte del programa ONE — Oracle Next Education + Alura LATAM.
