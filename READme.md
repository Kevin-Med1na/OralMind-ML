# OralMind-ML: Clasificación de Enfermedades Bucales con InceptionV3  

## Descripción  
**OralMind-ML** es un modelo de machine learning basado en la arquitectura InceptionV3, entrenado para clasificar imágenes de enfermedades bucales en seis categorías:  
1. **Úlceras Bucales**  
2. **Hipodoncia**  
3. **Cálculo Dental**  
4. **Gingivitis**  
5. **Caries**  
6. **Decoloración Dental**  

El modelo está diseñado para asistir en diagnósticos preliminares, mejorando la accesibilidad en salud bucal.  

## Características  
- **Arquitectura**: InceptionV3 con capas personalizadas para clasificación.  
- **Dataset**: Imágenes organizadas en 6 clases, montadas desde Google Drive.  
- **Precisión**: Validación con ~95% de accuracy (ajustable con más épocas).  
- **Técnicas**: Aumento de datos y fine-tuning para evitar overfitting.  

## Dataset  
El dataset contiene imágenes etiquetadas de las seis enfermedades bucales, divididas en:  
- **Train**: 11,683 imágenes  
- **Validation**: 1,410 imágenes  
- **Test**: 1,410 imágenes  

## Instalación  
1. Clona el repositorio:  
   ```bash  
   git clone https://github.com/tu-usuario/OralMind-ML.git  
   ```  
2. Instala dependencias:  
   ```bash  
   pip install tensorflow matplotlib  
   ```  
3. Descarga el [dataset](https://drive.google.com/drive/folders/1wn_2yPfMXkDX-rvxFwQxuEGLBqnLPMN4?usp=sharing) en Google Drive y ajusta las rutas en el código.  

## Entrenamiento  
Ejecuta el Jupyter Notebook `oral_diseases_training.ipynb` para:  
- Cargar el dataset desde Drive.  
- Entrenar el modelo con early stopping y ajuste de tasa de aprendizaje.  
- Guardar el modelo final (`oral-diseases-model-inceptionv3.keras`).  

## Resultados  
- **Accuracy en validación**: ~95% (mejorable con más datos o épocas).  
- **Pérdida**:  
  ![Accuracy Plot](https://github.com/Kevin-Medina/OralMind-ML/blob/main/training_and_validation_accuracy_plot.png)  

## Licencia  
[MIT](https://opensource.org/licenses/MIT)  
