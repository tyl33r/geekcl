+++
author = "Arturo"
date = 2008-12-29T14:36:53Z
description = ""
draft = false
slug = "laser-semiconductor-generar-numeros-aleatorios"
title = "Láser semiconductor para generar números aleatorios"

+++

<p>Los números aleatorios son aquellos que se producen derivados de algún proceso físico natural o artificial que no se puede predecir o sea que no responde a ningún patrón. Las principales fuentes de entropía utilizadas para generar aleatoriedad en la generación de números, son los procesos físicos como la <a href="http://geek.cl/wp-content/uploads/2008/12/radio_num.xhtml">desintregacion radioactiva</a> o el <a href="http://geek.cl/wp-content/uploads/2008/12/Ruido_blanco">ruido blanco</a>.  Ambos con una desventaja, que es su <b>baja tasa de generación de números aleatorios</b>, lo que dificulta el trabajo a los potentes computadores que necesitan procesar gran cantidad de datos rápidamente. Los <strong>números aleatorios de calidad</strong> son utilizados en variadas áreas, tales como la criptografía, simuladores financieros, equipos de diseño gráfico, etc.</p> 

<p align="center"><img src="http://geeksan.com/wp-content/uploads/import/40-PSD-ruido-blanco.png" alt="40-PSD-ruido-blanco.png" /><br /><cite>El PSD debería ser perfectamente "plana" pero se analizó un registro de señal finito. A mayor tiempo de registro más recta tiende a ser el PSD del ruido blanco (vía <a href="http://geek.cl/wp-content/uploads/2008/12/Archivo:White_noise_pwelch.png">Wikipedia</a>).</cite></p>

<p>Un equipo de científicos Japoneses de la <a href="http://geek.cl/wp-content/uploads/2008/12/index.html">Takushoku University</a>, <a href="http://geek.cl/wp-content/uploads/2008/12/english">Saitama University</a>, y <a href="http://geek.cl/wp-content/uploads/2008/12/index_e.html">NTT Corporation</a>, dice haber logrado generar números aleatorios a través de <a href="http://www.mrl.columbia.edu/ntm/level2/ch02/html/l2c02s12.html">láseres semiconductores</a> (véase también <a href="http://geek.cl/wp-content/uploads/2008/12/Semiconductor">Semiconductor</a>, <a href="http://geek.cl/wp-content/uploads/2008/12/Diodo_l%C3%A1ser">Diodo Láser</a>), a tasas bastante altas (1,7 Gbps), diez (10) veces más rápido que el fenómeno físico que lo sigue.</p> 

<p align="center"><img src="http://geeksan.com/wp-content/uploads/import/39-laser-diodo.gif" alt="39-laser-diodo.gif" /><br /><cite>Fotografía de Diodos Láseres un tipo de Láser Semiconductor (vía <a href="http://www.mrl.columbia.edu/ntm/level2/ch02/html/l2c02s12.html">U. Columbia</a>).</cite></p>

<p>El experimento se llevó a cabo volviendo a introducir parte de la luz láser reflejada, formando un circuito semi cerrado. Esto induce al caos ya que la intensidad de la luz oscila fuertemente, y se obtienen señales electromagnéticas muy complejas que abarcan una amplia gama de frecuencia. Para transformar la gama de frecuencia en números, se utiliza un<i> fotodetector</i> (detector de luz) que está conectado a un convertidor <i>análogo a digital</i>, el que se encarga de transformar en <strong>números binarios aleatorios</strong> las mediciones de intensidad de luz detectadas por el fotodetector.</p>