# Zsh

我们将安装 `zsh` ，其功能和主题将由 `oh-my-zsh` 提供。这安装和使用的过程是非常简易的。其中`Env.sh` 文件用于维护别名（aliases），输出（exports）和路径改变（path changes）等等，以免影响 `~/.zshrc`。

### Zsh

使用 homebrew 完成 zsh 和 zsh completions 的安装

        brew install zsh zsh-completions

安装 oh-my-zsh 让 zsh 获得额外的功能和主题

        curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh

用文本编辑器或 vi 打开 `.zshrc` 进行以下编辑

        ZSH_THEME=pygmalion
        alias zshconfig="vi ~/.zshrc"
        alias envconfig="vi ~/Projects/config/env.sh"
        plugins=(git colored-man colorize github jira vagrant virtualenv pip python brew osx zsh-syntax-highlighting)

### Env.sh
~~~
    #!/bin/zsh

    # PATH
    export PATH="/usr/local/share/python:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    export EDITOR='vi -w'
    # export PYTHONPATH=$PYTHONPATH
    # export MANPATH="/usr/local/man:$MANPATH"

    # Virtual Environment
    export WORKON_HOME=$HOME/.virtualenvs
    export PROJECT_HOME=$HOME/Projects
    source /usr/local/bin/virtualenvwrapper.sh

    # Owner
    export USER_NAME="YOUR NAME"
    eval "$(rbenv init -)"

    # FileSearch
    function f() { find . -iname "*$1*" ${@:2} }
    function r() { grep "$1" ${@:2} -R . }

    #mkdir and cd
    function mkcd() { mkdir -p "$@" && cd "$_"; }

    # Aliases
    alias cppcompile='c++ -std=c++11 -stdlib=libc++'
~~~
