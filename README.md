# w5-Visualization-project

En este proyecto de visualización he continuado con el proyecto de la semana pasada para sacar conclusiones que pueden sorprender a más de uno.De todos los datos obtenidos en dos CSVs he combinado algunos de ellos para tratar de explicar ciertos aspectos.

Primeramente he hecho un analisis general para luego tratar de hacerlo más especificamente.Para ello he usado Tableau ya que opino que me permitía una visualización más entendible.

El primer gráfico al que he intentado darle forma ha sido la combinación de la tasa de crimenes por estado. He podido sacar conclusiones que cuanto menos son curiosas
¿Como es posible que Alaska tenga la tasa de crimenes más alta de EEUU cuando no es el que más población tiene?

![image](https://user-images.githubusercontent.com/117199136/219949643-fd3d1d4f-398d-4ea9-ac1d-6dce576da3a8.png)

Después de haber investigado un poco se puede hacer suposiciones de ello. Por ejemplo, Alaska es un estado con altos indices de violencia doméstica. Esto puede derivarse de que la gente debido al clima y las pocas horas de luz pase más tiempo en casa y por tanto aumenten los conflictos, eso unido a que es un estado con una dispersion poblacional importante donde a muchos sitios solo se puede llegar en avioneta lo que hace que la cobertura estatal para poder atajar dichos delitos falle y por tanto puede ser una de las causas de dichas tasas.

Como segundo grafico he evaluado la evolución de la tasa de crimenes. 

![image](https://user-images.githubusercontent.com/117199136/219949898-6d8acf13-ddb5-4ce8-90d4-d470ce86ac88.png)
 
Como se puede observar en los últimos 30 años dichas tasas han descendido drasticamente.Para determinar que podría ser he analizado dos variables aleatoriamente que son los datos económicos y las tasas de alcoholemia. Respecto a las tasas de alcoholemia he de decir que EEUU tiene tasas incluso inferiores a Europa pero sus tasas de delicuencia son mucho mayores. Como en el anterior proyecto (donde realicé una matriz de correlación) se observa que las tasas de alcohelmia no son determinantes o en  caso de serlo son en un porcentaje menor y acotado a crimenes de baja evergadura como robos,asaltos.....pero rara vez a asesinatos u homicidios.

Respecto a los datos económicos(tomando en cuenta unos pocos) lo sorprendente es que en 1992 había una situación económica más boyante en EEUU que en el 2008(año de la crisis), lo que pasa es que las tasas de criminalidad son inversas.Para ilustrar esta inconcruencia me he ido a datos de 1992 de PIB y PIB per capita y los he comparado con los de 2008.

1992 crecimiento PIB--> 3.5%                             2008 crecimiento PIB--> 0.1%
     decrecimineto PIB/per capita--> -0.5%                    decrecimiento PIB/per capita--> -5.8%
     
     
En el tercer grafico he querido tratar de indagar si la renta por estado influye en la tasa de crimenes.
![image](https://user-images.githubusercontent.com/117199136/219951144-8938a552-ddad-44f5-87e6-aec4785c60d5.png)

Para ello he puesto el ejemplo de Maryland y Vermont. Como se puede comprobar aún Maryland siendo más rico tiene tasas de criminalidad mayores que Vermont, 399.9 vs 173.4. Por lo que deduzco que las tasas de criminalidad se deben a factores muchos más amplios que solo el nivel de riqueza.

Para el cuarto grafico he sacado la media de homicidios por cada estado en los últimos 10 años y me he fijado en dos estados.

![image](https://user-images.githubusercontent.com/117199136/219951604-0589f0fe-cf41-440e-9c7d-0f5fa4f9132e.png)

Son dos estados con caracteriticas muy similares respecto a población pero NO respecto a densidad de población. Nebraska:10 hab/km2  New-Hampshire:57 hab/km2 tasa homicidios--> Nebraska:51 // New-hampshire:18
Es probable que la dispersión geografica haga un efecto rebote a la hora de cometer crimenes además de que Nebraska es un estado eminentemente rural y por tanto habría que analizar más en detalle la variable de cuantos crimenes quedan resueltos o no, ya que eso puede dar la sensación de impunidad e incitar a la población a cometerlos de manera más frecuente.

En el quinto grafico comparo la media de robos de coches. he de decir que aqúi no he encontrado grandes sorpresas ya que he comparado dos estados con similitud en los habitantes y densidad poblacional como son Ohio y Pensilvania donde su correlación es bastante perfecta. Es decir, no hay ni por parte de uno ni por el otro datos estramboticos que puedan dar lugar a conclusiones sorprendentes.

Y por último he hecho un sexto grafico, exactamente un bloxpot.

![image](https://user-images.githubusercontent.com/117199136/219952170-519e9c7f-c7f4-4716-85bf-c0a9944e7fa9.png)

De este grafico he sacado ciertos analisis.

De primeras lo que observo es que la mediana está en un punto central por lo que estaríamos hablando de una posición simetrica. Otro de los puntos más destacados sería que hay tres valores que se distancian de manera considerable respecto al bigote superior por lo que vamos a analizar si dichos valores atipicos son valores que al final vamos a usar como muestra o si por el contrario vamos a descartarlos, puesto que lo que van hacer es sesgar nuestra distribución haciendo que la dispersión sea mayor.

Una vez hacemos un analisis general nos metemos en matería.
Q1 primer quartil está sobre los 50
Q3 tercer quartil está sobre los  210

Teniendo esto saco el IQR=Q1-Q3 dandome 160

Y para finalizar obtengo el rango al que estoy dispuesto que mis datos se dispersen para poder hacer una analisis más exahustivo Q3+1.5*IQR= 440

Por lo que los datos de los estados California ,Texas y Florida los voy a descatar debido a que están demasiado dispersos. Esto se puede deber a que la base de datos obtenida puede tener algún error de datos o calculo y por tanto habría que observarlo con más detenimiento o si por el contrario es Tableau que en su formato de comas ha generado datos completamente inusuales.

