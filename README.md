# Movie-Recommendation-System
This repository contains the solution to my Final Project at IT Academy by Barcelona Activa.  
My name is [Guillermo Seoane](https://www.linkedin.com/in/guilleseoane/) and I'm a **#DataScience** student.

## 📚 Archives:
In the repository you can find:
* **Exploratory_analysis** of the data,that allows you to understand it better and find insights (ex: flights per month, most used routes, etc.) based on "Mapping Destination Countries". [Download 'Mapping Destination Countries'](https://github.com/datagseoane/Vueling-Tech-Hack/blob/main/data/encode_countries.json)
* **Algorithm:** model used for prediction.
* **Graph**: 
* A **presentation.pdf** explaining how I have reach the solution

## 🦾 Dataset Dictionary:
Las principales variables en el conjunto de datos de MovieLens son las siguientes:

* **userId:** un identificador único para cada usuario que ha calificado películas en el conjunto de datos.
* **movieId:** un identificador único para cada película en el conjunto de datos.
* **rating:** una calificación numérica del 1 al 5 que el usuario dio a la película.
* **timestamp:** la fecha en que el usuario calificó la película.
* **title:** el título de la película.
* **Genre:** el género de la película, como comedia, drama o acción.

## Objetivos:
El objetivo principal de este proyecto es desarrollar un algoritmo de recomendación de películas que pueda utilizar el conjunto de datos de MovieLens para hacer recomendaciones personalizadas a los usuarios. Para lograr este objetivo, se han definido los siguientes objetivos específicos:
* Explorar y entender el conjunto de datos de MovieLens.
* Identificar patrones y tendencias en los datos que puedan utilizarse para hacer recomendaciones personalizadas.
* Desarrollar y probar dos métodos de recomendación diferentes: similitud de coseno y coeficiente de correlación de Pearson.
* Utilizar Gephi para la visualización y análisis de grafos para entender mejor la estructura de la red de usuarios y películas en el conjunto de datos.

## Methodology:
Se han desarrollado dos métodos de recomendación diferentes para este proyecto: similitud de coseno y coeficiente de correlación de Pearson.

#### 1. Similitud de Coseno: 
Este método utiliza la similitud de coseno para medir la similitud entre dos vectores de calificación de películas. Para cada usuario, se calcula la similitud de coseno con todos los demás usuarios en el conjunto de datos. A continuación, se seleccionan los usuarios con las mayores similitudes de coseno y se recomiendan las películas que han calificado positivamente pero que el usuario aún no ha visto.

#### 2. Coeficiente de Correlación de Pearson: 
Este método utiliza el coeficiente de correlación de Pearson para medir la similitud entre dos vectores de calificación de películas. Para cada usuario, se calcula el coeficiente de correlación de Pearson con todos los demás usuarios en el conjunto de datos. A continuación, se seleccionan los usuarios con los coeficientes de correlación más altos y se recomiendan las películas que han calificado positivamente pero que el usuario aún no ha visto.
Para ambos métodos, se ha utilizado una técnica de filtrado colaborativo, que se basa en la idea de que los usuarios con gustos similares tienden a calificar las mismas películas de manera similar. Estos métodos de recomendación no requieren información adicional sobre las películas o los usuarios, como su género o edad.

