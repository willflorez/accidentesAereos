<h1 align="center"> ACCIDENTES AEREOS OACI  </h1>


<p align="center">
<img src=https://th.bing.com/th/id/R.5554814c2a1e3fcae2fd53f3ad1c81c2?rik=g29HUUEaqtLZ0g&riu=http%3a%2f%2f3.bp.blogspot.com%2f-7bc3GooJBHg%2fTVRooDxkVOI%2fAAAAAAAAABI%2fohZzSQy5MBk%2fw1200-h630-p-k-no-nu%2fflight815-des.jpg&ehk=gr%2brjd9uxyZS48qM4lNQLViZpmaA8s%2fyWjvJVggfpAI%3d&risl=&pid=ImgRaw&r=0
</p>


# INDICE 
<!-- TABLA DE CONTENIDO -->
<details>
  <summary>TABLA DE CONTENIDO</summary>
  <ol>  
    <li><a href="#INTRODUCCION">INTRODUCCION</a></li>
    <li><a href="#OBJETIVO">OBJETIVO</a></li>
    <li><a href="#CONJUNTO-DE-TECNOLOGIAS">CONJUNTO DE TECNOLOGIAS</a></li>
    <li><a href="#EDA">EDA</a></li>
    <li><a href="#KPI1">KPI 1</a></li>
    <li><a href="#KPI2">KPI 2</a></li>
    <li><a href="#CONCLUSIONES">CONCLUSIONES</a></li>
  </ol>
</details>



# INTRODUCCION.

El presente proyecto analiza el conjunto de datos de la Organización de Aviación Civil Internacional (OACI),
que entrega información acerca de accidentes aéreos presentados a nivel mundial entre los años 1908 y 2021. En el análisis exploratorio de datos se logra conocer, entre otras cosas, el país con mas número de accidentes, el fabricante de aviones menos afortunado, las rutas de vuelo mas siniestradas, aparece también que las pruebas de vuelo, las demostraciones y las operaciones militares aportan un gran número de accidentes.

# OBJETIVO.

1. Analizar a profundidad el conjunto de datos para obtener información relevante acerca de los accidentes.

2. Entender el mensaje que los datos estan entregando, basado en la interpretación de las variables numéricas y categóricas y la relación entre ellas.

3. Realizar un tablero de control que presente la información analizada de manera clara y concisa, con una historia coherente y conclusiones acertadas.

4. Graficar en el tablero de control dos indicadores de gestión, el propuesto en el proyecto y el decidido por mi, reducción del 10% de la tasa de fallecimientos de tripulantes (propuesto en el proyecto) y de pasajeros (propuesto por el autor) respecto de la decada anterior.

5. Construir un README detallado con el fin que el lector comprenda los puntos anteriores y sea suficiente para exponer el trabajo realizado por mi.

# CONJUNTO DE TECNOLOGIAS.

![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white)
![PowerBI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=Power%20BI&logoColor=white)

# EDA.

1. HISTOGRAMA.

En el desarrollo del análisis exploratorio de datos, es inevitable no caer en la tentación, de empezar por conocer el comportamiento de la cantidad de fallecidos de tripulantes y pasajeros y el número de accidentes en los que se han visto involucrados. Y es que el conjunto de datos es precisamente sobre accidentes aéreos y fallecidos. Escrito esto la imagen a continuación:

![Alt text](output.png)

Evidentemente la realidad enseña que en un avión viajan mas pasajeros que tripulantes y las gráficas muestran que es desproporcionado el número de víctimas entre el primero y el segundo grupo, en el conjunto de datos estudiado. En pocos casos los pasajeros superan las 300 victimas en un siniestro, ha no ser que ocurra una tragedia de tipo terrorista (ataques a EEUU) o una desaparición durante un vuelo (Malasya Airlines).

2. DIAGRAMA DE CAJA.

Este diagrama tiene en cuenta las tasas de fallecimiento y su respectiva distribución, está mas agrupada la tasa que corresponde a los tripulantes fallecidos, normalmente el número de tripulantes es el mismo vuelo a vuelo, no así el de pasajeros.

![Alt text](diagramacaja.png)

El valor por fuera de los bigotes corresponde a una disminución significativa de la tasa de fallecimiento de los tripulantes.

3. GRAFICO DE DENSIDAD.

La cantidad de muertes reportadas por accidentes aéreos muestra un número de fallecidos inferior a 10 por evento,una de las razones es la baja frecuencia de vuelos al inicio de la industria, otra, es que los viajes en avión hoy por hoy son el medio de transporte mas confiable y seguro que hay, gracias al avance de la ingeniería aeronaútica.

![Alt text](DENSIDAD.png)

4. GRAFICO DE PARES.


La diagonal principal de la gráfica dice que la variable númerica de tripulantes fallecidos no es directamente proporcional a la variable número de muertes (los tripulantes no aportan gran número de vítimas) al contrario que la cantidad de pasajeros fallecidos, dicho de otra manera la mayor cantidad de fallecimientos totales son de pasajeros. Este resultado es lógico y esperado, en las aeronaves van más pasajeros que tripulantes.
Ahora bien, no hay relación entre pasajeros y tripulantes, son grupos excluyentes la misma persona no clasifica al mismo tiempo en los dos grupos de estudio.

![Alt text](PARES.png)

5. DIAGRAMA DE BARRAS.

La aerolínea rusa Aeroflot es la que mas veces se repite en el conjunto de datos analizado, tambien las fuerzas militares de EEUU, cuando de analizar la columna de operadores se trata. En esa misma columna aparecen actividades como el entrenamineto de vuelo y el turismo como las principales acciones cuando ocurren los siniestros.

![Alt text](BARRAS.png)

6.  GRAFICO DE PASTEL.


La aeronave de la constructora Douglas es la que más veces aparece en el análisis del conjunto de datos, es de origen estadounidense, se puede creer que durante las pruebas de sus aviones en suelo norteamericano se presentaron muchos accidentes (EEUU es el país con mas números de siniestros). Dato: Boeing también es estadounidense.

![Alt text](PASTEL.png)





hallazgos
Data Analyst


Evaluar la disminución de un 10% la tasa de fatalidad de la tripulación en los últimos 10 años, comparado a la década anterior.

Definimos la tasa de fatalidad de la tripulación como el número total de tripulantes fallecidos en los accidentes registrados en la década a considerar, dividido en la cantidad total de accidentes aéreos ocurridos en este período de tiempo. Su fórmula es (Suma total de fallecidos en el período de tiempo / Suma total de accidentes en el período de tiempo).