# 🛡️ Proyecto ML Seguridad: Detección de Ataques SQLi y XSS con Transformers

Este proyecto implementa un sistema de seguridad basado en Inteligencia Artificial para detectar ataques de **Inyección SQL (SQLi)** y **Scripting en Sitios Cruzados (XSS)** utilizando modelos de Machine Learning con arquitectura de **Transformers**.

El objetivo es clasificar peticiones web y payloads sospechosos en tiempo real para mitigar vulnerabilidades críticas de OWASP.

## 🚀 Características
* **Detección Avanzada**: Identificación de patrones complejos de SQL Injection y XSS que evaden los sistemas tradicionales basados en firmas.
* **Procesamiento de Lenguaje Natural**: Uso de mecanismos de atención (Transformers) para entender el contexto y la semántica de las consultas Web/API.
* **Entrenamiento Flexible**: Notebooks optimizados listos para ejecutarse en entornos como Google Colab.

## 🛠️ Tecnologías Utilizadas
* **Lenguaje**: Python 3
* **Entorno de Desarrollo**: Google Colab / Jupyter Notebooks
* **Frameworks de ML**: PyTorch / TensorFlow / Hugging Face Transformers
* **Librerías Clave**: Pandas, NumPy, Scikit-learn, Tokenizers

## 📦 Estructura del Repositorio
* `TRAIN_MODEL_SQL_Injection.ipynb`: Cuaderno principal enfocado en el preprocesamiento de datos, tokenización y entrenamiento del modelo Transformer para la detección de SQLi.
* `README.md`: Documentación del proyecto.

## 💻 Configuración y Uso

### Ejecución en Google Colab
1. Sube el archivo `.ipynb` de entrenamiento a tu cuenta de **Google Drive**.
2. Abre el archivo utilizando **Google Colab**.
3. Asegúrate de activar el entorno de ejecución con **GPU** (`Entorno de ejecución` > `Cambiar tipo de entorno de ejecución` > `T4 GPU`) para acelerar el entrenamiento del Transformer.
4. Ejecuta las celdas secuencialmente para procesar el dataset y entrenar el modelo.

### Ejecución Local
Si prefieres correrlo en tu máquina local, clona el repositorio e instala las dependencias:

```bash
git clone https://github.com
cd Proyecto_ML_Seguridad
pip install -r requirements.txt  # Asegúrate de listar tus dependencias aquí
```

## 📊 Dataset
El modelo se entrena utilizando datasets públicos y sintéticos que contienen:
* Payloads legítimos (peticiones HTTP benignas, consultas SQL estándar).
* Payloads maliciosos (intentos de bypass, strings de XSS y sentencias SQL inyectadas).

## 📄 Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

## ✒️ Autor
* **Henrixfs** - *Desarrollo Inicial* - [GitHub Profile](https://github.com)
