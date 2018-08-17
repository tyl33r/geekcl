+++
author = "Arturo"
date = 2013-09-16T10:35:28Z
description = ""
draft = false
slug = "instalar-personalizar-iterm-2"
tags = ["mac", "iterm2", "menlo", "zsh"]
title = "Mac: Instalar y personalizar iTerm 2"

+++


![iterm2 mac](/content/images/2016/06/iterm21.jpg)<br />
<cite>Instalar y cambiar la apariencia de iTerm2</cite>.

El viejuno y sin gracia terminal de Mac OS X es la única posibilidad que existe como emulador de consolas, y ofrece a mi parecer pocas opciones de personalización. Gracias al bueno de George Nachman existe una mejor opción llamada iTerm 2, la que ofrece un montón de mejoras con respecto a la opción por defecto.

## Mejoras:

* División de paneles tanto en forma vertical como horizontal.
* Temas
* El uso de Hotkeys o tecla de acceso rápido a la consola.
* Búsqueda
* Autocompletado
* Copiar usando el mouse
* Historial de Pegar
* Repetición instantánea
* Pantalla completa
* Multilenguaje
* Uso de exposé para las pestañas, etc, etc.


Todas las características salen correctamente explicadas y con mucho [mayor detalle aquí](https://www.iterm2.com/#/section/features).

### Instalación en Mac OS X.
Nada más fácil que descargarlo desde su [página oficial](https://www.iterm2.com/#/section/downloads)

### Personalizando iTerm 2.
El uso de temas y fuentes personalizadas hace que iTerm 2 se adapte mucho mejor a nuestras necesidades, sin realizar complicadas configuraciones.

La personalización más importante que yo recomiendo es el uso de los temas [Solarized Dark o Salarized Light](https://code.google.com/p/iterm2/wiki/ColorGallery), ambos disponibles para descargar.

* Una vez descargados anda a:

*iTerm>Preferences>Profiles>Colors>Load Presets>Import...*

y selecciona el tema que descargaste.

* Además de cambiar la fuente por defecto a Menlo. En iTerm 2 vé a:
*iTerm>Preferences>Profiles>Text*

En Regular Font y en Non ASCII Font selecciona Menlo con tamaño 14pt y Anti-aliased.

* Luego para mayor personalización puedes cambiar el cursor por efecto en:

*iTerm>Preferences>Profiles>Text*

Cursor y seleccionar "Underline" con "Blinking Cursor"

* Para el soporte de colores ir a:
*iTerm>Preferences>Profiles>Terminal*

Seleccionar en "Report Terminal Type" "xterm-256color".

Con estas personalizaciones el aspecto de iTerm2 realmente se vuelve más agradable, ya que la legibilidad en la consola aumenta gracias al tema Solarized y a la fuente Menlo.


![](/content/images/2016/06/iterm2-menlo-zsh-1.jpg)<br />
<cite>Personalización: iTerm2 + Menlo + Zsh</cite>.

>Dale una oportunidad a iTerm 2, verás que te va a gustar, más aún cuando aprendas a usar las múltiples posibilidades de configuración.
