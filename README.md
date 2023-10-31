# TSCDIA 2023 
# PRACTICA PROFESIONALIZANTE - ISPC
## Sala 2 -Grupo 22

# Título del Proyecto: _Predicción de Conectividad y Población en Argentina_ :technologist:

_Colaboradores:_  
     
:woman_technologist: [Hanún Romina](https://github.com/RomiHanun)
    
:man_technologist: [Juchniewicz Federico](https://github.com/FJISPC)  
    
:man_technologist: [Kanneman Samuel](https://github.com/samuelkanneman) 
    
:woman_technologist: [Lucero Carla](https://github.com/CarlaLucerocd)
     
:man_technologist: [Mansilla Leonardo Matias](https://github.com/LMmansilla)
     
:man_technologist: [Zelarayán Román](https://github.com/romanzelararg)

## Descripción : :globe_with_meridians:
***Este proyecto tiene como objetivo desarrollar un sistema de aprendisaje automático que pueda predecir y clasificar la conectividad a internet y la población de las localidades de Argentina , identificar patrones significativos , correlaciones entre otras variables y presentar los resultados de manera comprensible.***
 

## Enlace de Demostración:https://www.canva.com/design/DAFywakbuoo/BOWJAppxxA8C4_NUmh3gJw/watch?utm_content=DAFywakbuoo&utm_campaign=designshare&utm_medium=link&utm_source=editor

## Tabla de Contenidos:

++Preparación de los espacios de Trabajo.

   + Creación Repositorio GitHub.
   + Creación Proyecto Trello.

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
            
   ++ Análisis Exploratorio con Graficos.

   ++ Definir Modelos a Entrenar

   ++ Exploración de los distintos modelos.

   + Modelo Regresión Lineal.

   + Modelo Regresión Logística
   
   + Modelo  K-means
     
   + Modelo DBSCAN

   ++ Evaluación Y Conclusión de los distintos Modelos.

## Comprensión Empresarial: :bar_chart:

Problemas y  oportunidades detectados.
La conectividad a internet es un factor clave para el desarrollo económico y social de una localidad. Sin embargo, la conectividad a internet no está distribuida de manera uniforme en Argentina. Algunas localidades tienen una conectividad a internet muy alta, mientras que otras tienen una conectividad a internet muy baja.

Este proyecto tiene como objetivo contribuir a mejorar la conectividad a internet en Argentina. El sistema de aprendizaje automático desarrollado en este proyecto podría ser utilizado por las autoridades gubernamentales para identificar las localidades con una conectividad a internet baja y desarrollar políticas para mejorar la conectividad en estas localidades.

_Objetivo General:_
Desarrollar un sistema de aprendizaje automático que pueda predecir y clasificar la conectividad a internet y la población de las localidades en Argentina, identificar patrones significativos y correlaciones entre estas variables, y presentar los resultados de manera comprensible.

_Objetivos Específicos:_

 - [x] Predecir la conectividad a internet de una localidad en función de su población, ubicación geográfica, infraestructura, etc.

 - [x] Predecir la cantidad de conecciones de un tipo especifico en 2022 en función de otras variables.

 - [x] Predecir la población en 2022 en función de las variables proporcionadas.
       
 - [x] Clasificar las localidades en función de su conectividad a internet.

 - [x] Analizar la relación entre el acceso a internet y la población en diferentes regiones.

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

## Captura de Pantalla de Visualizaciones/Resultados:

Regresión Logistica

![image](https://github.com/romanzelararg/Grupo22-PP1-Sala2/assets/116818116/9e86a4df-0add-4fdf-95fd-8bfcac1dcb2b)

K-Means

![image](https://github.com/romanzelararg/Grupo22-PP1-Sala2/assets/116818116/a05d9c06-126d-4f83-a562-41ab11bf5fc1)

## Estado
Finalizado :construction_worker:

## Limitaciones:
> [!IMPORTANT]
> Una limitación del sistema de aprendizaje automático desarrollado en este proyecto es que depende de la calidad de los datos utilizados para entrenarlo. Si los datos están sesgados o incompletos, el sistema puede generar resultados imprecisos.

> [!IMPORTANT]
> Otra limitación del sistema es que es un modelo general. Esto significa que no está diseñado para una aplicación específica. Para utilizar el sistema para una aplicación específica, es necesario ajustar los parámetros del modelo.

## Oportunidades de mejora:
Para mejorar el sistema de aprendizaje automático desarrollado en este proyecto, se recomienda utilizar un conjunto de datos más grande y diverso. Esto ayudará a mejorar la precisión del sistema.

También se recomienda desarrollar modelos específicos para aplicaciones específicas. Esto ayudará a mejorar el rendimiento del sistema en estas aplicaciones.


## Conclusión:
Si bien nos planteamos al inicio los objetivos de realizar un modelo de Regresión Lineal y otro de Regresión Logística en base a los datos del conjunto de datos, en la marcha descubrimos que tambien se adaptaba mejor un modelo con Algoritmo K-means en función de un posible negocio que se quiera utilizar por parte de los interesados (stakeholders).
El modelo de Regresión Lineal nos indicó las mejores métricas, como vimos en la conclusión de dicho modelo.
Pero utilizando el modelo de Algoritmo Kmeans, para la finalidad del estudio a un stakeholder como ENACOM y el Gobierno Nacional que precisen conocer que provincias o localidades necesitan inversión para la instalación de nuevas tecnologías de Internet, el gráfico de resultados proporciona información valiosa.
	Se concluye con K-means que los clústeres 3 y 4, que representan las provincias y localidades con una densidad baja o muy baja de puntos de acceso a Internet, son los que requieren mayor inversión para mejorar la conectividad.
Específicamente, el clúster 4, que representa las zonas más aisladas y de difícil acceso, es el que requiere una inversión más urgente.
	Los clústeres 1 y 2, que representan las provincias y localidades con una densidad alta o media de puntos de acceso a Internet, son los que requieren una inversión menor para mejorar la conectividad.

Recomendaciones:
El Gobierno Nacional y ENACOM deben priorizar la inversión en las provincias y localidades que pertenecen a los clústeres 3 y 4.
La inversión debe centrarse en la instalación de nuevas tecnologías de Internet, como la fibra óptica y el 4G o 5G, para mejorar la conectividad en estas zonas.
Esta inversión ayudará a reducir la brecha digital y a garantizar el acceso a Internet a todos los ciudadanos de Argentina, independientemente de su ubicación geográfica.

Podemos concluir que este trabajo final representa un esfuerzo significativo en la aplicación de técnicas avanzadas de análisis de datos y aprendizaje automático.
Este proyecto no solo destaca por su enfoque técnico, sino también por su énfasis en el trabajo colaborativo y en grupo. La colaboración es fundamental en el campo de la ciencia de datos, ya que permite aprovechar la diversidad de conocimientos y habilidades de un equipo. La capacidad de trabajar en grupo facilita la resolución de problemas complejos, la generación de ideas y la discusión de enfoques que enriquecen la toma de decisiones. En este proyecto, la colaboración puede haber desempeñado un papel crucial en la selección de variables, la elección de algoritmos de aprendizaje automático y la interpretación de los resultados.
Para resumir, este proyecto demuestra cómo las técnicas de ciencia de datos pueden aplicarse de manera efectiva para abordar problemas del mundo real, como la predicción de la conectividad a internet y la población de localidades en Argentina. Además, resalta la importancia de la colaboración y el trabajo en grupo en la obtención de resultados más sólidos y completos. Estos enfoques son esenciales en el mundo actual, donde la recopilación y el análisis de datos desempeñan un papel fundamental en la toma de decisiones informadas y en la resolución de desafíos complejos.


                                                                                              

  







