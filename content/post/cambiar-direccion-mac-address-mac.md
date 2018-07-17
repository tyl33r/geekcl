+++
author = "Arturo"
date = 2009-07-21T02:21:50Z
description = ""
draft = false
slug = "cambiar-direccion-mac-address-mac"
title = "Resetear la «Dirección MAC» de tu Mac"

+++

<p>Mac OS X es Unix; algo así cómo <a href="http://cactusdigital.net/">Linux</a> pero comercial y de código cerrado. Los usuarios de <a href="http://es.wikipedia.org/wiki/Mac">Mac</a> tienen todo el potencial de un sistema operativo que fue de algunos, más que una simple fuente de inspiración.</p>

<p>Aprovechando la línea de comandos (algún usuario mac la conoce? ;) ), se puede resetear de forma aleatoria la <strong><a href="http://es.wikipedia.org/wiki/Direcci%C3%B3n_MAC">Dirección MAC</a></strong> o <strong>MAC Address</strong> de tu conexión inalámbrica de internet, algo que puede servirte para que sea más difícil encontrarte o identificarte antes de compartir archivos legales en la red BitTorrent.</p>

<code>ran=$(head /dev/urandom | md5sum); MAC=00:07:${ran:0:2}:${ran:3:2}:${ran:5:2}:${ran:7:2}; sudo ifconfig wlan0 down hw ether $MAC; sudo ifconfig wlan0 up; echo ifconfig wlan0:0</code><br />

[Vía - <a href="http://www.commandlinefu.com/commands/view/2678/resets-your-mac-to-a-random-mac-address-to-make-you-harder-to-find.">commandlinefu</a>].