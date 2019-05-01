# Proceso del analisis exploratorio de la base de datos de Properati (2007)

## **Por hacer:**

- Organizar el analisis inicial de los datos.
  - Realizar un analisis visual mas representativo para las variables, sobretodo las ultimas 9.
  - Hacer de la variable "state_name" un dummie para su uso en la regresion lineal.
   - ¿Qué states son los mas influyentes? A modo de quedarse con la menor cantidad de dummies posible.
  - Visualizar la cantidad de casos en los cuales se puede confiar en la informacion de la variable "description" para obtener datos sobre "rooms"
- Revision ortografica

- El archivo 2 ahora contiene un contador de ambientes (o cuartos, o dormitorios), actualmente genera 13 075 entradas de "title" y 33 370 de "description", todavia hay que hacerle mejorías, pero suponiendo que los datos son correctos, estaría dejando a rooms, con un aproximado de 40 000 registros únicos.

  
- Estimar un modelo de regresión lineal que realice predicciones para el precio por metro cuadrado.
  - ¿Que es exactamente un modelo de regresion lineal?
  - ¿Como implementar uno en el codigo?
  - ¿Cúales son los requisitos para su implementacion?

## **Puntos de vista generales:**

1-Pre_Analisis.ipynb - Analisis preliminar del proceso de limpieza.

2-Modificacion_de_datos.ipynb -Re-estabilizacion de los valores para fines del paso 3.

3-Tasado_lineal.ipynb - Implementación de un modelo de regresion lineal para el tasado de propiedades.

![alt text](https://github.com/Villamaru/stunning-octo-waffle/blob/master/imagenes/heatmap.png "Heatmap")

![alt text](https://github.com/Villamaru/stunning-octo-waffle/blob/master/imagenes/Tasado_lineal_1.png "Tasado lineal version 1")

## **Objetivos 1:**
 
- Efectuar una limpieza del dataset provisto. Particularmente, deberá diseñar estrategias para lidiar con los datos perdidos en ciertas variables. 

- Realizar un análisis descriptivo de las principales variables. 

- Crear nuevas columnas a partir de las características dadas que puedan tener valor predictivo. 
 


  

## **Objetivos 2:**

- Estimar un modelo de regresión lineal que realice predicciones para el precio por metro cuadrado.

- Usar cross-validation para validar el modelo. Deberá prestar cierta atención a la estructura espacial de los precios.

- Aplicar regularización a modelos lineales pueden hacerlo para obtener un puntaje adicional. La idea es la siguiente: estimar una regresión ridge y una LASSO sobre el dataset. Para ello deberán usar cross-validation para tunear el parámetro de regularización que maximiza R2 en tu test set. ¿Cómo son las performances entre los modelos regularizados y no regularizado? ¿Cuál funciona mejor? ¿Qué “hace” una regresión ridge? ¿Y una LASSO? ¿Qué diferencias hay con la regresión lineal sin regularizar?

- Seleccionar mediante muestreo aleatorio simple una submuestra de 100 propiedades. Este será su portafolio de departamentos. En base al mejor modelo que haya encontrado determine cuáles de los departamentos, tanto en su portafolio como fuera de él, se encuentran sobrevaluados o subvaluados y en qué magnitud.

- Teniendo en cuenta que podría comprar y vender propiedades al precio de mercado, omitamos costos de transacción, con un capital inicial igual al valor de mercado de las propiedades en su portafolio. ¿Cuál es el mejor portafolio de propiedades que podría comprar?
  - Utilizar el modelo para ver cuales son las propiedades subvaluadas con respecto al precio tasado por el modelo, entendiendo que el modelo funciona correctamente.

## **notas:**

De la clase de Regresion lineal, se concluyo que: La escala de las características es irrelevante para los modelos de regresión lineal. Al cambiar la escala, simplemente cambiamos nuestra interpretación de los coeficientes.
