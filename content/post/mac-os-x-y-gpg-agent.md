+++
author = "Arturo"
categories = ["zsh", "pass", "gnupg", "gpg", "iterm2", "mac os x"]
date = 2014-12-27T19:11:20Z
description = ""
draft = false
slug = "mac-os-x-y-gpg-agent"
tags = ["zsh", "pass", "gnupg", "gpg", "iterm2", "mac os x"]
title = "Mac OS X, gpg-agent y ZSH"

+++

![gpg-agent os x yosemite](/content/images/2014/12/logo-gnupg.png)

Que sirva como una nota para quien se le presente el mismo problema y no pierda tanto tiempo buceando la red en busca de la solución. **gpg-agent** es el programa encargado de evitar tener que estar ingresando la contraseña continuamente, una vez que ingreso la contraseña maestra de **gpg**, gpg-agent se encarga de *almacenarla* y no volver a solicitarla después de un determinado tiempo.

##Mac OS X + gpg-agent + ZSH y pass
No voy a explicar sobre la instalación de ninguna de estas utilidades, ya hablé algo sobre instalar y configurar [ZSH](http://geek.cl/cambio-en-mac-entra-zsh-sale-bash/) y [iTerm 2](http://geek.cl/instalar-personalizar-iterm-2/), respecto a [gpg (GnuPg)](https://www.gnupg.org/) y [pass](http://www.passwordstore.org/) escribiré algo más adelante. Pero lo importante acá es que de forma simple dejemos corriendo como demonio gpg-agent en Mac OS X utilizando un pluging presente para ZSH.


##Al Grano
Vamos a habilitar el pluging que viene por defecto dentro del amplio catálogo presente en ZSH de serie. 

*El listado de los plugins presentes se puede ver en ```~/.oh-my-zsh/plugins/*```*

Editemos el archivo de configuración de ZSH y agregamos el plugin.

```
nano ~/.zshrc
```

```
# Path to your oh-my-zsh installation.
export ZSH=$HOME/.oh-my-zsh

# Set name of the theme to load.
# Look in ~/.oh-my-zsh/themes/
# Optionally, if you set this to "random", it'll load a random theme each
# time that oh-my-zsh is loaded.
ZSH_THEME="fino-time"

# Example aliases
# alias zshconfig="mate ~/.zshrc"
# alias ohmyzsh="mate ~/.oh-my-zsh"

# Set this to use case-sensitive completion
# CASE_SENSITIVE="true"

# Uncomment this to disable bi-weekly auto-update checks
# DISABLE_AUTO_UPDATE="true"

# Uncomment to change how often to auto-update? (in days)
# export UPDATE_ZSH_DAYS=13

# Uncomment following line if you want to disable colors in ls
# DISABLE_LS_COLORS="true"

# Uncomment following line if you want to disable autosetting terminal title.
# DISABLE_AUTO_TITLE="true"

# Uncomment following line if you want to disable command autocorrection
# DISABLE_CORRECTION="true"

# Uncomment following line if you want red dots to be displayed while waiting for completion
# COMPLETION_WAITING_DOTS="true"

# Uncomment following line if you want to disable marking untracked files under
# VCS as dirty. This makes repository status check for large repositories much,
# much faster.
# DISABLE_UNTRACKED_FILES_DIRTY="true"

# Uncomment following line if you want to the command execution time stamp shown 
# in the history command output.
# The optional three formats: "mm/dd/yyyy"|"dd.mm.yyyy"|"yyyy-mm-dd"
HIST_STAMPS="dd.mm.yyyy"

# Would you like to use another custom folder than $ZSH/custom?
# ZSH_CUSTOM=/path/to/new-custom-folder

# Which plugins would you like to load? (plugins can be found in ~/.oh-my-zsh/plugins/*)
# Custom plugins may be added to ~/.oh-my-zsh/custom/plugins/
# Example format: plugins=(rails git textmate ruby lighthouse)
plugins=(git gpg-agent)

source $ZSH/oh-my-zsh.sh

# User configuration

export PATH="/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin"
# export MANPATH="/usr/local/man:$MANPATH"

# You may need to manually set your language environment
 export LANG=es_ES.UTF-8

# # Preferred editor for local and remote sessions
# if [[ -n $SSH_CONNECTION ]]; then
#   export EDITOR='vim'
# else
#   export EDITOR='mvim'
# fi

# Compilation flags
# export ARCHFLAGS="-arch x86_64"

# ssh
# export SSH_KEY_PATH="~/.ssh/dsa_id"
```

Así debe quedar el apartado plugins (**plugins=(git gpg-agent)**).

Una vez hecho esto reiniciamos iTerm2 y ya no nos pedirá constantemente la contraseña de gpg.
