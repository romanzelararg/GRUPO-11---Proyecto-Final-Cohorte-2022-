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
   >Objetivos y requisitos del Proyecto, definición del problema y plan preliminar diseñado
   
   #### :floppy_disk: *Mediante el framework Raster Vision se propone realizar el procedimiento completo de aprendizaje profundo geoespacial:*
 * Leer datos georreferenciados
 * Entrenar modelos
 * Realizar predicciones
 * Escribir predicciones en formatos georreferenciados.
   
#### :computer: *Se propone desarrollar un sistema automatizado que use:*
:white_check_mark: _Imágenes satelitales de alta resolución para identificar posibles piletas_

:white_check_mark: _Algoritmos de aprendizaje profundo, entrenados para reconocer formas y reflejos de agua en las imágenes_.

   #### :chart_with_upwards_trend: *Este sistema podría implementarse por entidades recaudadoras para:*
- [x] *Reducir la evasión fiscal*
- [x] *Aumentar la equidad tributaria*
- [x] *Optimizar recursos en la fiscalización*.
      
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

    
