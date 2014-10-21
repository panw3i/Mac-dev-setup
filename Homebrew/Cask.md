# Homebrew Cask

让我们试下通过 Homebrew Cask 优雅、简单、快速的安装和管理 OS X 图形界面程序，比如 Google Chrome 和 Dropbox。

### Install

安装 Homebrew-cask 是一件简单直接的事情，运行以下命令即可完成：

    $ brew tap caskroom/cask 「添加 Github 上的 caskroom/cask 库」
    $ brew install brew-cask 「安装 brew-cask 」
    $ brew cask install google-chrome 「安装 Google 浏览器」
    $ brew update && brew upgrade brew-cask && brew cleanup 「更新」

### Search

如果你想查阅 cask 是否存在你需要的 app，可以到 [caskroom.io](http://caskroom.io/) 进行搜索。

### Quick look plugins

有些 [插件](https://github.com/sindresorhus/quick-look-plugins) 可以让Mac 上的文件预览更有效，比如语法高亮、markdown 渲染、json 预览等等。

    $ brew cask install qlcolorcode
    $ brew cask install qlstephen
    $ brew cask install qlmarkdown
    $ brew cask install quicklook-json
    $ brew cask install qlprettypatch
    $ brew cask install quicklook-csv
    $ brew cask install betterzipql
    $ brew cask install webp-quicklook
    $ brew cask install suspicious-package

### App Installation

以下程序，我将会在 Apps 章节提及。

    $ brew cask install airmail
    $ brew cask install alfred
    $ brew cask install android-file-transfer
    $ brew cask install asepsis
    $ brew cask install appcleaner
    $ brew cask install caffeine
    $ brew cask install cheatsheet
    $ brew cask install doubletwist
    $ brew cask install dropbox
    $ brew cask install google-chrome
    $ brew cask install google-drive
    $ brew cask install google-hangouts
    $ brew cask install flux
    $ brew cask install latexian
    $ brew cask install onepassword
    $ brew cask install pdftk
    $ brew cask install spectacle
    $ brew cask install sublime-text
    $ brew cask install superduper
    $ brew cask install totalfinder
    $ brew cask install transmission
    $ brew cask install valentina-studio
    $ brew cask install vlc
