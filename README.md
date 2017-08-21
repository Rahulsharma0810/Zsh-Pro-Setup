# Rapid ZSH Setup  


[![N|Solid](http://ohmyz.sh/img/OMZLogo_BnW.png)](http://ohmyz.sh/)

Repo's Main Moto to provide rapid **ohmyzsh** setup with awesome plugins and abviously with sleek theme.

# Theme
###
#### [Avit](https://github.com/robbyrussell/oh-my-zsh/wiki/themes#avit)
[![N|Solid](https://github.com/sindresorhus/pure/blob/master/screenshot.png)](https://github.com/sindresorhus/pure)
# Plugins
#### - [Composer](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#composer)
#### - [Git](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#git)
#### - [Sublime](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#sublime)
#### - [Sudo](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#sudo)
#### - [Web-search](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#web-search)
#### - [extract]()
#### - [Z]()

### Installation
>sudo apt-get install zsh

>sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

### Post Installation

Add zshrc in .bashrc for autoload

```
# Launch Zsh
if [ -t 1 ]; then
exec zsh
fi
```

### Configuration

- Edit **~/.zshrc** for more configuration
``` subl ~/.zshrc ```
- Replace it with
```
# If you come from bash you might have to change your $PATH.
# export PATH=$HOME/bin:/usr/local/bin:$PATH

# Path to your oh-my-zsh installation.
  export ZSH=/home/rvs/.oh-my-zsh

# Set name of the theme to load. Optionally, if you set this to "random"
# it'll load a random theme each time that oh-my-zsh is loaded.
# See https://github.com/robbyrussell/oh-my-zsh/wiki/Themes
ZSH_THEME="refined"

# Uncomment the following line to use case-sensitive completion.
# CASE_SENSITIVE="true"

# Uncomment the following line to use hyphen-insensitive completion. Case
# sensitive completion must be off. _ and - will be interchangeable.
# HYPHEN_INSENSITIVE="true"

# Uncomment the following line to disable bi-weekly auto-update checks.
# DISABLE_AUTO_UPDATE="true"

# Uncomment the following line to change how often to auto-update (in days).
# export UPDATE_ZSH_DAYS=13

# Uncomment the following line to disable colors in ls.
# DISABLE_LS_COLORS="true"

# Uncomment the following line to disable auto-setting terminal title.
# DISABLE_AUTO_TITLE="true"

# Uncomment the following line to enable command auto-correction.
# ENABLE_CORRECTION="true"

# Uncomment the following line to display red dots whilst waiting for completion.
# COMPLETION_WAITING_DOTS="true"

# Uncomment the following line if you want to disable marking untracked files
# under VCS as dirty. This makes repository status check for large repositories
# much, much faster.
# DISABLE_UNTRACKED_FILES_DIRTY="true"

# Uncomment the following line if you want to change the command execution time
# stamp shown in the history command output.
# The optional three formats: "mm/dd/yyyy"|"dd.mm.yyyy"|"yyyy-mm-dd"
# HIST_STAMPS="mm/dd/yyyy"

# Would you like to use another custom folder than $ZSH/custom?
# ZSH_CUSTOM=/path/to/new-custom-folder

# Which plugins would you like to load? (plugins can be found in ~/.oh-my-zsh/plugins/*)
# Custom plugins may be added to ~/.oh-my-zsh/custom/plugins/
# Example format: plugins=(rails git textmate ruby lighthouse)
# Add wisely, as too many plugins slow down shell startup.

plugins=(composer git sublime sudo web-search extract z  zsh-syntax-highlighting)

source $ZSH/oh-my-zsh.sh

# User configuration

# export MANPATH="/usr/local/man:$MANPATH"

# You may need to manually set your language environment
# export LANG=en_US.UTF-8

# Preferred editor for local and remote sessions
# if [[ -n $SSH_CONNECTION ]]; then
#   export EDITOR='vim'
# else
#   export EDITOR='mvim'
# fi

# Compilation flags
# export ARCHFLAGS="-arch x86_64"

# ssh
# export SSH_KEY_PATH="~/.ssh/rsa_id"

# Set personal aliases, overriding those provided by oh-my-zsh libs,
# plugins, and themes. Aliases can be placed here, though oh-my-zsh
# users are encouraged to define aliases within the ZSH_CUSTOM folder.
# For a full list of active aliases, run `alias`.
#
# Example aliases
# alias zshconfig="mate ~/.zshrc"
# alias ohmyzsh="mate ~/.oh-my-zsh"
export PATH="$PATH:$HOME/.composer/vendor/bin"
export PATH=~/.composer/vendor/bin:$PATH
export PATH="/usr/local/sbin:$PATH"

```
- source ~/.zshrc
