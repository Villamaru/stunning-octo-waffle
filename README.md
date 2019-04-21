# Proceso del analisis exploratorio de la base de datos de Properati (2007)
Objetivos: 
 
- Efectuar una limpieza del dataset provisto. Particularmente, deberá diseñar estrategias para lidiar con los datos perdidos en ciertas variables. 

- Realizar un análisis descriptivo de las principales variables. 

- Crear nuevas columnas a partir de las características dadas que puedan tener valor predictivo. 
 
1-Pre_Analisis.ipynb - Analisis preliminar del proceso de limpieza.

2-Modificacion_de_datos.ipynb -Re-estabilizacion de los valores para fines del paso 3.

3-Tasado_lineal.ipynb

## **Puntos de vista generales:**
- Para hacer un programa que permita predecir el valor por metro cuadrado podriamos utilizar la variable "surface_total_in_m2" o "surface_covered_in_m2" para predecir la variable "price", estas tres features parecen tener mas relacion entre si que con "price_per_m2" la cual puede ser inferida de las anteriores.


![alt text](https://github.com/Villamaru/stunning-octo-waffle/blob/master/imagenes/heatmap.png "Heatmap")

## **Por hacer:**

- Organizar el analisis inicial de los datos
  - Realizar un analisis visual mas representativo para las variables, sobretodo las ultimas 9.
- Revision ortografica

- Crear el archivo 3 referente a la implementacion del predictor.
  - Limpieza de las variables para entregarle al predictor.
  - Analisis sobre la relacion entre las variables.


