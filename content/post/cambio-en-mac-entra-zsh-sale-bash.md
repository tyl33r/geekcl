+++
author = "Arturo"
date = 2013-09-23T10:15:52Z
description = ""
draft = false
slug = "cambio-en-mac-entra-zsh-sale-bash"
tags = ["mac", "zsh", "bash", "oh my zsh", "shell"]
title = "Cambio en Mac: entra Zsh, sale Bash"

+++

Para un usuario de mi nivel, creo que más bien básico, la simplicidad a la hora de configurar y lograr lo que necesito se anteponen a veces a lo extendido o robusta que puede ser una herramienta. Es por esto que he decidido **cambiar Bash por Zsh**, principalmente gracias a *Oh My Zsh*, un complemento que hace de esta shell una herramienta casi llegar y usar sin estar recurriendo a complicadas configuraciones.

**Zsh** recién instalado ya viene con autocompletado inteligente, corrección de comandos, alias de comandos, gracias a oh my zsh existe la posibilidad de usar temas, plugins. Al contrario de Bash que hay que configurarlo todo a mano.

*Después de terminar este post te recomiendo que leas [Instalación y personalización de iTerm 2](/instalar-personalizar-iterm-2/ "Instalar y personalizar iTerm 2")*

Primero debemos instalar las "Command Line Tools", luego "<a href="http://brew.sh/index_es.html" target="_blank">Homebrew</a>", después "<a href="http://www.zsh.org/" target="_blank">Zsh</a>" y por último "<a href="https://github.com/robbyrussell/oh-my-zsh" target="_blank">Oh My Zsh</a>".

### Paso 1: Instalar Command Line Tools para OS X Mountain Lion

* Ingresa a [https://developer.apple.com/downloads](https://developer.apple.com/downloads) utilizando tu Apple ID.

* Luego en el cuadro de búsqueda pon "command line tools"

* Dentro de la opciones de descarga, asegurate de descargar la última versión.

* Instala


### Paso 2: Instalar Homebrew
* El maravilloso gestor de paquetes, que sirve para instalar desde la línea de comandos cientos de programas libres que no vienen instalados.
```ruby
$ ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"
```

* Luego queda ejecutar "brew doctor" para verificar que todo esté bien.
```
$ brew doctor
```

### Paso 3: Ahora sí instalamos Zsh
* Actualizamos la lista de paquetes.
```
$ brew update
```

* Instalamos!
```
$ brew install zsh
```

* Hacemos que Zsh sea nuestra shell por defecto, tecleamos en la terminal:
```
$ chsh -s /usr/local/bin/zsh
```

### Paso 4: Ahora vitaminizamos Zsh con Oh My Zsh
* Instalación mediante curl en la línea de comandos.
```
$ curl -L github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh
```

* Para mayor personalización, con tu editor de texto favorito puedes editar el archivo .zshrc ubicado en tu ~ (Users/usuario/). En este archivo puedes agregar plugins, cambiar temas, crear alias, etc.

*Te recomiendo leas [Instalación y personalización de iTerm 2](/instalar-personalizar-iterm-2/ "Instalar y personalizar iTerm 2").*

Te dejo a continuación un video que deja bien claro todas las mejoras que trae Zsh + OMZ.

<iframe width="560" height="315" src="https://www.youtube.com/embed/kuR0irUO9ak" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

### Links que aportaron a este post:

* [Moncef Belyamani](https://www.moncefbelyamani.com/how-to-install-xcode-homebrew-git-rvm-ruby-on-mac/)

* Un archivo de configuración ejemplo bastante completo [.zshrc](https://github.com/thomasfrivold/mydotfiles)
