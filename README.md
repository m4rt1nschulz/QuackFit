# QuackFit
QuackFit es un programa para realizar análisis de poses en actividades deportivas a partir de imágenes o para detección en tiempo real.

# Principales librerías
Se usó YOLOv8 de Ultralytics con su modelo "yolov8n-pose.pt" para realizar la detección de poses y redes neuronales convolucionales de MobileNet en la librería timm (Pytorch Image Models) para el entrenamiento, partiendo del modelo "timm/mobilenetv3_large_100.ra_in1k". También se usaron otras librerías básicas para el manejo de imágenes y datos, estas fueron PIL, numpy, os y shutil.

# Requerimientos 
Para entrenar el modelo con otra base de datos y para su correcto uso en el análisis de pose, se requiere el uso de una GPU, la cuál puede venir de Google Colab o si se quiere correr localmente, de un dispositivo que tenga unidad de procesamiento gráfico disponible. 

# Modo de uso
Se debe correr el Jupyter Notebook llamado "Análisis de Pose en Actividades Deportivas.ipynb" y tras correr "Importación de Datos e Instalación de Librerías" ir directo a "Uso del Modelo para la detección de poses", correr estas 2 celdas y utilizar la función "pose_detect(path)" que recibe la ruta de la imagen a detectar para su análisis, donde retorna el ejercicio que fue detectado junto a la probabilidad de que el modelo esté en lo correcto.

# Video con demostración
En el siguiente link hay un pequeño video sobre este proyecto: https://drive.google.com/file/d/1vbQbPcqZ49DwDF52qtwG9I_lp0Km7Yvj/view?usp=sharing
