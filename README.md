## Proyecto: Detectando Críticas Negativas en Reseñas de Películas 🎬

### Descripción del Proyecto
Film Junky Union busca automatizar la clasificación de reseñas de películas como positivas o negativas, utilizando datos de IMDB. El objetivo principal era entrenar un modelo que alcanzara un **F1-score de al menos 0.85**, logrando identificar críticas negativas con alta precisión.

---

### Metodología
1. **Exploración y Análisis de Datos (EDA):**
   - Análisis de tendencias en la cantidad de reseñas por año.
   - Evaluación de distribuciones de polaridades (positivas/negativas) y puntuaciones.

2. **Modelos Implementados:**
   - **Modelo Constante (DummyClassifier):** Usado como línea base.
   - **TF-IDF con NLTK y Regresión Logística:** Enfoque básico de vectorización.
   - **TF-IDF con spaCy y LightGBM:** Adición de lematización para mejorar las características textuales.
   - **Modelo basado en BERT:** Uso de embeddings contextuales para capturar semántica compleja.

3. **Evaluación:**
   - Métricas: **F1-score**, **ROC AUC**, **APS**.
   - Visualización de curvas ROC y PRC para comparar el desempeño de los modelos.

---

### Resultados Clave
- **Modelo Constante:** F1-score de **0.0** (línea base sin capacidad predictiva).
- **TF-IDF + Regresión Logística:** 
  - **F1-score:** **0.88**
  - **ROC AUC:** **0.95**
  - Excelente balance entre precisión y simplicidad.
- **TF-IDF + LightGBM:** F1-score de **0.86**, buen desempeño, aunque ligeramente inferior.
- **BERT:** F1-score de **0.86**, destacando en textos complejos pero con alto costo computacional.

---

### Conclusiones
- **Eficiencia:** Los modelos basados en TF-IDF y Regresión Logística lograron un rendimiento competitivo con menor complejidad computacional.
- **Cumplimiento del Objetivo:** Se superó el umbral de **F1-score ≥ 0.85**, asegurando un alto nivel de precisión en la detección de reseñas negativas.
- **Consideraciones:** Aunque BERT capturó relaciones semánticas avanzadas, su uso práctico puede ser limitado debido a su elevado tiempo de procesamiento.

---

### Tecnologías Utilizadas
- **Procesamiento de Lenguaje Natural (NLP):** TF-IDF, spaCy, BERT.
- **Modelos de Machine Learning:** Regresión Logística, LightGBM.
- **Visualización:** Matplotlib, Seaborn.
- **Métricas:** F1-score, ROC AUC, APS.

---

### Repositorio
Encuentra el código completo y el análisis detallado en mi [perfil de GitHub](#).  
Descubre cómo el análisis de datos puede transformar la industria del entretenimiento. 🚀
