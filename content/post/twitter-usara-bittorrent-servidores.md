+++
author = "Arturo"
date = 2010-02-19T08:29:39Z
description = ""
draft = false
slug = "twitter-usara-bittorrent-servidores"
title = "Twitter usará BitTorrent en sus servidores"

+++

<img class="aligncenter" src="http://geeksan.com/wp-content/uploads/import/193-twitter-bittorrent.jpg" alt="193-twitter-bittorrent.jpg" />

<a href="http://twitter.com/">Twitter</a> utilizará el protocolo de red <a href="http://es.wikipedia.org/wiki/BitTorrent_(protocolo)">BitTorrent</a> para distribuir de forma más eficiente entre sus servidores la gran cantidad de información que se genera segundo a segundo.

Por el límite auto impuesto de los 140 caracteres en la red social <strong>Twitter</strong>, a primera vista podría pensarse que la cantidad de información que se genera no es considerable, pero esto está muy lejos de la realidad, ya que los miles de servidores que integran la red gastan una gran cantidad de recursos para poder gestionar las actualizaciones que crean sus millones de usuarios.

Es aquí donde entra el protocolo de red p2p <strong>BitTorrent</strong>, el cual debido a su modo de funcionamiento será de gran ayuda para Twitter en la descongestión de sus redes internas. La idea central del proyecto, al contrario de lo que pasa normalmente cuando compartimos un archivo torrent, no busca utilizar el ancho de banda de sus usuarios, si no que con los miles de servidores que ya tiene twitter se formará un inmenso enjambre, el cual gracias a BitTorrent distribuirán de forma más rápida y eficiente la información. Habrá un servidor semilla (seeder) el cual se encargará de distribuir los datos a los otros cientos de servidores o pares (peer).

El proyecto tiene por nombre <a href="http://github.com/lg/murder"><strong>Murder</strong></a> y el encargado de implementarlo es el ingeniero de Twitter Larry Gadea (<a href="http://twitter.com/Lg">@Lg</a>), es una idea bajo licencia Apache de Software Libre de la cual cualquier persona que esté interesada puede beneficiarse o aportar.

El protocolo BitTorrent lamentablemente casi siempre se asocia a descargas ilegales, violación de los derechos de autor, la decadencia de la música y sus músicos, etcétera. Pero con estas implementaciones demuestra que mas haya del uso que se le dé habitualmente, estamos ante una <em>tecnología para redes bastante potente</em>.

[Vía - <a href="http://torrentfreak.com/twitter-uses-bittorrent-for-server-deployment-100210/">TorrentFreak</a>.]