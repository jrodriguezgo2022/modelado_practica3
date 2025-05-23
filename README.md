# modelado_practica3

![grafica_1](assets/imagen_apartado5.png)

En la anterior gráfica podemos ver cómo avanza la posición de los 6 joints de las ruedas respecto al tiempo. Observamos que los joints del lado izquierdo y los del lado derecho son simétricos respecto a 0. Esto se debe a que los joints están colocados en diferentes direcciones; por ende, podemos ver que uno es positivo y el otro negativo. Viendo la gráfica, también podemos asumir que el movimiento duró alrededor de 5 segundos (desde el segundo 9 al 14). A partir de ahí, se estabiliza y volvemos a ver un nuevo pequeño movimiento entre los segundos 18 y 20. Estos dos movimientos se deben a que, en primer lugar, hice un movimiento de aproximación al cubo y, tras revisar si su colocación era correcta, corregí un poco la posición, dando así explicación a ese segundo movimiento.

![grafica_2](assets/imagen_apartado6.png)

En la anterior gráfica vemos los datos obtenidos de la IMU. En este caso, están graficadas tanto la aceleración en x como en y. En esta gráfica podemos confirmar el doble movimiento que visualizábamos en la primera imagen, siendo en esta más clara la diferenciación entre ambos.

![grafica_3](assets/imagen_apartado7.png)
![grafica_aux](assets/auxiliar.png)

Por último, las dos gráficas anteriores se tratan tanto del valor del g-parcial como del esfuerzo de cada joint por separado. En primer lugar, podemos ver un primer gran esfuerzo correspondiente a la bajada del brazo, así como su correspondiente movimiento para agarrar el cubo. A continuación, vemos una bajada en el esfuerzo seguida de una gran subida. Este esfuerzo refleja el movimiento necesario para llevar el cubo hasta su posición hold. Esta posición está en línea con respecto a la de la recogida con el cubo. El siguiente movimiento visible es el ocurrido tras el periodo de estabilización (tiempo que se tarda en introducir una nueva instrucción en RViz). Si miramos la gráfica auxiliar, podemos ver que participan los joints 1, 2 y 3. Esto nos da a entender que se trata del movimiento realizado desde la posición de hold hasta la posición en la que dejaremos el cubo. Por último, en el momento en que ocurre la pequeña bajada localizada al final de la gráfica, si nos fijamos en la gráfica auxiliar, se observa que ocurre en el mismo instante en que la pinza se abre y, por tanto, se da por finalizado el movimiento de pick and place.
