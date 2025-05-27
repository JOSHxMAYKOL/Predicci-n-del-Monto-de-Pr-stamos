# Predicción del Monto de Préstamos Digitales con Python y Redes Neuronales

## Objetivo General
Aplicar técnicas de regresión lineal simple y redes neuronales artificiales para predecir el monto de préstamos digitales de clientes peruanos, utilizando variables disponibles en el dataset y herramientas como Python, TensorFlow/Keras y GitHub.

---

## Objetivos Específicos
- Implementar un modelo de regresión lineal simple para predecir montos de préstamo.  
- Desarrollar una red neuronal basada en múltiples variables para mejorar la predicción.  
- Manipular datos con Pandas y NumPy para limpieza y transformación.  
- Visualizar resultados con Matplotlib y Seaborn para un análisis exploratorio profundo.  
- Aplicar estructuras de programación en Python (bucles, condiciones, listas y diccionarios) para análisis y visualización.  
- Usar GitHub como sistema de control de versiones para gestionar el proyecto.

---

## Descripción del Dataset
El dataset contiene información de clientes de préstamos digitales en Perú, con variables como:  
- `cliente`: Identificador único del cliente.  
- `mes`: Periodo de la transacción (formato YYYYMM).  
- `operDigital`: Tipo de operación digital realizada.  
- `trxDigitalUm`: Número de transacciones digitales.  
- `ventaPrestDig`: Monto del préstamo digital otorgado (variable objetivo).  
- `procedencia`: Lugar o región del cliente.  
- Otras variables relacionadas con comportamiento financiero y bancario.

---

## Explicación de los Modelos

### Regresión Lineal Simple
Se seleccionó la variable `trxDigitalUm` (número de transacciones digitales) como variable independiente, ya que refleja la actividad financiera digital del cliente, lo que influye en la cantidad solicitada o aprobada en el préstamo. El modelo ajusta una línea que intenta predecir el monto del préstamo en función de esta variable.

**Métricas de evaluación:**  
- MAE (Error Absoluto Medio) indica el error promedio en la unidad monetaria.  
- MSE (Error Cuadrático Medio) penaliza errores grandes.  
- R2 indica la proporción de varianza explicada por el modelo.

### Red Neuronal
Para capturar relaciones más complejas, se desarrolló una red neuronal con dos capas ocultas que toma como entrada variables codificadas categóricas (`operDigital`, `procedencia`) junto con la variable numérica `trxDigitalUm`. Esto permite mejorar la precisión de predicción mediante el aprendizaje no lineal.

**Métricas y visualización:**  
Se evaluó el desempeño mediante MAE, MSE y R2 sobre datos de prueba, además de analizar la evolución de la pérdida y error durante el entrenamiento.

---

## Resultados y Visualizaciones

- La regresión lineal simple muestra una tendencia positiva entre el número de transacciones digitales y el monto del préstamo, aunque con limitaciones para captar relaciones complejas.  
- La red neuronal mejora notablemente la precisión, reflejado en mejores métricas y gráficos que muestran buena concordancia entre valores predichos y reales.  
- Los análisis de residuos en ambos modelos muestran errores distribuidos sin sesgos evidentes, confirmando la validez de los modelos.

Además, se realizaron visualizaciones detalladas del dataset para comprender la distribución de variables, correlaciones y frecuencia de operaciones digitales.

---

## Uso de Estructuras de Programación

Se implementaron bucles para contar frecuencias de registros por tipo de operación digital, utilizando listas y diccionarios, y se visualizaron estos conteos mediante gráficos de barras, facilitando el análisis exploratorio.

---

## Librerías Utilizadas

- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- tensorflow / keras  

---

## Conclusiones

- La variable `trxDigitalUm` es un buen predictor simple del monto del préstamo, reflejando la relación directa entre actividad digital y volumen de préstamo.  
- Las redes neuronales permiten capturar patrones complejos y mejoran la precisión de las predicciones.  
- La limpieza, codificación y análisis exploratorio son pasos fundamentales para obtener modelos robustos.  
- La combinación de métodos clásicos y aprendizaje automático es eficaz para problemas financieros como la predicción de préstamos digitales.

---

## Recomendaciones

- Explorar variables adicionales y técnicas de ingeniería de características para mejorar modelos.  
- Considerar modelos más avanzados (boosting, random forest) para comparación.  
- Evaluar modelos con diferentes métricas y validación cruzada para mayor confiabilidad.

---

## Enlace al repositorio GitHub

*(Aquí colocarás el enlace a tu repositorio una vez creado)*

---

## Archivos entregables

- Código fuente en formato `.ipynb` o `.py`.  
- README.md con toda la información.  
- Gráficos exportados o integrados en el notebook.  

---

*Fin del documento*
