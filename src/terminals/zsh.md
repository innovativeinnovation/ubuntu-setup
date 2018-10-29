# Zsh

[Zsh](http://www.zsh.org/) is a shell designed for interactive use, although
it is also a powerful scripting language.

### Installation

To install Zsh:

```bash
sudo apt install zsh
```

To set Zsh as the default login shell:

```bash
sudo usermod -s /usr/bin/zsh $(whoami)
```

Now restart your computer and repoen your terminal.

If you don't already have a `~/.zshrc` configuration, copy the recommended
settings with:

```bash
cp /etc/zsh/newuser.zshrc.recommended .zshrc
```

To install Powerline, Powerline fonts and Zsh Powerlevel9k Theme:

```bash
sudo apt install powerline fonts-powerline zsh-theme-powerlevel9k
```

To install Oh My Zsh framework:

```bash
sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

To enable Powerlevel9k theme:

```bash
echo "source /usr/share/powerlevel9k/powerlevel9k.zsh-theme" >> ~/.zshrc
```

To install and enable Zsh Syntax Highlighting plugin:

```bash
sudo apt install zsh-syntax-highlighting
echo "source /usr/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ~/.zshrc
```

### Plugins

Oh-My-Zsh has many plugins. You can find a list of pre-installed plugins at
https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins

### Screenshot

![Zsh](../images/zsh.png)
