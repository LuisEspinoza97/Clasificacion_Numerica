# Clasificacion_Numerica

Este código fue escrito en Google Colab, un entorno de Python en línea que permite crear, ejecutar y compartir notebooks de forma gratuita. Para usar este código, deberás abrir un nuevo notebook en Google Colab y copiar el código en él.

Este código es una implementación de una red neuronal convolucional capaz de clasificar imágenes del conjunto de datos MNIST. Para usarlo, primero debes importar las librerías necesarias, cargar el conjunto de datos MNIST utilizando Keras y definir la arquitectura de la red neuronal.

Luego, debes procesar los datos en el conjunto de entrenamiento y de prueba y entrenar el modelo utilizando el método fit. Una vez entrenado el modelo, se puede evaluar con los datos de prueba utilizando el método evaluate.

Además, el código proporciona una funcionalidad adicional que permite cargar imágenes en el modelo para realizar predicciones y mostrar las 3 mejores opciones con su respectiva probabilidad.

# Descricion de codigo

Importación de librerías: En esta sección se importan las librerías necesarias para trabajar con matrices, construir redes neuronales y visualizar los datos. Se utilizan las librerías numpy, keras, matplotlib, y PIL.

Importación de datos: Aquí se importan los datos que se utilizarán para entrenar el modelo. Se utiliza el dataset MNIST, que es un conjunto de imágenes de dígitos escritos a mano y sus correspondientes etiquetas.

Arquitectura de la red neuronal: En esta sección se construye la arquitectura de la red neuronal utilizando la librería keras. Se establecen las capas de entrada y salida, el número de neuronas en cada capa y la función de activación que se utilizará.

Procesamiento de datos: En esta sección se procesan los datos de entrenamiento y de prueba para que sean compatibles con la arquitectura de la red neuronal. Se redimensionan las imágenes a un tamaño de 28x28, se normalizan los valores de los píxeles para que estén en el rango [0,1], y se hace una codificación one-hot de las etiquetas.

Entrenamiento del modelo: Aquí se entrena la red neuronal utilizando los datos de entrenamiento. Se utilizan los datos procesados, se establece el número de épocas y el tamaño del lote (batch size) y se ajustan los pesos de la red a medida que se realizan iteraciones.

Evaluación del modelo: En esta sección se evalúa el desempeño del modelo utilizando los datos de prueba. Se calcula la pérdida y la exactitud (accuracy) del modelo en los datos de prueba.

Visualización de los resultados: Se visualizan los resultados del modelo. Se muestra una imagen aleatoria del conjunto de prueba y la etiqueta real correspondiente. Luego se hace una predicción utilizando el modelo y se muestra la etiqueta predicha. También se muestra un gráfico que representa la precisión y la pérdida del modelo durante el entrenamiento.

Subiendo imágenes: En esta sección se carga una imagen desde la máquina del usuario utilizando la librería PIL. Se convierte la imagen a un arreglo de NumPy y se redimensiona a 28x28 píxeles. Se normalizan los valores de los píxeles y se hace una predicción utilizando el modelo entrenado. Finalmente, se muestra la imagen y la etiqueta predicha.

Evaluación del modelo con datos de prueba: En esta sección se realiza una evaluación del modelo utilizando los datos de prueba. Se calcula la pérdida y la exactitud del modelo en los datos de prueba.

Visualización de la precisión y la pérdida durante el entrenamiento: En esta sección se muestra un gráfico que representa la precisión y la pérdida del modelo durante el entrenamiento. Se utiliza la función fit de keras para entrenar el modelo y se establece el conjunto de validación para evaluar el desempeño del modelo durante el entrenamiento.

Guardar modelo, cargar imágenes y dar las 3 mejores opciones: En esta sección se guarda el modelo entrenado utilizando la función save de keras. Luego, se carga el modelo previamente entrenado utilizando la función load_model. Se carga una imagen subida por el usuario y se hace una predicción utilizando el modelo cargado. Finalmente, se muestran las tres etiquetas con mayor probabilidad de acuerdo a la predicción del modelo.
