# GRUPO-11

<h1 align="center"> PROYECTO FINAL </h1>
<h1 align="center"> Detección de piletas utilizando imágenes satelitales y Deep Learning </h1>

### COHORTE 2022

### :globe_with_meridians: TECNICATURA EN CIENCIAS DE DATOS E INTELIGENCIA ARTIFICIAL

### *Colaboradores:*

- [Hanun Romina](https://github.com/RomiHanun) 
- [Kanneman Samuel](https://github.com/samuelkanneman)
- [Zelarayán Román ](https://github.com/romanzelararg)
- [Mansilla Leonardo Matias ](https://github.com/LMmansilla)
- [Lucero Carla](https://github.com/CarlaLucerocd)
- [Juchniewicz Federico](https://github.com/FJISPC)

![ImagenSatelital](https://github.com/romanzelararg/GRUPO-11---Proyecto-Final-Cohorte-2022-/blob/main/img_SAS_wgs_r.jpg)

### :pushpin: *El procesamiento de imágenes, combinado con machine learning, ofrece un gran potencial para la ciencia de datos. Un ejemplo de aplicación y uso para la Gestion Urbana es la detección de piletas.*

# :black_nib: *Modelo de Referencia CRISP-DM*
## 1. Comprensión del Negocio
   >Objetivos y requisitos del Proyecto, definición del problema y plan preliminar diseñado.

:paperclip: ***Mediante el framework Raster Vision se propone realizar el procedimiento completo de aprendizaje profundo geoespacial:***
- [x] Leer datos georreferenciados
- [x] Entrenar modelos
- [x] Realizar predicciones
- [x] Escribir predicciones en formatos georreferenciados.

💻 ***Desarrollar un sistema automatizado que use:***

✅ Imágenes satelitales de alta resolución para identificar posibles piletas

✅ Algoritmos de aprendizaje profundo, entrenados para reconocer formas y reflejos de agua en las imágenes.

:space_invader: ***Objetivo del sistema automatizado***

El objetivo es que dicho sistema pueda identificar piscinas en imágenes satelitales de alta resolución. Éste sistema podría ser de gran utilidad para entidades recaudadoras de impuestos, ya que permitiría identificar propiedades con piscinas que no están declaradas, lo que podría ayudar a reducir la evasión fiscal y aumentar la equidad tributaria.

Además, el sistema también podría ayudar a optimizar los recursos utilizados en la fiscalización, ya que permitiría identificar las propiedades que deben ser inspeccionadas de manera más eficiente.


:pencil: ***Identificación de las partes interesadas y sus necesidades***

*Partes interesadas:*

* Entidades recaudadoras: Buscan utilizar el sistema para reducir la evasión fiscal, aumentar la equidad tributaria y optimizar recursos en la fiscalización.

* Equipo de desarrollo del proyecto: Incluye a Romina Yael Hanun, Federico Juchniewicz, Samuel Kanneman, Carla Lucero, Leonardo Matías Mansilla y Román Zelarayán, quienes están a cargo de desarrollar y entrenar el modelo de deep learning.

* Usuarios finales: Podrían ser analistas urbanos o autoridades municipales interesadas en la gestión y planificación urbana.

*Necesidades:*

* Automatización y precisión: Desarrollar un sistema automatizado que utilice imágenes satelitales de alta resolución y algoritmos de aprendizaje profundo para identificar piletas con precisión.
  
* Procesamiento de datos geoespaciales: Implementar un procedimiento completo de aprendizaje profundo geoespacial que incluya la lectura de datos georreferenciados, entrenamiento de modelos, realización de predicciones y escritura de predicciones en formatos georreferenciados.
  
* Acceso y manejo de datos: Utilizar herramientas como Raster Vision y GDAL para manejar datos raster y vectoriales, y asegurar el acceso a datos almacenados en AWS S3 sin necesidad de autenticación.
  
* Visualización y evaluación: Capacidad para visualizar los resultados de la segmentación semántica y evaluar la precisión del modelo.
  

Identificar los posibles beneficios y desafios del proyecto:

El proyecto descrito tiene como objetivo utilizar imágenes satelitales y técnicas de deep learning para detectar piscinas, lo que puede tener varios beneficios y desafíos:

Beneficios:

Automatización en la detección: El uso de algoritmos de aprendizaje profundo puede automatizar y acelerar el proceso de identificación de piscinas en grandes áreas geográficas.
Mejora en la gestión urbana: La detección precisa de piscinas puede ayudar a las entidades recaudadoras a reducir la evasión fiscal y aumentar la equidad tributaria.
Optimización de recursos: El sistema propuesto podría optimizar los recursos utilizados en la fiscalización, haciendo el proceso más eficiente.

Desafíos:

Calidad de los datos: La precisión del modelo depende de la calidad y resolución de las imágenes satelitales, así como de la precisión de las anotaciones utilizadas para el entrenamiento.
Complejidad técnica: Implementar y mantener un sistema de aprendizaje profundo requiere conocimientos especializados y puede ser técnicamente desafiante.
Cambios ambientales: Las condiciones ambientales y cambios estacionales pueden afectar la visibilidad de las piscinas en las imágenes satelitales, lo que podría complicar la detección.

Mediante el framework Raster Vision se propone realizar el procedimiento completo de aprendizaje profundo geoespacial

💾 Mediante el framework Raster Vision se propone realizar el procedimiento completo de aprendizaje profundo geoespacial:
Leer datos georreferenciados
Entrenar modelos
Realizar predicciones
Escribir predicciones en formatos georreferenciados.
    
      
## 2. Comprensión de los Datos
   >Recopilación , primeros conocimientos de los datos

Objetivo: Análisis exploratorio de las imágenes satelitales que tenemos disponibles.
Análisis exploratorio de las imágenes satelitales del área de interés. Implica visualizar las imágenes, entender su resolución y otros metadatos.

Exploración de herramientas de descarga.
Descarga de imágenes satelitales para entrenamiento.
Instalación de librerías de RasterVision
Carga de imágenes satelitales en Drive
Identificar las fuentes de datos y proyecciones
Dataset de evidencia de campo (relevamiento de piscinas) fue obtenido de la página web del gobierno de la Ciudad de Buenos Aires. (https://buenosaires.gob.ar/). El mismo consistió en:

‌

Datos georreferenciados: Estos datos, que pueden incluir información sobre la ubicación de las piscinas, se utilizan para entrenar el modelo y evaluar su rendimiento;
Datos de entrenamiento y validación: Estos son subconjuntos de los datos georreferenciados que se utilizan específicamente para entrenar el modelo y evaluar su rendimiento durante el proceso de entrenamiento.
Es importante mencionar que el cuaderno no especifica exactamente de dónde se obtienen estos datos. Sin embargo, en proyectos similares, las imágenes satelitales a menudo se obtienen de fuentes como Google Earth, Bing Maps, o servicios de imágenes satelitales como Sentinel o Landsat. Los datos georreferenciados pueden provenir de diversas fuentes, incluyendo bases de datos públicas o privadas, o pueden ser recopilados manualmente.


Realizar un análisis exploratorio de los datos.

Se descarga y se guarda un archivo .geojson, que es un formato de archivo abierto para representar datos geoespaciales simples.
Los archivos GeoJSON contienen información geográfica, como puntos, líneas y polígonos, junto con otros datos en formato JSON;
Se configura las clases para la segmentación, se define el tamaño de las ventanas de entrenamiento y establece una serie de transformaciones de aumento de datos para mejorar la robustez del modelo de aprendizaje automático.
Las transformaciones de aumento de datos son técnicas comunes para aumentar artificialmente la diversidad de los datos de entrenamiento sin recopilar nuevos datos, lo que puede mejorar la capacidad del modelo para generalizar a nuevas imágenes.


Identificar las características y la calidad de los datos.

Características y la calidad de los datos:

Características del Proyecto:

Objetivo: Utilizar el procesamiento de imágenes y machine learning para detectar piletas en imágenes satelitales.
Framework Utilizado: Raster Vision, para el proceso completo de aprendizaje profundo geoespacial.
Fuente de Datos: Imágenes satelitales de la página web del gobierno de la Ciudad de Buenos Aires.
Aplicación Propuesta: Implementación por entidades recaudadoras para reducir la evasión fiscal y optimizar recursos.
Calidad y Configuración de Datos:

Dataset: Alta resolución, obtenido de una fuente gubernamental confiable.
Preprocesamiento: Uso de GDAL para leer y escribir datos geoespaciales.
Clases Definidas: Dos clases, 'background' y 'pileta', con sus respectivas transformaciones y visualización.
Calidad del Código:

Estructura: El código está bien organizado, con comentarios explicativos y secciones claramente definidas.
Modelo de Deep Learning: Utiliza un modelo preentrenado de PyTorch con configuraciones específicas para la tarea.
Visualización: Incluye código para visualizar los resultados de la segmentación semántica.
Entrenamiento del Modelo: Configura y entrena el modelo con un conjunto de datos de entrenamiento y validación.
Posibles Mejoras:

Validación de Datos: Asegurarse de que las anotaciones y etiquetas sean precisas.
Optimización de Hiperparámetros: Ajustar los hiperparámetros para mejorar el rendimiento del modelo.
Evaluación Rigurosa: Implementar métricas de evaluación para medir la precisión y el recall del modelo.

Definir las clases para la segmentación

En el contexto de la segmentación semántica en deep learning, las "clases" se refieren a las categorías de objetos que el modelo está diseñado para reconocer en las imágenes. Cada píxel en la imagen se clasifica en una de las clases posibles.

En el colab ISPC_Piletas_Entrenamiento.ipynb`, las clases para la segmentación probablemente serían al menos dos: 'pileta' (piscina) y 'background' (fondo). Esto significa que el modelo está entrenado para reconocer y diferenciar entre estas dos categorías en las imágenes satelitales.

La clase 'pileta' correspondería a los píxeles que representan piscinas en las imágenes.
La clase 'background' correspondería a todos los demás píxeles que no representan piscinas.
Estas clases permiten al modelo aprender a distinguir entre las características visuales de las piscinas y el resto de la imagen. Una vez entrenado, el modelo puede aplicarse a nuevas imágenes para identificar y segmentar las piscinas.

## 3. Preparación de los Datos
   >Seleccion de tablas, registros y atributos, transformación y limpieza de datos.
Preparar los datos para el modelado:
Implica la limpieza de las imágenes, la evaluación del dataset (evaluación visual de correspondencia de las anotaciones), la eliminación de las partes no deseadas y la preparación de las etiquetas para el entrenamiento del modelo.
>
Definición de nuestra área de interés
El Área de Interés (AoI) se refiere a la región geográfica específica que se está analizando o estudiando. En nuestro caso, está relacionada con la detección de piletas (piscinas) utilizando imágenes satelitales y técnicas de aprendizaje profundo.

El AoI se define mediante un archivo GeoJSON, que es un formato de archivo abierto para representar datos geoespaciales simples. Este archivo contiene información geográfica, como puntos, líneas y polígonos, junto con otros datos en formato JSON. En el contexto del aprendizaje automático y el procesamiento de imágenes, el AoI se utiliza para delimitar la región sobre la cual el modelo realizará predicciones o análisis.

En resumen, el AoI es crucial para enfocar el análisis de datos geoespaciales en una región específica y es un componente esencial en proyectos de visión por computadora y teledetección que involucran datos georreferenciados.

Entrenamiento del modelo 'resnet18'

Carga del Modelo Preentrenado:

Se carga un modelo resnet18 preentrenado utilizando torch.hub.
Se configura el modelo para la tarea específica de segmentación semántica con las clases definidas.
Entrenamiento del Modelo:

Se inicia el entrenamiento del modelo con los conjuntos de datos preparados.
Se realizan iteraciones (épocas) donde el modelo aprende a identificar piletas en las imágenes.

Generación de variable
En el caso del colab ISPC_Piletas_Entrenamiento.ipynb` , el código muestra la generación de dos variables:

annotations_url = "https://drive.google.com/file/d/1V9N0xDJKApR_p3PlFZ-9xSvMWWh1Xv3o/view?usp=drive_link"
annotations_file_dest = "/content/drive/MyDrive/Deteccion/anotaciones/anotaciones_wgs_geoj_r2.geojson"

Aquí, annotations_url es una variable que almacena la URL del archivo que se desea descargar desde Google Drive, y annotations_file_dest es una variable que almacena la ruta donde se guardará el archivo descargado.

Preprocesar y Transformar los datos para su uso en el modelo.
Se empezó a trabajar con una imagen que era bastante extensa de aproximadamente 40 manzanas pero se hizo difícil poder entrenar el modelo.
Por lo que reducimos la imagen a 4 manzanas y se logró entrenar correctamente.
Con dicho entrenamiento se obtuvo un modelo y se usos para predecir otro.

## 4. Modelado
   >Selección y aplicación varias técnicas de modelado
>
Objetivo: Generación del modelo deep learning.
Entrenar el modelo de deep learning utilizando el framework Raster Vision. Asegurarse de configurar correctamente los parámetros del modelo y de utilizar una división adecuada de los datos para el entrenamiento y la validación.

Seleccionar el modelo de aprendizaje profundo (ResNet-18).
ResNet-18 es una arquitectura de red neuronal convolucional que ha demostrado ser muy efectiva en tareas de reconocimiento de imágenes. La versión "18" se refiere a la profundidad de la red, es decir, el número de capas que tiene.

Las ResNets son conocidas por su capacidad para entrenar redes muy profundas gracias a sus "conexiones residuales" o "conexiones de salto". Estas conexiones permiten que el gradiente se propague directamente a través de varias capas sin atenuarse, lo que ayuda a mitigar el problema del "gradiente que desaparece", un problema común cuando se entrenan redes neuronales profundas.

En el contexto del colab ISPC_Piletas_Entrenamiento.ipynb, ResNet-18 ha sido seleccionado por varias razones:

Eficiencia: ResNet-18 es relativamente ligero en comparación con otras variantes de ResNet (como ResNet-50, ResNet-101, etc.), lo que lo hace más rápido y eficiente en términos de memoria y tiempo de cálculo.
Rendimiento: A pesar de su simplicidad, ResNet-18 puede ofrecer un rendimiento sólido en muchas tareas de visión por computadora, incluyendo la detección y segmentación de objetos.
Preentrenamiento: ResNet-18 está disponible como un modelo preentrenado en varias bibliotecas de deep learning, lo que permite un inicio rápido y mejora el rendimiento al aprovechar los patrones aprendidos de grandes conjuntos de datos como ImageNet.

Configurar el modelo y los parámetros de entrenamiento.

Selección del Modelo: Se ha seleccionado ResNet-18, que es una arquitectura de red neuronal convolucional conocida por su eficacia en tareas de reconocimiento de imágenes.

Configuración de Parámetros del Modelo: Los parámetros del modelo, como el número de capas y neuronas, así como las funciones de activación, se configuran de acuerdo con las necesidades de la tarea.

Configuración de Parámetros de Entrenamiento: Los parámetros de entrenamiento, como el número de épocas, el tamaño del lote y la tasa de aprendizaje, se establecen. Estos parámetros pueden tener un gran impacto en la eficacia del entrenamiento.

Entrenar el modelo con los datos de entrenamiento.

Entrenamiento del Modelo: El modelo se entrena utilizando los datos de entrenamiento, ajustando los pesos y los parámetros internos de la red para minimizar el error.

. Entrenamiento del Modelo:

Se inicia el entrenamiento del modelo con los conjuntos de datos preparados.
Se realizan iteraciones (epoch) donde el modelo aprende a identificar piletas en las imágenes.

Monitorear el rendimiento del modelo durante el entrenamiento.

Visualización: Se utiliza SemanticSegmentationVisualizer para visualizar las predicciones del modelo y las etiquetas reales, lo que ayuda a monitorear cómo el modelo está aprendiendo.
Registro de Estadísticas: Se registran estadísticas de los datos para asegurarse de que el entrenamiento se base en datos sólidos y bien informados.
Guardado del Modelo: Una vez completado el entrenamiento, se guarda el modelo y su configuración para su uso futuro.


## 5. Evaluación
   >Evaluación del modelo y revisión de los pasos ejecutados

## 6. Despliegue
    >Generar un informe o implementar un proceso

    
