# Predicción de Abandono Corporativo (Employee Churn Prediction)

Este proyecto tiene como objetivo predecir la probabilidad de que un empleado abandone la empresa utilizando técnicas de Machine Learning. Se desarrolla un flujo completo desde la exploración de datos hasta la selección del modelo óptimo.

## Contenido

- [Descripción del Proyecto](#descripción-del-proyecto)  
- [Datos](#datos)  
- [Flujo del Proyecto](#flujo-del-proyecto)  
- [Preprocesamiento](#preprocesamiento)  
- [Modelos Entrenados](#modelos-entrenados)  
- [Evaluación y Selección de Modelo](#evaluación-y-selección-de-modelo)  
- [Resultados](#resultados)  
- [Requirements](#requisitos)  
- [Autor](#autor)  

---

## Descripción del Proyecto

El abandono corporativo (employee churn) representa un costo importante para las empresas, tanto financiero como operativo. Predecir qué empleados tienen mayor riesgo de abandonar permite implementar estrategias de retención más efectivas. Este proyecto aplica técnicas de Machine Learning para construir un modelo predictivo confiable que ayude a la toma de decisiones en recursos humanos.

---

## Datos

El dataset utilizado contiene información histórica de empleados, incluyendo:

- Datos demográficos: edad, género, estado civil, etc.  
- Datos laborales: departamento, antigüedad, salario, nivel jerárquico, etc.  
- Métricas de desempeño: evaluaciones, productividad, etc.
- Satisfacción laboral: nivel de satisfacción, balance trabajo-vida personal, etc.
- Trayectoria laboral: años en actividad, años desde última promoción, etc.
- Información de abandono: columna target indicando si el empleado dejó la empresa o no.

---

## Flujo del Proyecto

El proyecto se desarrolló siguiendo los pasos típicos de un pipeline de Machine Learning:

1. **Análisis de estructura de datos**  
   - Inspección inicial de las variables y tipos de datos.  
   - Identificación de valores faltantes, outliers y distribuciones.  
   - Visualización exploratoria para detectar patrones.

2. **Preprocesamiento de datos**  
   - Imputación de valores faltantes.  
   - Codificación de variables categóricas (One-Hot / Label Encoding).  
   - Escalado de variables numéricas.  
   - Balanceo de clases usando técnicas como SMOTE.  

3. **Entrenamiento de modelos**  
   - División de los datos en conjunto de entrenamiento y test.  
   - Entrenamiento de varios algoritmos de clasificación, incluyendo:  
     - Regresión Logística
     - Decision Tree
     - K-Nearest Neighbours (KNN)
     - Multilayer Perceptron (MLP)
     - Random Forest  
     - Gradient Boosting 
     - Support Vector Classifier (SVC)
     - Linear Discriminant Analysis (LDA)  
   - Ajuste de hiperparámetros mediante GridSearchCV.

4. **Evaluación de modelos**  
   - Métricas utilizadas: Accuracy, Precision, Recall, F1-score, ROC-AUC.  
   - Validación cruzada para garantizar estabilidad del modelo.  

5. **Selección del modelo óptimo**  
   - Comparación de métricas entre todos los modelos.  
   - Selección del modelo con mejor desempeño general y balance entre Balanced Accuracy, Precision y Recall.  
   - Guardado del modelo final para futuras predicciones utilizando pickle.

---

## Resultados

- El modelo predice correctamente el abandono corporativo en aproximadamente un **94.31% de los casos**.  
- Permite identificar empleados con alto riesgo de abandono y planificar intervenciones preventivas.

---

## Requirements
```bash
pip install -r requirements.txt
```
--- 

## Autor

- **Joaquín Loaces**
- LinkedIn: https://www.linkedin.com/in/joaqu%C3%ADn-loaces-5201271aa/
