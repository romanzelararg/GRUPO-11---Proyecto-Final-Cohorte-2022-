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
    


      
## 2. Comprensión de los Datos
   >Recopilación , primeros conocimientos de los datos

:white_check_mark: _Instalación de librerías de RasterVision_ Estos comandos instalaron diferentes módulos del proyecto "raster-vision", cada uno responsable de una parte especifica de la funcionalidad del sistema. Al ejecutar estos comandos , preparamos el entorno raster-vision , asegurandonos de que todos los componentes necesarios están instalados y configurados correctamente.

:white_check_mark: _Carga de imágenes satelitales en Drive_ Instalamos una herramienta de linea de comandos que facilita la descarga de archivos desde Google Drive. Este paquete es especialmente útil para descargar archivos grandes que se encuentran en Google DRive , como las imágenes que utilizaremos y queremos automatizar este proceso en scripts o notebooks.
Instalamos GDAL , la cual es una biblioteca de código abierto para leer y escribir datos geoespaciales en una variedadd de formatos.

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

    
