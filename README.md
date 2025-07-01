# Analisis_Sentimiento_IMDB_ModeloF1

🧭 1. Definición del problema
Objetivo: Construir un modelo que clasifique reseñas de películas como positivas o negativas.

Métrica clave: F1-score ≥ 0.85.

Tipo de problema: Clasificación binaria de texto.

📥 2. Carga y exploración inicial de datos
Tareas:

Cargar el dataset proporcionado.

Verificar estructura, tipos de datos, valores nulos o duplicados.

Revisar ejemplos de reseñas y distribución de clases.

Herramientas: pandas, matplotlib, seaborn.

📊 3. Análisis exploratorio de datos (EDA)
Tareas:

Visualizar la distribución de clases (positivas vs. negativas).

Analizar longitud promedio de reseñas, frecuencia de palabras, etc.

Concluir si existe desequilibrio de clases.

Herramientas: seaborn, nltk, wordcloud.

🧹 4. Preprocesamiento de texto
Tareas:

Limpiar texto: minúsculas, eliminación de signos, stopwords, etc.

Tokenización y lematización (si no se usa BERT).

Convertir texto a vectores:

Opción 1: TF-IDF

Opción 2: Word embeddings (Word2Vec, GloVe)

Opción 3: BERT embeddings (BERT_text_to_embeddings())

Herramientas: scikit-learn, nltk, transformers, spaCy.

🤖 5. Entrenamiento de modelos
Tareas:

Dividir datos en entrenamiento y prueba.

Entrenar al menos tres modelos:

LogisticRegression

GradientBoostingClassifier o XGBoost

RandomForestClassifier o SVM

Evaluar con evaluate_model() y comparar F1-score y AUC-ROC.

Herramientas: scikit-learn, xgboost, lightgbm.

🧪 6. Prueba con reseñas personalizadas
Tareas:

Escribir reseñas positivas y negativas.

Clasificarlas con los tres modelos entrenados.

Comparar predicciones y justificar diferencias (por ejemplo, sensibilidad al vocabulario o longitud del texto).

📌 7. Análisis comparativo y hallazgos
Tareas:

Comparar métricas de los modelos (F1, AUC, precisión, recall).

Analizar errores comunes (falsos positivos/negativos).

Justificar por qué un modelo supera a los demás.

Evaluar si se cumple el umbral de F1 ≥ 0.85.
