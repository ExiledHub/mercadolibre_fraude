# Mercado Libre - Modelo de Fraude
![Python Version](https://img.shields.io/badge/python-3.10.11-blue.svg) 

## Objetivo del Proyecto 
El objetivo del proyecto es realizar un proceso de analisis y modelado sobre la data de transacciones de fraude de la plataforma de Mercado Libre. El modelo requerido busca maximizar las ganancias de la empresa y minimizando las pérdidas debido a fraudes, garantizando al mismo tiempo una excelente experiencia de usuario. 

## Instalación  
### Configuración del entorno virtual 
Para configurar el entorno virtual y instalar las dependencias, sigue estos pasos: 

```
bash python -m venv .venv 
source .venv/bin/activate # En Windows usa `.venv\Scripts\activate` 
pip install -r requirements.txt 
```  
## Orden de Ejecución 
Para reproducir el análisis y los modelos de Machine Learning, ejecuta los cuadernos Jupyter en el siguiente orden: 
1.  `analisis.ipynb` - Realiza el análisis exploratorio y la preparación de los datos. 
2.  `model_training.ipynb` - Entrena los modelos y evalúa su rendimiento. 

## Reportes Generados 
Dentro de la carpeta `report`, encontrarás los siguientes análisis y reportes: 
-  `anova_report.txt`: Reporte del análisis ANOVA realizado sobre los datos. 
-  `raw_data.html`: Reporte en HTML que contiene la exploración de la data cruda. 
-  `preprocessed_data.html`: Reporte en HTML que muestra la data después de la preprocesamiento. 

## Modelos Desarrollados 
Se han entrenado diversos modelos para la detección de fraude, que se encuentran en la carpeta `models`: 
-  `ann_model.pkl`: Modelo de Red Neuronal Artificial. 
-  `lgbm_model.pkl`: Modelo LightGBM. 
-  `svm_model.pkl`: Modelo de Máquinas de Vectores de Soporte. 
-  `logreg_model.pkl`: Modelo de Regresión Logística. 
-  `random_forest_model.pkl`: Modelo de Random Forest. Además, se han creado dos modelos ensamblados: 
-  `ensemble_model_pres.pkl`: Modelo ensamblado con alta precisión pero menor recall. 
-  `ensemble_model_bal.pkl`: Modelo ensamblado balanceado con buen rendimiento en precisión y recall. 