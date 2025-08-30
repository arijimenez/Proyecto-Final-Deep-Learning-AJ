# Proyecto-Final-Deep-Learning-AJ
El objetivo del estudio fue aplicar transfer learning para resolver un problema de clasificación de imágenes. Se eligió la ruta de clasificación con modelos preentrenados y se compararon tres arquitecturas: ResNet50, MobileNetV2 y Efficient- NetB0. 
# 📂 Clasificación de Imágenes con Deep Learning

## 📌 Descripción del Proyecto
Este proyecto tiene como objetivo desarrollar y evaluar diferentes arquitecturas de **redes neuronales convolucionales (CNNs)** para la **clasificación de imágenes**.  
Se trabajó con un dataset balanceado que fue dividido en **conjuntos de entrenamiento y validación**, con el fin de comparar el rendimiento de tres modelos populares de deep learning.

## 🧠 Modelos Evaluados
- **ResNet50**: Red profunda con conexiones residuales que permiten un mejor flujo de gradientes.  
- **MobileNetV2**: Arquitectura ligera optimizada para dispositivos móviles y entornos con recursos limitados.  
- **EfficientNetB0**: Modelo que escala de forma compuesta (profundidad, anchura y resolución) para lograr eficiencia y precisión.

## ⚙️ Metodología
1. Preprocesamiento de imágenes (redimensionamiento y normalización).  
2. Transfer learning con pesos preentrenados en ImageNet.  
3. Fine-tuning de las capas superiores.  
4. Evaluación con métricas de clasificación: **Accuracy, Precision (macro), Recall (macro) y F1-score (macro)**.  

## 📊 Resultados Comparativos

| Modelo        | Accuracy | Precision (macro) | Recall (macro) | F1 (macro) |
|---------------|----------|-------------------|----------------|------------|
| ResNet50      | 0.8591   | 0.8610            | 0.8620         | 0.8585     |
| MobileNetV2   | 0.5841   | 0.5974            | 0.5872         | 0.5836     |
| **EfficientNetB0** | **0.9015** | **0.9017**       | **0.9026**      | **0.9016** |

## 🔎 Análisis
- **EfficientNetB0** obtuvo el mejor rendimiento en todas las métricas, alcanzando un **90.15% de accuracy**. Su diseño eficiente y balanceado le permite extraer características de forma más precisa sin aumentar demasiado el costo computacional.  
- **ResNet50** mostró un desempeño sólido (**85.91% accuracy**), gracias a sus conexiones residuales que ayudan a evitar el problema del gradiente desapareciente. Es un buen compromiso entre precisión y complejidad.  
- **MobileNetV2** fue el modelo con menor desempeño (**58.41% accuracy**). Aunque está diseñado para ser rápido y ligero en dispositivos móviles, sacrifica capacidad de representación, lo que afectó sus resultados en este dataset.  

## ✅ Conclusión
- El **mejor modelo para este dataset es EfficientNetB0**, ya que combina eficiencia y alta precisión.  
- **ResNet50** es una alternativa recomendable si se cuenta con más recursos computacionales.  
- **MobileNetV2** es útil únicamente en escenarios donde la prioridad es la **baja demanda de recursos**, sacrificando exactitud en la clasificación.  

---
