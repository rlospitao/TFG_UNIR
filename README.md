<h1> Predicción de las precipitaciones en Madrid con Redes Neuronales </h1>
<h2 align="center"> Trabajo Fin de Estudios del Curso de Adaptación al Grado de Ingeniería Informática</h2>


<h3 align="center">  Universidad Internacional de La Rioja <br> Escuela Superior de Ingeniería y Tecnología </h3>
<p align="center"> Ruth Lospitao Ruiz, Julio 2022


<p><b>Resumen:</b> La escasez de precipitaciones puede suponer una catástrofe humana y económica de gran impacto. Este trabajo consiste en proponer una posible solución, mediante la predicción de las precipitaciones en la comunidad de Madrid. Para ello, se descargan datos climatológicos de la Agencia Española de Meteorología, los cuales serán tratados para utilizarlos en diferentes modelos predictivos basados en las redes neuronales recurrentes.

<p><b>Palabras clave: </b>Predicción de precipitaciones, datos climatológicos, redes neuronales recurrentes, modelos predictivos, aprendizaje profundo
<p>
<p>
Este repositorio contiene el código correspondiente al trabajo de <i>"Predicción de las precipitaciones en Madrid con Redes Neuronales"</i>. Se trata de cuatro libros notebooks desarrollados con Jupyter. Para poder ejecutar los notebooks, se recomienda abrir el repositorio desde Google Collaborate ya que así se dispone del entorno necesario para su ejecución.
<p>Para la realización de este proyecto se han llevado a cabo las siguientes tareas:
<ol>
  <li><b> Recopilación y extracción de los datos climatológicos</b> de la Comunidad de Madrid. Para ello, se utilizará la fuente abierta de <a href="https://opendata.aemet.es/" target="_blank">OpenData AEMET</a>. </li>
 <li><b>Transformación y preparación de los datos </b>a los formatos necesarios para su análisis. Para ello, se trabajará con notebooks de Jupyter en lenguaje de programación Python.</li>
<li><b>Selección de las variables climáticas más adecuadas</b> para el modelo de predicción a través de una matriz de correlación.</li>
<li><b>Desarrollo y evaluación de diferentes modelos predictivos</b>. Se desarrollarán en lenguaje de programación Python, utilizando librerías de Aprendizaje Profundo.</li>
</ol>
<p> El proyecto, consta de los siguientes libros Jupyter: 

* <i> 01a-extract_data_all_stations.ipynb</i>. <p>Notebook que se conecta a OpenData AEMET para descargar toda la información climatológica mensual de todas las estaciones de la Comunidad de Madrid, desde el año 1960 hasta 2022. La información se almacena en <i>data\data_all_stations_from1960.csv</i>
* <i>01b-extract_data_3195.ipynb</i>.<p>Notebook que se conecta a OpenData AEMET para descargar los datos climatológicos mensuales de la estación de medición de Retiro, desde 1893 hasta 2022. La información obtenida se almacena en <i>data\data_3195.csv</i> Finalmente, serán los datos de la estación de Retiro los que se utilicen para este estudio; ya que es la estación con más datos y puede ser representativa de Madrid.
* <i>02-clean_data_3195.ipynb</i>.<p>Notebook que realiza la exploración y limpieza de los datos climatológicos de la estación de Retiro. Para ello, se transformaran variables, se eliminaran las que no sean necesarias y se corregirán valores atípicos y NaN. El resultadp  se almacena en <i>data\clean_3195.csv</i>
* <i>03-predective_models.ipynb</i>.<p>A partir del conjunto de datos limpios, se procederá a prepararlos en series temporales y diseñar diferentes modelos predictivos basados en redes neuronales para compararlos. La predicción se almacena en <i>data\prediction_precipitation_3195.xlsx</i>
* <i>04-calculate_spi.ipynb</i>.<p>Notebook que, a partir del fichero demostración <i>data\rainfall_3195.xlsx</i> (que almacena posibles predicciones), calcula el índice SPI para determinar si hay o no sequía.

<p>Para su desarrollo, se ha empleado un entorno en Anaconda Navigator con las siguientes librerías: ´matplotlib, missingno, seaborn,Keras 2.6 y TensorFlow 2´

<p>Nota: Para su ejecución, se recomienda buscar desde Google Collaborate este repositorio, teniendo en cuenta que la lectura de los ficheros se realiza desde un directorio (previamente creado) con el nombre <i>data</i>. Otra opción, sería subir los ficheros .csv al directorio <i>sample_data</i>de Google Collaborare y modificar el path.

  <p>Para cualquier duda o consulta sobre este trabajo, puede ponerse en contacto con el autor en rlospitao@gmail.com
  
  <p>10 de Julio 2022
