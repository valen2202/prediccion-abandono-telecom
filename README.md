# Predicción de Abandono de Clientes en Telecomunicaciones

Este proyecto fue desarrollado como parte de la **Diplomatura en Ciencia de Datos (UTN)**.  
El objetivo es analizar datos de clientes de una empresa de telecomunicaciones para **predecir la probabilidad de abandono (churn)** utilizando técnicas de Machine Learning.

---

## Objetivos del Proyecto
- Analizar y comprender patrones de comportamiento de los clientes.
- Detectar variables que influyen en el abandono.
- Entrenar y evaluar modelos predictivos para identificar clientes en riesgo.

---

## Contenido del Repositorio
- **Proyecto empresa telecom.ipynb** → Notebook principal con análisis y modelado.
- **requirements.txt** → Librerías necesarias.
- **/img** → Gráficos y visualizaciones (opcional).
- **/data** → Dataset utilizado (si es público).

---

## Tecnologías y Librerías Utilizadas
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- imbalanced-learn

---

## Flujo de Trabajo
1. **Carga y exploración de datos**
   - Limpieza y tratamiento de valores faltantes.
   - Análisis exploratorio (EDA).
2. **Análisis de variables**
   - Distribuciones.
   - Correlaciones.
   - Selección de variables relevantes.
3. **Preparación de datos**
   - Codificación de variables categóricas.
   - Escalado de variables numéricas.
   - Manejo del desbalance de clases con SMOTE.
4. **Modelado y evaluación**
   - Modelos probados: Regresión Logística, KNN, Naive Bayes.
   - Métricas: AUC, Recall, Precision, F1-score.

---

## Resultados

| Modelo               | AUC   | Recall (Churn) | Precision (Churn) | F1-Score |
|----------------------|-------|----------------|-------------------|----------|
| Regresión Logística  | 0.845 | 0.71           | 0.58              | **0.64** |
| KNN                  | 0.843 | **0.86**       | 0.47              | 0.61     |
| Naive Bayes          | 0.833 | 0.80           | 0.50              | 0.62     |

**Modelo con mejor rendimiento:** Regresión Logística (AUC más alto y buen equilibrio en métricas).  

**Insights relevantes:**
1. El Recall es clave en este problema, ya que es más importante identificar correctamente a los clientes que podrían abandonar.
2. KNN logró el mejor Recall (0.86), pero con menor precisión.
3. La Regresión Logística ofrece un equilibrio entre AUC, Recall y Precision, siendo una buena opción para producción.

---

## Cómo Ejecutar el Proyecto

### 1. Clonar este repositorio
```bash
git clone https://github.com/valen2202/prediccion-abandono-telecom.git
cd prediccion-abandono-telecom



## Cómo usarlo
1. Clonar este repositorio.
2. Instalar las dependencias:
   ```bash
   pip install -r requirements.txt
