# 🧠 Skin Cancer Detection - Deep Learning Model (ISIC 2020)

Este proyecto implementa un modelo de Deep Learning para **clasificar imágenes de lesiones en la piel como benignas o malignas**, utilizando el conjunto de datos **ISIC 2020**. Está desarrollado en **Python con TensorFlow** y estructurado para facilitar el entrenamiento local y la experimentación.

---

## 📁 Estructura del proyecto

```
ModeloDeepLearning/
│
├── data/                    # Contiene las imágenes y el archivo CSV con etiquetas
│   ├── images/              # Todas las imágenes .jpg del dataset
│   └── labels.csv           # CSV con nombre de imagen y etiqueta (malignancy)
│
├── models/
│   └── skin_cancer_model.py # Definición del modelo CNN
│
├── utils/
│   └── preprocessing.py     # Funciones de carga y preprocesamiento de datos
│
├── main.py                  # Script principal para entrenamiento y evaluación
└── requirements.txt         # Dependencias del entorno
```

---

## 🚀 ¿Qué hace esta app?

- Carga imágenes dermatológicas del dataset ISIC 2020.
- Usa un modelo CNN (a definir) para clasificar lesiones como benignas o malignas.
- Entrena y evalúa el modelo con métricas de precisión.
- Es totalmente ejecutable de forma **local** en PyCharm o con cualquier editor compatible.

> **Nota**: Aún se encuentra en fase de desarrollo. El modelo, la arquitectura y estrategias de entrenamiento pueden variar.

---

## ⚙️ Requisitos

- Python 3.10
- pip actualizado
- PyCharm (opcional, recomendado)

---

## 📦 Instalación local

### 1. Clona el repositorio

```bash
git clone https://github.com/tuusuario/ModeloDeepLearning.git
cd ModeloDeepLearning
```

### 2. Crea un entorno virtual

```bash
python -m venv venv
```

### 3. Activa el entorno virtual

- En Windows:
  ```bash
  venv\Scripts\activate
  ```
- En macOS/Linux:
  ```bash
  source venv/bin/activate
  ```

### 4. Instala las dependencias

```bash
pip install -r requirements.txt
```

---

## 📥 Dataset

- Descarga el dataset desde [dataset](https://challenge2020.isic-archive.com/)
- Coloca las imágenes en la carpeta `data/images/`.
- Asegúrate de que el archivo `labels.csv` esté en `data/` y tenga columnas como:

```csv
image_name,malignancy
ISIC_123.jpg,1
ISIC_456.jpg,0
```

---

## ▶️ Ejecución del entrenamiento

Una vez preparado el dataset:

```bash
python main.py
```

---

## 📈 Resultados

El script imprimirá la precisión del modelo sobre el conjunto de prueba. Se pueden añadir mejoras como:

- Aumento de datos (data augmentation)
- Callbacks (EarlyStopping, ModelCheckpoint)
- Visualización con TensorBoard

---

## ✅ Estado del proyecto

🔧 En desarrollo.  
📌 En la siguiente fase se implementarán mejores arquitecturas CNN y se compararán estrategias de entrenamiento.

---

## 📄 Licencia

Este proyecto es libre para fines educativos y experimentales.

---

## 🙋‍♂️ Autor

**Anyelo Nuñez Obispo**  
Estudiante de Ingeniería de Sistemas  
Universidad César Vallejo
