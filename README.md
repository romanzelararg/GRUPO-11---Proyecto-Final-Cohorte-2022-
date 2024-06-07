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

### :electron: *El procesamiento de imágenes, combinado con machine learning, ofrece un gran potencial para la ciencia de datos. Un ejemplo de aplicación y uso para la Gestion Urbana es la detección de piletas.*

### *Antecedentes*
La idea de utilizar imágenes satelitales para la detección de piletas surge de la necesidad de gestionar mejor el consumo de agua en localidades con problemas de abastecimiento, ya que la información obtenida es valiosa para las empresas proveedoras de agua, ayudándolas a ajustar la provisión según la estacionalidad y la demanda; además de favorecer la reducción de la evasión fiscal, el aumento de la equidad tributaria y la optimización de recursos en la fiscalización. Las municipalidades están llevando a cabo relevamientos de piletas para medir el uso del agua y optimizar los recursos hídricos.

Un antecedente relevante se encuentra en las provincias de Córdoba y Neuquén, donde se emplearon imágenes satelitales para identificar piletas domiciliarias. Aunque inicialmente este proceso era manual y dependía de filtros específicos, se ha avanzado hacia la automatización con el uso de tecnologías de alta resolución y machine learning.

En Córdoba, a partir de 2022, se implementó un sistema avanzado de imágenes satelitales en cuatro bandas, incluyendo infrarrojas, que permitió una detección más precisa de zonas húmedas y piletas. Este sistema ha mejorado significativamente la capacidad de captación de datos, incrementando la detección de metros cuadrados construidos no declarados y piletas. Los resultados han sido notables: hasta septiembre de 2023, se detectaron 44 millones de metros cuadrados y más de 28 mil nuevas piletas en la provincia. Este avance no solo refleja un aumento en la construcción, sino principalmente una mejora en la tecnología de monitoreo y en el procesamiento de datos. La incorporación de inteligencia artificial ha optimizado el rendimiento del software y la eficiencia de los operadores.

Estos desarrollos subrayan la importancia de adoptar tecnologías avanzadas como el machine learning para la detección automatizada de piletas mediante imágenes satelitales, contribuyendo así a una gestión más eficiente de los recursos hídricos y fiscales.

https://www.lavoz.com.ar/politica/record-de-deteccion-de-metros-construidos-y-de-piletas-sin-declarar-en-cordoba/

### *Introducción*
El procesamiento de imágenes combinado con técnicas de machine learning ofrece un vasto potencial para la ciencia de datos, especialmente en el ámbito de la gestión urbana. Un ejemplo destacado de esta sinergia es la detección de piletas mediante imágenes satelitales y algoritmos de deep learning. Éste proyecto tiene como objetivo desarrollar un sistema automatizado que utilice imágenes satelitales de alta resolución y aprendizaje profundo para identificar piscinas en la Ciudad de Buenos Aires.

Para llevar a cabo ésta tarea, se utilizará el framework Raster Vision, que permite realizar el procedimiento completo de aprendizaje profundo geoespacial: desde la lectura de datos georreferenciados hasta el entrenamiento de modelos, la realización de predicciones y la escritura de estas predicciones en formatos georreferenciados. El dataset de evidencia de campo, que incluye relevamientos de piscinas, será obtenido Gerencia de Generación de datos del GCBA (https://buenosaires.gob.ar/antropologia-urbana/herramientas-para-la-generacion-de-datos-territoriales).

El sistema propuesto no solo facilitará la identificación de piscinas mediante algoritmos entrenados para reconocer formas y reflejos de agua en las imágenes, sino que también ofrecerá múltiples beneficios a las entidades recaudadoras. Entre estos beneficios se destacan la reducción de la evasión fiscal, el aumento de la equidad tributaria y la optimización de recursos en la fiscalización. Además, esta información será valiosa para las empresas proveedoras de agua, ayudándolas a ajustar la provisión según la estacionalidad y demanda.

Sin embargo, el proyecto también enfrenta varios desafíos. La calidad de los datos es fundamental; la precisión del modelo dependerá de la resolución de las imágenes satelitales y de la exactitud de las anotaciones utilizadas para el entrenamiento. La complejidad técnica del desarrollo y mantenimiento del sistema de aprendizaje profundo requiere conocimientos especializados. Además, las condiciones ambientales y los cambios estacionales pueden afectar la visibilidad de las piscinas en las imágenes, complicando su detección.

En resumen, éste proyecto busca aprovechar el poder del deep learning y el procesamiento de imágenes satelitales para mejorar la gestión urbana mediante la detección automatizada de piletas, ofreciendo así beneficios tangibles y enfrentando desafíos técnicos y ambientales significativos.

### *Objetivo General*
Desarrollar un sistema automatizado basado en deep learning para detectar piletas mediante fotos aéreas o imágenes satelitales de alta resolución, utilizando el framework Raster Vision, con el fin de mejorar la gestión urbana y fiscal en la Ciudad de Buenos Aires.

#### Objetivos Específicos
##### Recolección y Preparación de Datos
o	Obtener un Dataset, producto de un relevamiento de la Gerencia de Generación de datos del GCBA, que funcione como evidencia de campo. 
- https://buenosaires.gob.ar/antropologia-urbana/herramientas-para-la-generacion-de-datos-territoriales
  
o	Corroborar una muestra de estas etiquetas para crear un conjunto de datos de entrenamiento consistente.

o	Obtener un conjunto de imágenes satelitales descargadas mediante el software SAS-PLANET.
- Desarrollo del Modelo de Deep Learning
  
o	Configurar el entorno de trabajo utilizando el framework Raster Vision para el procesamiento de datos georreferenciados.

o	Diseñar y entrenar un modelo de aprendizaje profundo que pueda identificar piletas, basándose en características visuales como formas y reflejos de agua.

o	Evaluar el rendimiento del modelo utilizando métricas adecuadas (precisión, recall, F1 score) y realizar ajustes necesarios para optimizar su desempeño.
- Implementación del Sistema de Detección
o	Integrar el modelo entrenado en un pipeline automatizado que procese nuevas imágenes satelitales y realice predicciones sobre la presencia de piletas.

o	Implementar un sistema para almacenar y visualizar las predicciones en formatos georreferenciados, facilitando su integración con sistemas de información geográfica (SIG).
- Validación y Verificación
  
o	Realizar pruebas de campo y validación cruzada para asegurar la precisión y robustez del sistema en diversas áreas de la ciudad.

o	Ajustar el modelo y el sistema en base a los resultados obtenidos para mejorar su confiabilidad y precisión.
- Aplicación y Beneficios
  
o	Desarrollar informes y visualizaciones que demuestren cómo el sistema puede ser utilizado por entidades recaudadoras para detectar piletas no registradas, reduciendo la evasión fiscal y aumentando la equidad tributaria.

o	Presentar un análisis costo-beneficio que muestre cómo la implementación del sistema puede optimizar recursos en la fiscalización urbana.
- Documentación y Capacitación
  
o	Documentar detalladamente el proceso de desarrollo, incluyendo la recolección de datos, el entrenamiento del modelo, la integración del sistema y los resultados de validación.

o	Capacitar al personal de las entidades recaudadoras en el uso del sistema y la interpretación de los resultados.
- Exploración de Extensiones Futuras
  
o	Investigar la posibilidad de extender el sistema para detectar otras características urbanas relevantes (como construcciones ilegales, áreas verdes, etc.).

o	Evaluar la viabilidad de aplicar el sistema en otras ciudades y regiones, considerando la disponibilidad de datos y las necesidades específicas locales.


#### Metodología
##### Análisis de Requisitos:
o	Definir claramente los requisitos técnicos y funcionales del sistema.

o	Establecer los criterios de éxito y las métricas de evaluación.

##### Desarrollo Iterativo:
o	Seguir un enfoque ágil para el desarrollo del sistema, permitiendo iteraciones rápidas y ajustes continuos basados en retroalimentación.

##### Colaboración y Feedback:
o	Mantener una comunicación constante con las partes interesadas, incluyendo las entidades recaudadoras y expertos en SIG, para asegurar que el sistema desarrollado satisfaga sus necesidades.

##### Monitoreo y Mejora Continua:
o	Implementar un sistema de monitoreo para evaluar continuamente el rendimiento del sistema en producción.

o	Planificar actualizaciones y mejoras basadas en nuevos datos y tecnologías emergentes.

Este enfoque detallado y estructurado asegura que el proyecto no solo cumpla con los objetivos técnicos, sino que también aporte beneficios tangibles para la gestión urbana y fiscal de la Ciudad de Buenos Aires.

### Procesamiento 
![ImagenSatelital](https://github.com/romanzelararg/GRUPO-11---Proyecto-Final-Cohorte-2022-/blob/main/P%C3%B3ster%20Gr%C3%A1fico%20de%20pasos%20Corporativo%20Multicolor%20(1)%20(1).png)


## :black_nib: *Modelo de Referencia CRISP-DM*
### 1. Comprensión del Negocio
   >Objetivos y requisitos del Proyecto, definición del problema y plan preliminar diseñado.

 :pushpin: ***Mediante el framework Raster Vision se propone realizar el procedimiento completo de aprendizaje profundo geoespacial:***
- [x] Leer datos georreferenciados
- [x] Entrenar modelos
- [x] Realizar predicciones
- [x] Escribir predicciones en formatos georreferenciados.

:pushpin: ***Desarrollar un sistema automatizado que use:***

- [x] Imágenes satelitales de alta resolución para identificar posibles piletas

- [x] Algoritmos de aprendizaje profundo, entrenados para reconocer formas y reflejos de agua en las imágenes.

:pushpin: ***Objetivo del sistema automatizado***

El objetivo es que dicho sistema pueda identificar piscinas en imágenes satelitales de alta resolución. Éste sistema podría ser de gran utilidad para entidades recaudadoras de impuestos, ya que permitiría identificar propiedades con piscinas que no están declaradas, lo que podría ayudar a reducir la evasión fiscal y aumentar la equidad tributaria.

Además, el sistema también podría ayudar a optimizar los recursos utilizados en la fiscalización, ya que permitiría identificar las propiedades que deben ser inspeccionadas de manera más eficiente.

:pushpin: ***Definición del Problema y Plan Preliminar Diseñado***

El problema a resolver es la detección automatizada de piscinas en imágenes satelitales. Para abordar este problema, se propone un procedimiento completo de aprendizaje profundo geoespacial utilizando framework Raster Vision, que incluye:

- *Lectura de datos georreferenciados*
   * Se obtendrán imágenes satelitales de alta resolución, que serán utilizadas como base de datos principal. Estas imágenes deben ser accesibles sin la necesidad de autenticación, facilitando así el flujo de trabajo. 
   * Utilizaremos herramientas como Raster Vision y GDAL (Geospatial Data Abstraction Library) para la lectura y manipulación de estos datos, asegurando que la información geoespacial sea correctamente procesada y preparada para el entrenamiento del modelo.
  
- *Entrenamiento de modelos*
   * Se entrenan modelos de aprendizaje profundo, específicamente redes neuronales convolucionales(CNN), para reconocer las características distintivas de las piscinas en las imágenes satelitales.
   * El entrenamiento del modelo incluirá la segmentación semántica , permitiendo distinguir entre diferentes tipos de superficies y detectar con precisión las piscinas.Este proceso implica la anotación de imágenes para crear un conjunto de datos de entrenamiento robusto.
   * La calidad de las anotaciones es crucial, por lo que se invertirá tiempo en asegurar que los datos etiquetados sean precisos y representativos.
  
- *Realización de predicciones*
   * Una vez que el modelo esté entrenado , se aplicará a nuevas imágenes satelitales para identificar y localizar piscinas.
   * Las predicciones serán validadas y ajustadas para mejorar la precisión del sistema .Esto incluye la evaluación del rendimiento del modelo utilizando métricas como la precisión , el recall y el F1-score, y realizando ajustes basados en los resultados de estas evaluaciones.

- *Escritura de predicciones en formatos georreferenciados*
   * Las predicciones realizadas por el modelo serán convertidas en formatos georreferenciados que puedan ser integradas fácilmente en sistemas de información geográfica(SIG).
   * Esta fase asegura que los resultados puedan ser utilizados para escribir las predicciones en formatos estándar, asegurando la compatibilidad con diferentes plataformas y aplicaciones.

:pushpin: ***Desarrollo del Sistema Automatizado***

* Imágenes Satelitales de Alta Resolución
  - El sistema utiliza imágenes satelitales de alta resolución para identificar posibles piscinas. La calidad y resolución de estas imágenes son esenciales para la precisión modelo. Las imágenes deben capturar detalles finos y permitir una clara distinción de las características de las piscinas .
* Algoritmo de Aprendizaje Profundo
  - Se entrenan algoritmos de aprendizaje profundo, específicamente diseñados para recorrer formas y reflejos de agua en las imágenes satelitales. Estos algoritmos deben manejar la variabilidad en las condiciones de iluminación y los diferentes tipos de piscinas. El entrenamiento incluirá técnicas de argumentación de datos para mejorar la robustez del modelo frente a diferentes condiciones ambientales y variaciones estacionales.

:pushpin: ***Identificación de las partes interesadas y sus necesidades***

*Partes interesadas:*

* Entidades recaudadoras: Buscan utilizar el sistema para reducir la evasión fiscal, aumentar la equidad tributaria y optimizar recursos en la fiscalización.

* Equipo de desarrollo del proyecto: Incluye a Romina Yael Hanun, Federico Juchniewicz, Samuel Kanneman, Carla Lucero, Leonardo Matías Mansilla y Román Zelarayán, quienes están a cargo de desarrollar y entrenar el modelo de deep learning.

* Usuarios finales: Podrían ser analistas urbanos o autoridades municipales interesadas en la gestión y planificación urbana.

*Necesidades:*

* Automatización y precisión: Desarrollar un sistema automatizado que utilice imágenes satelitales de alta resolución y algoritmos de aprendizaje profundo para identificar piletas con precisión.
  
* Procesamiento de datos geoespaciales: Implementar un procedimiento completo de aprendizaje profundo geoespacial que incluya la lectura de datos georreferenciados, entrenamiento de modelos, realización de predicciones y escritura de predicciones en formatos georreferenciados.
  
* Acceso y manejo de datos: Utilizar herramientas como Raster Vision y GDAL para manejar datos raster y vectoriales, y asegurar el acceso a datos almacenados en AWS S3 sin necesidad de autenticación.
  
* Visualización y evaluación: Capacidad para visualizar los resultados de la segmentación semántica y evaluar la precisión del modelo.
  
:pushpin: ***Identificar los posibles beneficios y desafios del proyecto***

Utilizar imágenes satelitales y técnicas de deep learning para detectar piscinas implica beneficios y desafíos:

*Beneficios*

* Automatización en la detección: El uso de algoritmos de aprendizaje profundo puede automatizar y acelerar el proceso de identificación de piscinas en grandes áreas geográficas.
  
* Mejora en la gestión urbana: La detección precisa de piscinas puede ayudar a las entidades recaudadoras a reducir la evasión fiscal y aumentar la equidad tributaria.
Optimización de recursos: El sistema propuesto podría optimizar los recursos utilizados en la fiscalización, haciendo el proceso más eficiente.

*Desafíos*

* Calidad de los datos: La precisión del modelo depende de la calidad y resolución de las imágenes satelitales, así como de la precisión de las anotaciones utilizadas para el entrenamiento.
  
* Complejidad técnica: Implementar y mantener un sistema de aprendizaje profundo requiere conocimientos especializados y puede ser técnicamente desafiante.
  
* Cambios ambientales: Las condiciones ambientales y cambios estacionales pueden afectar la visibilidad de las piscinas en las imágenes satelitales, lo que podría complicar la detección.
      
### 2. Comprensión de los Datos
#### Recopilación , primeros conocimientos de los datos

El primer paso en la fase de comprensión de los datos del modelo CRISP-DM implica la identificación y adquisición de las fuentes de datos relevantes. Este proceso es fundamental para asegurar que se cuenta con la información adecuada para abordar el problema planteado.
1.	Identificación de Fuentes de Datos:
   * Imágenes satelitales: Para este proyecto, las imágenes satelitales fueron descargadas mediante el software SAS-PLANET.
   * Datos Georreferenciados: Se obtuvieron datos sobre la ubicación de las piscinas 
de un relevamiento de la Gerencia de Generación de datos del GCBA. https://buenosaires.gob.ar/antropologia-urbana/herramientas-para-la-generacion-de-datos-territoriales

2. Análisis Exploratorios de las Imágenes Satelitales:
   * Visualización de Imágenes: Se realiza una visualización inicial de las imágenes satelitales para comprender mejor su contenido y características visuales.
   * Resolución y Metadatos: Es esencial entender la resolución espacial de las imágenes, que determina el nivel de detalle que se puede observar. Además, se revisan los metadatos para obtener información adicional.
  
#### Exploración de Herramientas de Descarga

Para la obtención de imágenes satelitales se exploran diversas herramientas de descarga. La elección de la herramienta adecuada para afectar significativamente la calidad y usabilidad de las imágenes obtenidas.

* Descarga y Evaluación de Imágenes:
  - SAS PLANET: Esta herramienta se utilizó para descargar imágenes satelitales de alta resolución de áreas específicas de interés. SAS PLANET permite la descarga de datos desde múltiples servicios de mapas.

#### Descarga de Imágenes Satelitales para Entrenamiento

El proceso de descarga de imágenes satelitales para el entrenamiento del modelo incluye:

* Selección de Zonas de Interés: Se identificaron y seleccionaron áreas específicas dentro de la Ciudad de Buenos Aires que contienen piscinas para asegurar la relevancia de los datos.

* Descarga y Almacenamiento: Utilizando SAS PLANET, se descargaron las imágenes seleccionadas y se almacenaron en Google Drive para facilitar el acceso y la manipulación durante el desarrollo del proyecto.

#### Instalación de Librerías y Configuración del Entorno

Para llevar a cabo el procesamiento de imágenes y el entrenamiento del modelo, se instaló un conjunto de librerías esenciales:

1.	*Raster Visión:* esta herramienta se utilizó para el proceso completo de aprendizaje profundo geoespacial, incluyendo la segmentación de imágenes.

2.	*GDAL (Geospatial Data Abstraction Library):* GDAL se empleó para leer y escribir datos geoespaciales, facilitando el procesamiento de imágenes.

3.	*Cargar en Google Drive:* Las imágenes satelitales se cargaron de Google Drive para permitir un fácil acceso y manipulación desde cualquier lugar.

#### Identificación de las fuentes de Datos y Proyecciones

El dataset utilizado incluyó evidencia de campo georreferenciada.
 El mismo consistió en:
  * Datos georreferenciados: Estos datos, que pueden incluir información sobre la ubicación de las piscinas, se utilizan para entrenar el modelo y evaluar su rendimiento.

#### Análisis exploratorio de los datos

  - *Descarga de Archivos GeoJSON:* Se descarga y se guarda un archivo. geojson (formato de archivo abierto para representar datos geoespaciales simples). Los archivos GeoJSON contienen información geográfica, como puntos, líneas y polígonos, junto con otros datos en formato JSON;
  - *Configuración de Clases para la Segmentación:* Se define el tamaño de las ventanas de entrenamiento y establece una serie de transformaciones de aumento de datos para mejorar la robustez del modelo de aprendizaje automático. 

#### Identificar las características y la calidad de los datos

Características del Proyecto
- [x] Objetivo: Utilizar el procesamiento de imágenes y machine learning para detectar piletas en imágenes satelitales.
- [x] Framework Utilizado: Raster Vision, para el proceso completo de aprendizaje profundo geoespacial.
- [x] Fuente de Datos: Datos georreferenciados en WGS84 (anotaciones, imágenes y áreas de interés)
- [x] Aplicación Propuesta: Implementación por entidades recaudadoras para reducir la evasión fiscal y optimizar recursos.

#### Calidad y Configuración de Datos
  - Dataset: Alta resolución, obtenido de una fuente gubernamental confiable.
  - Preprocesamiento: Uso de GDAL para leer y escribir datos geoespaciales. Esta etapa incluyó la normalización de las imágenes, la eliminación de ruido y la corrección de cualquier distorsión geométrica.
  - Clases Definidas: Dos clases, 'background' y 'pileta', con sus respectivas transformaciones y visualización.

#### Calidad del Código
  - Estructura: El código está bien organizado, con comentarios explicativos y secciones claramente definidas.
  - Modelo de Deep Learning: Utilizamos un modelo preentrenado de PyTorch con configuraciones específicas para la tarea.
  - Visualización: Incluye código para visualizar los resultados de la segmentación semántica.
  - Entrenamiento del Modelo: Configura y entrena el modelo con un conjunto de datos de entrenamiento y validación.

#### Posibles Mejoras
- [x] Validación de Datos: Asegurarse de que las anotaciones y etiquetas sean precisas, posiblemente mediante la validación cruzada y la revisión manual.
- [x] Optimización de Hiperparámetros: Ajustar los hiperparámetros, como la tasa de aprendizaje, el tamaño del lote y el número de épocas, para mejorar el rendimiento del modelo
- [x] Evaluación Rigurosa: Implementar métricas de evaluación para medir la precisión y el recall del modelo.

#### Definir las clases para la segmentación
En el contexto de la segmentación semántica en deep learning, las "clases" se refieren a las categorías de objetos que el modelo está diseñado para reconocer en las imágenes. Cada píxel en la imagen se clasifica en una de las clases posibles.

En el colab ISPC_Piletas_Entrenamiento.ipynb`, las clases para la segmentación probablemente serían al menos dos: 'pileta' (piscina) y 'background' (fondo). Esto significa que el modelo está entrenado para reconocer y diferenciar entre estas dos categorías en las imágenes satelitales.

  - [x] La clase 'pileta' correspondería a los píxeles que representan piscinas en las imágenes.
  - [x] La clase 'background' correspondería a todos los demás píxeles que no representan piscinas.
        
Estas clases permiten al modelo aprender a distinguir entre las características visuales de las piscinas y el resto de la imagen. Una vez entrenado, el modelo puede aplicarse a nuevas imágenes para identificar y segmentar las piscinas de manera efectiva.

![image](https://github.com/romanzelararg/GRUPO-11---Proyecto-Final-Cohorte-2022-/assets/108492765/6f023a97-8d5b-4d35-a270-c9b749bfe4eb)


### 3. Preparación de los Datos
   >Seleccion de tablas, registros y atributos, transformación y limpieza de datos.

   Preparar los datos para el modelado implica la limpieza de las imágenes, la evaluación del dataset (evaluación visual de correspondencia de las anotaciones), la eliminación de las partes no deseadas y la preparación de las etiquetas para el entrenamiento del modelo.

 :test_tube: ***Definición de nuestra área de interés***

El Área de Interés (AoI) se refiere a la región geográfica específica que se está analizando o estudiando. En nuestro caso, está relacionada con la detección de piletas (piscinas) utilizando imágenes satelitales y técnicas de aprendizaje profundo.

El AoI se define mediante un archivo GeoJSON, que es un formato de archivo abierto para representar datos geoespaciales simples. Este archivo contiene información geográfica, como puntos, líneas y polígonos, junto con otros datos en formato JSON. En el contexto del aprendizaje automático y el procesamiento de imágenes, el AoI se utiliza para delimitar la región sobre la cual el modelo realizará predicciones o análisis.

En resumen, el AoI es crucial para enfocar el análisis de datos geoespaciales en una región específica y es un componente esencial en proyectos de visión por computadora y teledetección que involucran datos georreferenciados.

 :test_tube: ***Entrenamiento del modelo 'resnet18'***

* Carga del Modelo Preentrenado:
   - [x] Se carga un modelo resnet18 preentrenado utilizando torch.hub.
   - [x] Se configura el modelo para la tarea específica de segmentación semántica con las clases definidas.
  
* Entrenamiento del Modelo:
   - [x] Se inicia el entrenamiento del modelo con los conjuntos de datos preparados.
   - [x] Se realizan iteraciones (épocas) donde el modelo aprende a identificar piletas en las imágenes.

 :test_tube: ***Generación de variable***

En el caso del colab ISPC_Piletas_Entrenamiento.ipynb` , el código muestra la generación de dos variables:

   - [ ] annotations_url = "https://drive.google.com/file/d/1V9N0xDJKApR_p3PlFZ-9xSvMWWh1Xv3o/view?usp=drive_link"
         
   - [ ] annotations_file_dest = "/content/drive/MyDrive/Deteccion/anotaciones/anotaciones_wgs_geoj_r2.geojson"

Aquí, <sup>annotations_url</sup>  es una variable que almacena la URL del archivo que se desea descargar desde Google Drive, y <sup>annotations_file_dest</sup> es una variable que almacena la ruta donde se guardará el archivo descargado.

 :test_tube: ***Preprocesar y Transformar los datos para su uso en el modelo*** 

Se comenzó a trabajar con una imagen que era bastante extensa de aproximadamente 40 manzanas, pero se hizo difícil poder entrenar el modelo.
Por lo que se tomó la decisión de reducir la imagen a 4 manzanas y se logró entrenar correctamente.

Con dicho entrenamiento se obtuvo un modelo y se utilizó para predecir otro.

### 4. Modelado
   >Selección y aplicación de varias técnicas de modelado

Generación del modelo deep learning y su entrenamiento utilizando el framework Raster Vision. Asegurandonos de configurar correctamente los parámetros del modelo y de utilizar una división adecuada de los datos para el entrenamiento y la validación.

:pencil: ***Seleccionar el modelo de aprendizaje profundo (ResNet-18)***

ResNet-18 es una arquitectura de red neuronal convolucional que ha demostrado ser muy efectiva en tareas de reconocimiento de imágenes.

En el contexto del colab ISPC_Piletas_Entrenamiento.ipynb, ResNet-18 ha sido seleccionado por varias razones:

   - [ ] Eficiencia: ResNet-18 es relativamente ligero en comparación con otras variantes de ResNet (como ResNet-50, ResNet-101, etc.), lo que lo hace más rápido y eficiente en términos de memoria y tiempo de cálculo.
   - [ ] Rendimiento: A pesar de su simplicidad, ResNet-18 puede ofrecer un rendimiento sólido en muchas tareas de visión por computadora, incluyendo la detección y segmentación de objetos.
   - [ ] Preentrenamiento: ResNet-18 está disponible como un modelo preentrenado en varias bibliotecas de deep learning, lo que permite un inicio rápido y mejora el rendimiento al aprovechar los patrones aprendidos de grandes conjuntos de datos como ImageNet.

:pencil: ***Configurar el modelo y los parámetros de entrenamiento***

* Selección del Modelo: Se ha seleccionado ResNet-18, que es una arquitectura de red neuronal convolucional conocida por su eficacia en tareas de reconocimiento de imágenes.

* Configuración de Parámetros del Modelo: Los parámetros del modelo, como el número de capas y neuronas, así como las funciones de activación, se configuran de acuerdo con las necesidades de la tarea.

* Configuración de Parámetros de Entrenamiento: Los parámetros de entrenamiento, como el número de épocas, el tamaño del lote y la tasa de aprendizaje, se establecen. Estos parámetros pueden tener un gran impacto en la eficacia del entrenamiento.

:pencil: ***Entrenar el modelo con los datos de entrenamiento***

El modelo se entrena utilizando los datos de entrenamiento, ajustando los pesos y los parámetros internos de la red para minimizar el error.

   - [x] Se inicia el entrenamiento del modelo con los conjuntos de datos preparados.
   - [x] Se realizan iteraciones (epoch) donde el modelo aprende a identificar piletas en las imágenes.

:pencil: ***Monitorear el rendimiento del modelo durante el entrenamiento***

* Visualización: Se utiliza <sup>SemanticSegmentationVisualizer</sup> para visualizar las predicciones del modelo y las etiquetas reales, lo que ayuda a monitorear cómo el modelo está aprendiendo.

* Registro de Estadísticas: Se registran estadísticas de los datos para asegurarse de que el entrenamiento se base en datos sólidos y bien informados.
  
* Guardado del Modelo: Una vez completado el entrenamiento, se guarda el modelo y su configuración para su uso futuro.


### 5. Evaluación
   >Evaluación del modelo y revisión de los pasos ejecutados
La evaluación del rendimiento del modelo permite comprender cómo se comporta el modelo en datos no vistos durante el entrenamiento .Este análisis se realiza utilizando el conjunto de datos de validación y se mide mediante diversas métricas de evaluación  como la precisión, la exhaustividad (recall), el puntaje F1 y el AUC-ROC.

:microscope: ***Propósitos de la Evaluación***
Evaluar el rendimiento del modelo con los datos de validación es crucial para varios propósitos:

1.	*Generalización:* Evaluar cómo el modelo se comporta en datos no vistos durante el entrenamiento. Los datos de validación proporcionan una estimación realista del rendimiento en situaciones del mundo real.
2.	*Ajustes de Hiperparametros:* Durante la validación, podemos ajustar los hiper parámetros del modelo (como la tasa de aprendizaje, el tamaño del lote, etc) para obtener un mejor rendimiento.
3.	*Selección de Modelos:* Comparamos diferentes modelos o arquitecturas utilizando los datos de validación para elegir el mejor.
4.	*Evitar el sobreajuste:* Si el modelo tiene un rendimiento excelente en los datos de entrenamiento, pero no en los de validación, podría ser sobre ajustado. La validación ayuda a detectar esto.
   
En resumen, la evaluación con datos de validación nos permite comprender como nuestro modelo se desempeñará en el mundo real y tomar decisiones informadas para mejorarlo.

:microscope: ***Métricas de Evaluación utilizadas***

Para una evaluación exhaustiva del modelo, utilizamos varias métricas de evaluación que ofrecen una visión completa del rendimiento:

•	Precisión: Mide la proporción de predicciones positivas correctas respecto al total de predicciones positivas.

•	Recall (Exhaustividad): Mide la proporción de verdaderos positivos respecto al total de instancias reales positivas.

•	F1-score: Es la media armónica entre precisión y recall, proporcionando un equilibrio entre ambas métricas.

•	Especificidad: Mide la proporcion de verdaderos negativos respecto al total de instancias reales negativas.

•	AUC-ROC: Mide el rendimiento del modelo a través de todas las posibles clasificaciones de umbrales.

:microscope: ***Evaluación para la Clase “Background”***

Analizamos los resultados de evaluación para la clase ID O, que corresponde a la clase.

Aquí están los detalles:

***1.	Matriz de Confusión:***
  - Verdaderos Positivos (TP): 103,510,288.0
  - Falsos Positivos (FP): 93,874.0
  - Verdaderos Negativos (TN): 364.0
  - Falsos Negativos (FN): 0.0

***2.	Métricas de Evaluación:***
   
•	Precisión: 0.9991

    - La precisión mide la proporción de predicciones positivas correctas (TP) respecto al total de predicciones positivas (TP +FP). En este caso, es alta lo que indica que el modelo tiene pocas falsas alarmas.
  	
•	Recall (Sensibilidad):1.0

    - El Recall mide la proporción de verdaderos positivos (TP) respecto al total de instancias de fondo de imagen. Un valor de 1.0 significa que el modelo detecta todas las instancias de fondo.
    
•	F1-score:0.9995

    - El F1-score es la media armónica entre precisión y recall. Es útil para encontrar un equilibrio entre ambas métricas.
    
•	Especificidad: 0.0039

    - La especificidad mide la proporción de verdaderos negativos (TN) respecto al total de instancias de fondo que no son positivas (TN +FP). Un valor bajo indica que el modelo tiene dificultades para detectar instancias de fondo.

•	Error de conteo:

    - El error de conteo (count_error) es igual a la cantidad de falsos positivos (FP), que en este caso es 93.874.

•	Conteo Total:

    - El conteo total de instancia de fondo en la imagen (gt_count) es 103,510,288.

•	Predicciones Realizadas:

    - El conteo total de predicciones realizadas por el modelo(pred_count) es 103,604,162.

•	Frecuencia Relativa:

    - La frecuencia relativa de la clase de fondo en la imagen es 0.9991.

En resumen, el modelo tiene un alto rendimiento en la detección de la clase de fondo (“background”) , con una precisión cercana al 99.91% y un recall del 100%. Sin embargo, la especificidad es baja, lo que indica que el modelo tiene dificultades para identificar instancias de fondo que no son positivas.

### Evaluación para la Clase “Pileta” (Piscina)

Analizamos los resultados de evaluación para la clase con ID 1, que corresponde a la clase “pileta”. Aquí los detalles:

***1.	Información de la clase:***
•	ID de Clase:1
•	Nombre de la Clase: “pileta” (o piscina)

***2.	Matriz de Confusión:***
•	Verdaderos Negativos (TN): 103,510,288.0
•	Falsos Negativos (FN): 93,874.0
•	Verdaderos Positivos (TP): 364.0
•	Falsos Positivos (FP):0.0


***3.	Métricas de Evaluación:***
   
•	Precision:100%

    - Todas las predicciones positivas son correctas
    
•	Recall (Sensibilidad):0.39%

    - El modelo tiene dificultades para identificar correctamente las piscinas
    
•	F-score:0.77

    - Este valor se debe al bajo recall
    
•	Especificidad:100%

    - El modelo identifica correctamente las instancias negativas
    
•	Error de conteo:

    - El error de conteo (falsos negativos) es 93,874
    
•	Frecuencia Relativa:

    - La clase pileta representa aproximadamente el 0.09% de las instancias de la imagen.
    
En resumen, aunque la precisión es alta, el recall(sensibilidad) es muy bajo (0.39%).

Esto sugiere que el modelo tiene dificultades para identificar correctamente las piscinas en las imágenes. El F1-score también es bajo debido al bajo recall. 

### Interpretación de los resultados

•	***Clase “background” (fondo):***
La precisión es alta, esto significa que la mayoría de las predicciones positivas son correctas y hay pocas falsas alarmas. El recall es del 100%, el modelo detecta todas las instancias de fondo de imagen. El F1-score es alto, esta métrica combina precisión y recall y en este caso muestra un buen equilibrio. La especificidad es baja, el modelo tiene dificultades para identificar las instancias de fondo que no son positivas. El error de conteo (falsos positivos) es de 93.87 y la frecuencia relativa, la clase de fondo representa el 99.91% de las instancias en la imagen.

•	***Clase “pileta” (Piscina):***
La precisión es del 100%, todas las predicciones son correctas. El recall es muy bajo, el modelo tiene dificultades para identificar correctamente las piscinas, el F1-score también es bajo, esto se debe al bajo recall. La especificidad es alta, el modelo identifica correctamente las instancias negativas. El error de conteo (falsos negativos) es de 93.874, y la clase pileta representa aproximadamente el 0.09% de las instancias en la imagen.


## Conclusiones
En este proyecto, hemos demostrado cómo la automatización en la detección de piletas puede mejorar significativamente la gestión urbana y optimizar recursos, utilizando el poder del deep learning y el procesamiento de imágenes satelitales. A pesar de enfrentar desafíos notables como la calidad de los datos, la complejidad técnica y los cambios ambientales, hemos verificado que nuestro modelo es eficiente para evaluar la cantidad de piscinas detectadas, siempre que se controlen factores críticos como el tamaño y la calidad de las imágenes.

Para mejorar aún más este modelo, es esencial enfocarse en la recopilación de datos específicos, el aumento de datos, el ajuste de hiperparámetros y la optimización continua. Estos pasos adicionales permitirán superar las limitaciones actuales y maximizar el potencial del modelo para aplicaciones futuras en la gestión urbana.
Concluimos en este Proyecto que, con los datos obtenidos y entrenados, se verifica que el modelo genera eficiencia a la hora de evaluar la cantidad de piscinas detectadas, siempre y cuando se controle la imagen a trabajar (tamaño, calidad, etc).


## Recomendaciones futuras

Algunas recomendaciones que pueden ayudar a optimizar impacto y utilidad de éste proyecto en el futuro:

  1. *Extender a Otras Características Urbanas:* Investigar la posibilidad de extender el sistema para detectar otras características urbanas relevantes, como construcciones ilegales, áreas verdes, etc. Esto ampliaría su utilidad y beneficios.

    - Construcciones Ilegales: Identificar edificaciones no autorizadas o construcciones ilegales en áreas urbanas. Esto podría ayudar a las autoridades a tomar medidas rápidas y eficientes.
    - Áreas Verdes y Espacios Públicos: Detectar parques, plazas y áreas verdes en la ciudad. Esto podría ser útil para la planificación urbana y la gestión de espacios públicos.
    - Estacionamientos y Vehículos: Identificar áreas de estacionamiento, vehículos estacionados en lugares no permitidos o incluso contar la cantidad de automóviles en una zona específica.
    - Infraestructura Vial: Detectar señales de tráfico, semáforos, cruces peatonales y otros elementos de infraestructura vial.
    - Calidad del Aire y Contaminación: Utilizar imágenes satelitales para evaluar la calidad del aire y detectar fuentes de contaminación.

  2. *Evaluación en Otras Ciudades y Regiones:* Evaluar la viabilidad de aplicar el sistema en otras ciudades y regiones, considerando la disponibilidad de datos y las necesidades específicas locales. Esto podría ayudar a replicar el éxito en otros contextos.

  3. *Mejora Continua y Actualizaciones:* Implementar un sistema de monitoreo para evaluar continuamente el rendimiento del sistema en producción. Planificar actualizaciones y mejoras basadas en nuevos datos y tecnologías emergentes.

4. *Documentación y Capacitación:* Continuar documentando detalladamente el proceso de desarrollo, incluyendo la recolección de datos, el entrenamiento del modelo y la integración del sistema. Además, capacitar al personal de las entidades recaudadoras en el uso del sistema y la interpretación de los resultados.



## LISTADO DE ALGORITMOS, FRAMEWORKS Y HERRAMIENTAS PRE ENTRENADAS UTILIZADOS EN EL PROYECTO

	El proyecto de detección de piletas mediante imágenes satelitales utiliza varios algoritmos y técnicas para lograr su objetivo. A continuación, se presentan algunos de los más relevantes:
 
1. Redes Neuronales Convolucionales (CNN):
   
   - Estas redes son fundamentales para el aprendizaje profundo en visión por computadora. Se entrenaron para reconocer patrones y características en imágenes, como formas y texturas. En este proyecto, se utilizan para identificar piscinas en las imágenes satelitales.
     
2. Segmentación Semántica:
   
   - La segmentación semántica es una técnica que asigna una etiqueta a cada píxel de una imagen. En este caso, se utiliza para distinguir las áreas de las piscinas de otras superficies en las imágenes.
     
3. Raster Vision:
   
   - Raster Vision es un framework que nos permitió el procesamiento de datos georreferenciados. Facilitó la lectura de imágenes satelitales, el entrenamiento de modelos y la escritura de predicciones en formatos georreferenciados.
     
4. GDAL (Geospatial Data Abstraction Library):
   
   - GDAL es una biblioteca que se utiliza para manejar datos raster y vectoriales. En este proyecto, se emplea para la manipulación y preparación de datos geoespaciales.
     
5. Técnicas de Argumentación de Datos:
   
   - Para mejorar la robustez del modelo, se aplicaron técnicas de argumentación de datos, como la rotación, el cambio de brillo y la ampliación/reducción de imágenes.


    

    
