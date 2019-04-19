# Proceso del analisis exploratorio de la base de datos de Properati (2007)
Objetivos: 
 
● Efectuar una limpieza del dataset provisto. Particularmente, deberá diseñar estrategias para lidiar con los datos perdidos en ciertas variables. 

● Realizar un análisis descriptivo de las principales variables. 

● Crear nuevas columnas a partir de las características dadas que puedan tener valor predictivo. 
 
Un analisis preliminar del proceso de limpieza se puede encontrar en Pre_Analisis.ipynb

## **Puntos de vista generales:**
- Para hacer un programa que permita predecir el valor por metro cuadrado podriamos utilizar la variable "surface_total_in_m2" o "surface_covered_in_m2" para predecir la variable "price", estas tres features parecen tener mas relacion entre si que con "price_per_m2" la cual puede ser inferida de las anteriores.


![alt text](https://github.com/Villamaru/stunning-octo-waffle/blob/master/imagenes/heatmap.png "Heatmap")

## **Por hacer:**

- Organizar el analisis inicial de los datos
  - Realizar un analisis escrito para las ultimas variables restantes; expresadas abajo.
- Revision ortografica

'lat-lon', 'lat', 'lon', 'price', 'currency','price_aprox_local_currency', 'price_aprox_usd', 'surface_total_in_m2','surface_covered_in_m2', 'price_usd_per_m2', 'price_per_m2', 'floor','rooms', 'expenses', 'properati_url', 'description', 'title','image_thumbnail'


