# zman

[![License](https://img.shields.io/badge/license-MIT-007EC7)](/LICENSE)
[![works with prezto](https://img.shields.io/badge/works%20with-%E2%9D%AF%E2%9D%AF%E2%9D%AF%20prezto-red)](#install-for-prezto)
[![works with ohmyzsh](https://img.shields.io/badge/works%20with-%20%E2%9E%9C%20oh--my--zsh-C2D33F)](#install-for-oh-my-zsh)

> Zsh plugin that uses `fzf` to quickly find and browse Zsh docs

![zman](https://raw.githubusercontent.com/mattmc3/zman/resources/img/zman.gif)

## Description

This plugin scrapes the Zsh documentation for index words and phrases and lets you
quickly navigate to the online docs. It uses `[fzf]` to provide fuzzy searching. Be sure
you have it installed prior to using this plugin.

## Installation

### Install with a Zsh plugin manager

To install using a Zsh plugin manager, add the following to your .zshrc

- [pz]: `pz source mattmc3/zman`
- [zcomet]: `zcomet load mattmc3/zman`
- [zgenom]: `zgenom load mattmc3/zman`
- [znap]: `znap source mattmc3/zman`

### Install manually, without a plugin manager

To install manually, first clone the repo:

```zsh
git clone https://github.com/mattmc3/zman ${ZDOTDIR:-~}/.zplugins/zman
```

Then, in your .zshrc, add the following line:

```zsh
source ${ZDOTDIR:-~}/.zplugins/zman/zman.zsh
```

### Install for Oh-My-Zsh

To install with [Oh-My-Zsh][ohmyzsh], first clone the repo from an interactive Zsh session:

```zsh
# make sure your $ZSH_CUSTOM is set
ZSH_CUSTOM=${ZSH_CUSTOM:-~/.oh-my-zsh/custom}

# now, clone the plugin
git clone https://github.com/mattmc3/zman $ZSH_CUSTOM/plugins/zman
```

Then, add the plugin to your Oh-My-Zsh plugins list in your .zshrc

```zsh
# in your .zshrc, add this plugin to your plugins list
plugins=(... zman)
```

### Install for Prezto

To install with [Prezto][prezto], first clone the repo from an interactive Zsh session:

```zsh
# make sure your $ZPREZTODIR is set
ZPREZTODIR=${ZPREZTODIR:-~/.zprezto}
# clone the repo to a prezto contrib dir
git clone https://github.com/mattmc3/zman $ZPREZTODIR/contrib/zman/external
# set up the contrib
echo "source \${0:A:h}/external/zman.plugin.zsh" > $ZPREZTODIR/contrib/zman/init.zsh
```

Then, add the plugin to your Prezto plugins list in .zpreztorc

```zsh
zstyle ':prezto:load' pmodule \
  ... \
  zman \
  ...
```

[ohmyzsh]: https://github.com/ohmyzsh/ohmyzsh
[prezto]: https://github.com/sorin-ionescu/prezto
[zshzoo]: https://github.com/zshzoo/zshzoo
[pz]: https://github.com/mattmc3/pz
[zcomet]: https://github.com/agkozak/zcomet
[zgenom]: https://github.com/jandamm/zgenom
[znap]: https://github.com/marlonrichert/zsh-snap
[fzf]: https://github.com/junegunn/fzf
