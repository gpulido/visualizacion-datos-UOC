# Horizon Graph

![Alt text](./horizon.svg)

*El diagrama anterior ha sido realizado usando https://rawgraphs.io/*

## Descripcion

Es un tipo de gráfico basado en un gráfico de linea normal. Este gráfico se divide en un número determinado de bandas horizontales con la misma altura, cada una de las bandas se colorea con un color y a continuación se apilan todas las bandas para que partan desde el origen de coordenadas, de tal forma que se solapen los distintos colores correspondientes a los distintos valores. Si hay valores en el eje vertical negativos, también se dividen en bandas, se invierten y se apilan con los valores positivos. De esta forma se consigue reducir el tamaño vertical del diagrama al alto de una de las bandas manteniendo la misma información. Esto permite mostrar registros agrupados por una categoria con muchas clases en las que se dibuja un diagrama por cada clase en un espacio mucho mas reducido. Se suele usar para mostrar la evolución de una variable en el tiempo (que se suele usar para el eje X) para multitud de clases. Por ejemplo la variación del porcentaje de paro a lo largo del tiempo para cada uno de los países de la union europea. Es una representación que permite mostrar un valor cuantitativo (paro) a lo largo de otra variable cuantitativa (tiempo) clasificada por una variable cualitativa (pais). 


## Datos

Para la realización del gráfico se han usado los datos históricos de desempleo de europa, proporcionados por [eurostat](https://ec.europa.eu/eurostat/web/lfs/data/database?p_p_id=NavTreeportletprod_WAR_NavTreeportletprod_INSTANCE_IFjhoVbmPFHt&p_p_lifecycle=0&p_p_state=normal&p_p_mode=view)
Se han usando los datos mensuales desde 1983.

Se han filtrado y transformado calculando la media en cada uno de los meses y realizando la diferencia de cada pais con respecto a la media, para así poder tener datos positivos (en azul) y negativos (en rojo)

El fichero csv con los datos finales usados se encuentra [aqui](./data.csv) 

## Referencias

https://flowingdata.com/2015/07/02/changing-price-of-food-items-and-horizon-graphs/