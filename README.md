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
>Objetivos y requisitos del proyecto
Entender la necesidad de detectar piletas en imágenes satelitales, y cómo esto puede ayudar a reducir la evasión fiscal y aumentar la equidad tributaria.


>💾 Mediante el framework Raster Vision se propone realizar el procedimiento completo de aprendizaje profundo geoespacial:
Leer datos georreferenciados
Entrenar modelos
Realizar predicciones
Escribir predicciones en formatos georreferenciados.

Se propone desarrollar un sistema automatizado:

El objetivo es desarrollar un sistema automatizado que pueda identificar piscinas en imágenes satelitales de alta resolución. Este sistema podría ser de gran utilidad para entidades recaudadoras de impuestos, ya que permitiría identificar propiedades con piscinas que no están declaradas, lo que podría ayudar a reducir la evasión fiscal y aumentar la equidad tributaria.

Además, este sistema también podría ayudar a optimizar los recursos utilizados en la fiscalización, ya que permitiría identificar las propiedades que deben ser inspeccionadas de manera más eficiente.

💻 Se propone desarrollar un sistema automatizado que use:
✅ Imágenes satelitales de alta resolución para identificar posibles piletas

✅ Algoritmos de aprendizaje profundo, entrenados para reconocer formas y reflejos de agua en las imágenes.


Identificación de las partes interesadas y sus necesidades.

Partes interesadas:

Entidades recaudadoras: Buscan utilizar el sistema para reducir la evasión fiscal, aumentar la equidad tributaria y optimizar recursos en la fiscalización.
Equipo de desarrollo del proyecto: Incluye a Romina Yael Hanun, Federico Juchniewicz, Samuel Kanneman, Carla Lucero, Leonardo Matías Mansilla y Román Zelarayán, quienes están a cargo de desarrollar y entrenar el modelo de deep learning.
Usuarios finales: Podrían ser analistas urbanos o autoridades municipales interesadas en la gestión y planificación urbana.
Necesidades:

Automatización y precisión: Desarrollar un sistema automatizado que utilice imágenes satelitales de alta resolución y algoritmos de aprendizaje profundo para identificar piletas con precisión.
Procesamiento de datos geoespaciales: Implementar un procedimiento completo de aprendizaje profundo geoespacial que incluya la lectura de datos georreferenciados, entrenamiento de modelos, realización de predicciones y escritura de predicciones en formatos georreferenciados.
Acceso y manejo de datos: Utilizar herramientas como Raster Vision y GDAL para manejar datos raster y vectoriales, y asegurar el acceso a datos almacenados en AWS S3 sin necesidad de autenticación.
Visualización y evaluación: Capacidad para visualizar los resultados de la segmentación semántica y evaluar la precisión del modelo.
📈 Este sistema podría implementarse por entidades recaudadoras para:
Reducir la evasión fiscal
Aumentar la equidad tributaria
Optimizar recursos en la fiscalización.

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

:bookmark_tabs: Definimos la configuracion para la clasificación y el preprocesamineto de las imágenes , especificamente para segmentación y clasificación que incluyen "pileta" (piscina) y "background" (fondo).

:bookmark_tabs: Definimos el tamaño en pixeles de los recortes cuadrados que se van a usar para entrenar el modelo y una serie de trasformaciones que ayudan a mejorar la robustez y generalización del modelo entrenandolo con variaciones de las imágenes originales.

## 4. Modelado
   >Selección y aplicación varias técnicas de modelado

## 5. Evaluación
   >Evaluación del modelo y revisión de los pasos ejecutados

## 6. Despliegue
    >Generar un informe o implementar un proceso

    
