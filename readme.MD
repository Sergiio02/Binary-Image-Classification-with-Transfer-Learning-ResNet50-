<img src="https://algoritmia8.com/wp-content/uploads/2020/09/11.png" alt="Imagen de Customer Segmentation" width="700"/>

# Binary Image Classification with Transfer Learning (ResNet50)

Este proyecto explora diferentes enfoques para la clasificación binaria de imágenes, en específico, clasificar imágenes según si son perros o gatos, comenzando con un modelo CNN básico y aplicando técnicas como regularización con Dropout y aumento de datos. Finalmente, se incorpora transferencia de aprendizaje con ResNet50, logrando una mejora significativa en precisión y generalización. Se incluyen gráficos de entrenamiento, comparaciones de desempeño y análisis de resultados.


## 📂 Estructura del Proyecto

- `dogOrCatClassification.ipynb` # Notebook con todo el códigodelproyecto
- `README.md` # Documentación del proyecto

## 📥 Requisitos

Este proyecto requiere las siguientes bibliotecas de Python:

- pandas
- numpy
- matplotlib
- scikit-learn
- keras
- tensorflow

## 📊 Resultados

### 🔸 Modelo Base: Arquitectura CNN simple (Conv2D + Dense)

- 🎯 Entrenamiento: ~95%

- 🧪 Validación: ~78%

- ❌ Problema: Alto overfitting

### 🔸 Modelo base + Dropout

- 🎯 Entrenamiento: ~86%

- 🧪 Validación: ~84%

- ✅ Mejor generalización, menos overfitting

### 🔸 Modelo base + Dropout +  Data Augmentation

- 🎯 Entrenamiento: ~79%

- 🧪 Validación: ~78%

- ❌ Generalizan bien pero impreciso

### 🔸 Transfer Learning con ResNet50

- 🎯 Entrenamiento: ~99%

- 🧪 Validación: ~99%

🏆 Mejor modelo, generaliza bien, mucha precisión sin sobreajuste 

### Conclusión Final

La transferencia de aprendizaje con ResNet50 ofreció los mejores resultados, combinando alta precisión y excelente generalización, muy por encima de modelos personalizados con data augmentation y dropout.

## Próximos Pasos

- **Optimización de modelospersonalizados**: Explorar arquitecturas propias variando el número de capas, funciones de activación y técnicas de regularización para mejorar el rendimiento sin usar transfer learning.
- **Despliegue del modelo**: Implementar el modelo final (como el basado en ResNet50) en una aplicación web o servicio para su uso en entornos reales.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar el proyecto, por favor abre un pull request o una issue.
