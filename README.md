# Rapid ZSH Setup  


[![N|Solid](http://ohmyz.sh/img/OMZLogo_BnW.png)](http://ohmyz.sh/)

Repo's Main Moto to provide rapid **ohmyzsh** setup with awesome plugins and abviously with sleek theme.

# Theme
###
#### [Refined](https://github.com/robbyrussell/oh-my-zsh/wiki/themes#avit)
[![N|Solid](https://github.com/sindresorhus/pure/blob/master/screenshot.png)](https://github.com/sindresorhus/pure)
# Plugins
#### - [Composer](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#composer)
#### - [Git](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#git)
#### - [Sublime](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#sublime)
#### - [Sudo](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins#sudo)
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
```vi ~/.zshrc```
- Replace it with ```~/.zshrc``` content
- Uncomment Section Accroding to your needs.
- source ~/.zshrc
