# Predicción de Abandono de Clientes de Beta Bank

## Resumen del Proyecto
Este proyecto tiene como objetivo predecir el abandono de clientes en Beta Bank, utilizando datos históricos sobre el comportamiento de los clientes y la terminación de contratos. Se ha desarrollado un modelo predictivo para identificar clientes propensos a abandonar el banco, con el fin de implementar estrategias proactivas de retención.

## Objetivos
1. **Desarrollar un modelo predictivo** con un valor F1 mínimo de 0.59.
2. **Evaluar y mejorar** la calidad del modelo utilizando métricas como F1 y AUC-ROC.
3. **Implementar técnicas** para corregir el desequilibrio de clases en los datos.

## Metodología
1. **Preparación y Análisis de Datos:**
   - Descarga y limpieza del conjunto de datos `Churn.csv`.
   - Exploración y preprocesamiento de características relevantes (edad, saldo, número de productos, etc.).

2. **Investigación del Equilibrio de Clases:**
   - Entrenamiento inicial del modelo sin corrección del desequilibrio.
   - Evaluación del rendimiento y descubrimiento de desequilibrios en las clases.

3. **Mejora del Modelo:**
   - Implementación de técnicas de sobremuestreo y balanceo de clases.
   - Ajuste de hiperparámetros para optimizar el modelo.
   - Comparación de diferentes enfoques y selección del modelo más efectivo.

4. **Evaluación Final:**
   - Prueba del modelo en un conjunto de datos separado.
   - Evaluación de las métricas F1 y AUC-ROC.
   - Documentación y presentación de los hallazgos.

## Resultados Esperados
- **Predicción precisa del abandono de clientes** con un valor F1 superior a 0.59.
- **Implementación de estrategias de retención** basadas en las predicciones del modelo.
- **Informe detallado y documentación** del proceso, hallazgos y mejoras realizadas.

