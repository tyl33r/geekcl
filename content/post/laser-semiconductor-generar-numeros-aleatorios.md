+++
author = "Arturo"
date = 2008-12-29T14:36:53Z
description = ""
draft = false
tags = ["láser", "aleatoriedad", "números", "entropía"]
slug = "laser-semiconductor-generar-numeros-aleatorios"
title = "Láser semiconductor para generar números aleatorios"

+++

Los números aleatorios son aquellos que se producen derivados de algún proceso físico natural o artificial que no se puede predecir o sea que no responde a ningún patrón. Las principales fuentes de entropía utilizadas para generar aleatoriedad en la generación de números, son los procesos físicos como la [desintregacion radioactiva](http://www.sc.ehu.es/sbweb/fisica/cuantica/desintegracion/radio.htm) o el [ruido blanco](https://es.wikipedia.org/wiki/Ruido_blanco). Ambos con una desventaja, la cual es su **baja tasa de generación de números aleatorios**, lo que dificulta el trabajo a los potentes computadores que necesitan procesar gran cantidad de datos rápidamente. Los **números aleatorios de calidad** son utilizados en variadas áreas, tales como la criptografía, simuladores financieros, equipos de diseño gráfico, etc.

![ruido blanco](/images/import/40-PSD-ruido-blanco.png)<br />
<cite>El PSD debería ser perfectamente "plana" pero se analizó un registro de señal finito. A mayor tiempo de registro más recta tiende a ser el PSD del ruido blanco (vía [Wikipedia](https://es.wikipedia.org/wiki/Ruido_blanco#/media/File:White_noise_pwelch.png)).</cite>

Un equipo de científicos Japoneses de la [Takushoku University](https://language.takushoku-u.ac.jp/english/), [Saitama University](http://en.saitama-u.ac.jp/), y [NTT Corporation](http://www.ntt.co.jp/index_e.html), dice haber logrado generar números aleatorios a través de [láseres semiconductores](http://users.df.uba.ar/acha/Lab5/Lasersemicond.pdf) (véase también [Semiconductor](https://es.wikipedia.org/wiki/Semiconductor), [Diodo Láser](https://es.wikipedia.org/wiki/Diodo_l%C3%A1ser)), a tasas bastante altas (1,7 Gbps), diez (10) veces más rápido que el fenómeno físico que lo sigue.

![laser diodo](/images/import/39-laser-diodo.gif)<br />
<cite>Fotografía de Diodos Láseres un tipo de Láser Semiconductor (vía [U. Columbia](http://www.aml.engineering.columbia.edu/ntm/level2/ch02/html/l2c02s12.html)).</cite>

El experimento se llevó a cabo volviendo a introducir parte de la luz láser reflejada, formando un circuito semi cerrado. Esto induce al caos ya que la intensidad de la luz oscila fuertemente, y se obtienen señales electromagnéticas muy complejas que abarcan una amplia gama de frecuencia. Para transformar la gama de frecuencia en números, se utiliza un *fotodetector* (detector de luz) que está conectado a un convertidor *análogo a digital*, el que se encarga de transformar en **números binarios aleatorios** las mediciones de intensidad de luz detectadas por el fotodetector.
