# TSCDIA 2023 
# PRACTICA PROFESIONALIZANTE - ISPC
## Sala 2 -Grupo 22

# Título del Proyecto: _Predicción de Conectividad y Población en Argentina_ :technologist:

_Colaboradores:_  
 
:woman_technologist: [Barea Silvana](https://github.com/recursosssbb) 
    
:woman_technologist: [Hanún Romina](https://github.com/RomiHanun)
    
:man_technologist: [Juchniewicz Federico](https://github.com/FJISPC)  
    
:man_technologist: [Kanneman Samuel](https://github.com/samuelkanneman) 
    
:woman_technologist: [Lucero Carla](https://github.com/CarlaLucerocd)
     
:man_technologist: [Mansilla Leonardo Matias](https://github.com/LMmansilla)
     
:man_technologist: [Zelarayán Román](https://github.com/romanzelararg)

## Descripción : :globe_with_meridians:
***Este proyecto tiene como objetivo desarrollar un sistema de aprendisaje automático que pueda predecir y clasificar la conectividad a internet y la población de las localidades de Argentina , identificar patrones significativos , correlaciones entre otras variables y presentar los resultados de manera comprensible.***
 

## Enlace de Demostración:

## Tabla de Contenidos:

++Preparacion de los espacios de Trabajo.

   + Creacion Repositorio GitHub.
   + Creacion Proyecto Trello.

++Análisis Descriptivo del Dataset:**

   + Cambios Extructurales.
   
   + Confección de encoding.
   
   + Transformación de los Datos a binarios.
   
   + Creación columna concatenada Provincia-Partido-Localidad.
   
   + Eliminación de datos repetidos.
   
   + Análisis descriptivo del Dataset.
   
   + Análisis y transformación de las variables Provincia-Partido-Población.
   
   + Merge con distintas tablas de interés.
   
       - Merge 1 (Accesos a internet fijo por tecnología y localidad).
   
       - Merge 2 (Se agregan los datos de población por provincia al dataframe de base).
   
       - Merge 3 (Acceso a internet por cada 100 habitantes y por cada 100 hogares).
   
       - Merge 4 (Salarios promedio y mediano por provincia)

   ++ Limpieza de datos

   ++ Analisis Exploratorio con Graficos.

   ++ Definir Modelos a Entrenar

   ++ Exploracion de los distintos modelos.

   + Modelo Regresion Lineal.

   + Modelo Regresion Logistica
   
   + Modelo  K-means
     
   + Modelo DBSCAN

   ++ Evaluacion Y Conclusion de los distintos Modelos.

## Comprensión Empresarial: :bar_chart:

Problemas y  oportunidades detectados.
La conectividad a internet es un factor clave para el desarrollo económico y social de una localidad. Sin embargo, la conectividad a internet no está distribuida de manera uniforme en Argentina. Algunas localidades tienen una conectividad a internet muy alta, mientras que otras tienen una conectividad a internet muy baja.

Este proyecto tiene como objetivo contribuir a mejorar la conectividad a internet en Argentina. El sistema de aprendizaje automático desarrollado en este proyecto podría ser utilizado por las autoridades gubernamentales para identificar las localidades con una conectividad a internet baja y desarrollar políticas para mejorar la conectividad en estas localidades.

_Objetivo General:_
Desarrollar un sistema de aprendizaje automático que pueda predecir y clasificar la conectividad a internet y la población de las localidades en Argentina, identificar patrones significativos y correlaciones entre estas variables, y presentar los resultados de manera comprensible.

_Objetivos Específicos:_

 - [x] Predecir la conectividad a internet de una localidad en función de su población, ubicación geográfica, infraestructura, etc.

 - [x] Predecir la cantidad de conecciones de un tipo especifico en 2022 en función de otras variables.

 - [x] Predecir la poblacion en 2022 en función de las variables proporcionadas.
       
 - [x] Clasificar las localidades en función de su conectividad a internet.

 - [x] Analizar la relacion entre el acceso a internet y la población en diferentes regiones.

 - [x] Explorar patrones en la distribución de conexiones de Internet.

 - [x] Identificar patrones significativos y correlaciones entre la conectividad a internet y la población de las localidades.

 - [x] Presentar los resultados de manera comprensible para los usuarios.


       

## Comprensión de Datos: :card_index_dividers:
1. _Los  dataset utilizados corresponden a la página de ENACOM (Ente Nacional de Comunicaciones)_ 
https://datosabiertos.enacom.gob.ar/dataviews/241175/conectividad-al-servicio-de-internet/

    - _Se realizó la concatenación de los dataset para la obtención de mayor cantidad de datos._ 
https://datosabiertos.enacom.gob.ar/dataviews/252830/accesos-a-internet-fijo-por-tecnologia-y-localidad/ 

    - _Confeccionamos un tablero Trello, utilizando esta herramienta de gestión de Proyectos, con el fin de obtener organización , colaboración, seguimiento del progreso y gestionar de manera efectiva todas las etapas del Proyecto.Link Trello:_ https://trello.com/w/proyectogrupo22pp1
  
El conjunto de datos contiene información relacionada con diferentes provincias y localidades de Argentina, incluyendo datos demográficos, de acceso a servicios de comunicación y ubicaciones geográficas. A continuación, se detallan las columnas presentes en el conjunto de datos:

* Year: Año de los datos.
  
* Quarter: Trimestre del año al que pertenecen los datos.
  
* Provincia: Provincia a la que pertenece la información.
  
* Partido: Partido dentro de la provincia.
  
* Localidad: Nombre de la localidad.
  
* Población_2022: Población en el año 2022.
  
* Acc_cada_100_hog: Acceso a Internet cada 100 hogares.
  
* Acc_cada_100_hab: Acceso a Internet cada 100 habitantes.
  
* ADSL_2022: Número de conexiones ADSL en 2022.

* Cablemodem_2022: Número de conexiones por cable en 2022.
   
* Dial Up_2022: Número de conexiones Dial Up en 2022.
  
* Fibra optica_2022: Número de conexiones de fibra óptica en 2022.
  
* Satelital_2022: Número de conexiones satelitales en 2022.
  
* Wireless_2022: Número de conexiones inalámbricas en 2022.
  
* Telefonia Fija_2022: Número de líneas de telefonía fija en 2022.
  
* 3G_2022: Número de conexiones 3G en 2022.
  
* 4G_2022: Número de conexiones 4G en 2022.
  
* Cant_ADSL_2022: Cantidad de conexiones ADSL en 2022.
  
* Cant_Cablemodem_2022: Cantidad de conexiones por cable en 2022.
  
* Cant_DialUp_2022: Cantidad de conexiones Dial Up en 2022.
  
* Cant_FibraOptica_2022: Cantidad de conexiones de fibra óptica en 2022.
  
* Cant_Otros_2022: Cantidad de otras conexiones en 2022.
  
* Cant_Satelital_2022: Cantidad de conexiones satelitales en 2022.
  
* Cant_Wimax_2022: Cantidad de conexiones Wimax en 2022.
  
* Cant_Wireless_2022: Cantidad de conexiones inalámbricas en 2022.
  
* Total_2022: Total de conexiones en 2022.
  
* Pob_prov_2022: Población provincial en 2022.
  
* Salario_promedio: Salario promedio.
  
* Latitud: Coordenada de latitud.
  
* Longitud: Coordenada de longitud.


## Marco Conceptual.
_El marco conceptual de este proyecto se basa en las siguientes áreas:_
*	Aprendizaje automático: El aprendizaje automático es un campo de la inteligencia artificial que se centra en desarrollar algoritmos que pueden aprender de los datos sin ser explícitamente programados.
  
*	Predicción: La predicción es el proceso de estimar el valor futuro de una variable en función de sus valores pasados.
  
*	Clasificación: La clasificación es el proceso de asignar una etiqueta a un objeto en función de sus características.

*	Análisis de agrupamiento: El análisis de agrupamiento es el proceso de agrupar objetos similares.

*	Análisis de correlación: El análisis de correlación es el proceso de medir la relación entre dos variables.

## Metodología: :clipboard:
_La metodología que se utilizará en este proyecto se basa en los siguientes pasos:_

1.	Obtención de los datos: Los datos se obtendrán del dataset "Conectividad al servicio de Internet (Argentina)" publicado por el Ente Nacional de Comunicaciones (ENACOM).
   
2.	Preparación de los datos: Los datos se prepararán para el análisis de aprendizaje automático. Esto incluye la eliminación de valores atípicos, la codificación de las variables categóricas, y la normalización de los datos.

3.	Entrenamiento del modelo: El modelo de aprendizaje automático se entrenará utilizando los datos preparados.

4.	Evaluación del modelo: El modelo se evaluará utilizando un conjunto de datos de prueba.
   
5.	Presentación de los resultados: Los resultados del modelo se presentarán de manera comprensible para los usuarios.
   
## Highlights:
:pushpin: •	El sistema de aprendizaje automático desarrollado en este proyecto es capaz de predecir la conectividad a internet de una localidad con un alto grado de precisión.

:pushpin: •	El sistema de aprendizaje automático desarrollado en este proyecto es capaz de clasificar las localidades en función de su conectividad a internet.

:pushpin: •	El sistema de aprendizaje automático desarrollado en este proyecto es capaz de identificar patrones significativos y correlaciones entre la conectividad a internet y la población de las localidades.

:pushpin: •	El sistema de aprendizaje automático desarrollado en este proyecto presenta los resultados de manera comprensible para los usuarios.

## Captura de Pantalla de Visualiaciones/Resultados:

## Estado
En Proceso. :construction_worker:

## Limitaciones:
> [!IMPORTANT]
> Una limitación del sistema de aprendizaje automático desarrollado en este proyecto es que depende de la calidad de los datos utilizados para entrenarlo. Si los datos están sesgados o incompletos, el sistema puede generar resultados imprecisos.

> [!IMPORTANT]
> Otra limitación del sistema es que es un modelo general. Esto significa que no está diseñado para una aplicación específica. Para utilizar el sistema para una aplicación específica, es necesario ajustar los parámetros del modelo.

## Oportunidades de mejora:
Para mejorar el sistema de aprendizaje automático desarrollado en este proyecto, se recomienda utilizar un conjunto de datos más grande y diverso. Esto ayudará a mejorar la precisión del sistema.

También se recomienda desarrollar modelos específicos para aplicaciones específicas. Esto ayudará a mejorar el rendimiento del sistema en estas aplicaciones.


## Conclusión:
***El sistema de aprendizaje automático desarrollado en este proyecto es una herramienta valiosa para mejorar la conectividad a internet en Argentina. El sistema puede ser utilizado por las autoridades gubernamentales para identificar las localidades con una conectividad a internet baja y desarrollar políticas para mejorar la conectividad en estas localidades.***

                                                                                              

  







