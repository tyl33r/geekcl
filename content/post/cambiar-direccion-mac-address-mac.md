+++
author = "Arturo"
date = 2009-07-21T02:21:50Z
description = ""
tags = ["mac", "mac adress", "os x", "apple"]
draft = false
slug = "cambiar-direccion-mac-address-mac"
title = "Resetear la «Dirección MAC» de tu Mac"

+++

Mac OS X es Unix; algo así cómo Linux pero comercial y de código cerrado. Los usuarios de [Mac](https://es.wikipedia.org/wiki/Mac) tienen todo el potencial de un sistema operativo que fue para algunos, más que una simple fuente de inspiración.

Aprovechando la línea de comandos (algún usuario mac la conoce? ;)), se puede resetear de forma aleatoria la [Dirección MAC](https://es.wikipedia.org/wiki/Direcci%C3%B3n_MAC) o **MAC Address** de tu conexión inalámbrica de internet, algo que puede servirte para que sea más difícil encontrarte o identificarte antes de compartir archivos *legales* en la red BitTorrent.

'''
ran=$(head /dev/urandom | md5sum); MAC=00:07:${ran:0:2}:${ran:3:2}:${ran:5:2}:${ran:7:2}; sudo ifconfig wlan0 down hw ether $MAC; sudo ifconfig wlan0 up; echo ifconfig wlan0:0
'''

[Vía - [commandlinefu](https://www.commandlinefu.com/commands/view/2678/resets-your-mac-to-a-random-mac-address-to-make-you-harder-to-find)].
