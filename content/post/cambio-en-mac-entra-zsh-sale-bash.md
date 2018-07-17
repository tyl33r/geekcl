+++
author = "Arturo"
categories = ["mac", "zsh", "bash", "Oh My Zsh", "shell"]
date = 2013-09-23T10:15:52Z
description = ""
draft = false
slug = "cambio-en-mac-entra-zsh-sale-bash"
tags = ["mac", "zsh", "bash", "Oh My Zsh", "shell"]
title = "Cambio en Mac: entra Zsh, sale Bash"

+++

Para un usuario de mi nivel, creo que más bien básico, la simplicidad a la hora de configurar y lograr lo que necesito se anteponen a veces a lo extendido o robusta que puede ser una herramienta. Es por esto que he decidido **cambiar Bash por Zsh**, principalmente gracias a *Oh My Zsh*, un complemento que hace de esta shell una herramienta casi llegar y usar sin estar recurriendo a complicadas configuraciones.

**Zsh** recién instalado ya viene con autocompletado inteligente, corrección de comandos, alias de comandos, gracias oh my zsh existe la posibilidad de usar temas, plugins. Al contrario de Bash que hay que configurarlo todo a mano.

<em>Después de terminar este post te recomiendo que leas <a title="Instalar y personalizar iTerm 2" href="https://geek.cl/instalar-personalizar-iterm-2/">Instalación y personalización de iTerm 2.</a></em>

Primero debemos instalar las "Command Line Tools", luego "<a href="http://brew.sh/index_es.html" target="_blank">Homebrew</a>", después "<a href="http://www.zsh.org/" target="_blank">Zsh</a>" y por último "<a href="https://github.com/robbyrussell/oh-my-zsh" target="_blank">Oh My Zsh</a>".
### Paso 1: Instalar Command Line Tools para OS X Mountain Lion
<ul>
	<li>Ingresa a <a href="http://developer.apple.com/downloads">http://developer.apple.com/downloads</a> utilizando tu Apple ID.</li>
	<li>Luego en el cuadro de búsqueda pon "command line tools"</li>
	<li>Dentro de la opciones de descarga, asegurate de descargar la última versión (Mac OS X Mountain Lion for XCode).</li>
	<li>Instala</li>
</ul>
<h3>Paso 2: Instalar Homebrew</h3>
<ul>
<ul>
	<li>El maravilloso gestor de paquetes, que sirve para instalar desde la línea de comandos cientos de programas libres que no vienen instalados.</li>
</ul>
</ul>

<code>$ ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"</code>

<ul>
<li>Luego queda ejecutar "brew doctor" para verificar que todo esté bien.</li>

</ul>
<code>$ brew doctor</code>
<h3>Paso 3: Ahora sí instalamos Zsh</h3>
<ul>

	<li>Actualizamos la lista de paquetes.</li>
</ul>

<code>$ brew update</code>

<ul>
	<li>Instalamos!</li>
</ul>

<code>$ brew install zsh</code>
<ul>

	<li>Hacemos que Zsh sea nuestra shell por defecto, tecleamos en la terminal:</li>
</ul>

<code>$ chsh -s /usr/local/bin/zsh</code>

<h3>Paso 4: Ahora vitaminizamos Zsh con Oh My Zsh</h3>

<ul>
<li>Instalación mediante curl en la línea de comandos.</li>
</ul>

<code>$ curl -L github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh</code>

<ul>
<li>Para mayor personalización, con tu editor de texto favorito puedes editar el archivo .zshrc ubicado en tu ~ (Users/usuario/). En este archivo puedes agregar plugins, cambiar temas, crear alias, etc.</li>
</ul>

<em>Para mayor personalización te recomiendo que leas <a title="Instalar y personalizar iTerm 2" href="https://geek.cl/instalar-personalizar-iterm-2/">Instalación y personalización de iTerm 2.</a></em>

Te dejo a continuación un video que deja bien claro todas las mejoras que trae Zsh + OMZ.

<iframe src="//www.youtube-nocookie.com/embed/kuR0irUO9ak?rel=0" height="360" width="640" allowfullscreen="" frameborder="0"></iframe>

<strong><em>Links que aportaron a este post:</em></strong>

<ul>
<li><a href="http://www.moncefbelyamani.com/how-to-install-xcode-homebrew-git-rvm-ruby-on-mac/">Moncef Belyamani</a></li>

<li>Un archivo de configuración ejemplo bastante completo <a href="https://github.com/thomasfrivold/mydotfiles">.zshrc</a></li>
</ul>
