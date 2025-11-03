# Redes_Neuronales

En este trabajo se documenta el flujo completo de clasificación de dígitos con MNIST. Se organizan las celdas del notebook por punto para mantener trazabilidad y claridad. Se añadieron descripciones en markdown para explicar decisiones y resultados. Se cuidó la coherencia entre el preprocesamiento del entrenamiento, de las pruebas y de las imágenes propias. Finalmente, se validó el desempeño y se dejaron indicaciones para reproducir la predicción en tiempo real.

## Resumen

1. **Entrenamiento y gráficas.**
   Se entrenó un modelo de redes neuronales para clasificar dígitos 0–9 y se graficó el comportamiento del sistema (accuracy y loss) a lo largo del entrenamiento. Se reportó la exactitud en entrenamiento y en validación, destacando la época óptima según los criterios definidos.

2. **Evaluación en prueba y comparación.**
   Se evaluó la exactitud del modelo sobre el conjunto de prueba provisto por MNIST y se comparó contra la exactitud de validación. Se añadió un comentario breve justificando similitudes o diferencias observadas.

3. **Generación y preprocesamiento de 50 imágenes.**
   Se generaron 50 imágenes propias (5 por dígito 0–9). Se preprocesaron para que el modelo pudiera evaluarlas, replicando el pipeline del taller (escala de grises, umbral, inversión y redimensionado a 28×28), y se guardaron para trazabilidad.

4. **Evaluación en imágenes propias y análisis de errores.**
   Se corrió la inferencia sobre las 50 imágenes y se compararon los resultados con los previos. Se comentaron motivos de potencial error (iluminación, trazos delgados/rotos, escala, centrado, ruido) y su impacto en clases específicas.

5. **Tres mejoras o innovaciones.**
   Se implementaron tres cambios en etapas seleccionadas (p. ej., normalización consistente, binarización estricta y ensanchado morfológico del trazo). Se explicó qué se hizo, por qué se hizo y si derivó en mejoras de predicción y/o de usabilidad del sistema.

6. **Predicción en tiempo real.**
   Se integró un sistema de predicción en tiempo real usando la cámara del equipo, aplicando el mismo preprocesamiento y cargando el modelo entrenado. Se verificó la coherencia de dimensiones y escalas requeridas por el modelo.

---

## Documentos
* (Archivo en jupyter)[Tarea_redes_neuronales.ipynb]
* (Archivo en HTML)[Tarea_redes_neuronales.html]
* (Archivo de prediccion en tiempo real)[real_time_prediction.ipynb]
* [Archivo del modelo](my_model_new.h5)
* [Numeros usados como base de datos](https://drive.google.com/drive/u/0/folders/1zxLFp6LuusRxunKrktOS0b9igbphHU93)
