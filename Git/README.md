# Git and Github

作为一名开发者怎么可能没有 [Git](http://git-scm.com/) ? 我们马上来安装：

    $ brew install git

好的，现在我们来测试一下 gti 是否安装完好：

    $ git --version

运行 `$ which git` 将会输出 `/usr/local/bin/git`.

接着，我们将定义你的 Git 帐号（与你在 [GitHub](https://github.com/) 使用的用户名和邮箱一致）

    $ git config --global user.name "Your Name Here"
    $ git config --global user.email "your_email@youremail.com"

They will get added to your `.gitconfig` file.

将你的代码推送到 Github 上的仓库，我们将推荐使用 HTTPS 方法（另一个是 SSH）。当我们将 Git password 缓存后 [here](https://help.github.com/articles/set-up-git):，你就不需要使用的时候每次都输入用户名和密码 :

    $ git config --global credential.helper osxkeychain

- - -

### SSH Config for Github

SSH 的设置参考此链接 [here](https://help.github.com/articles/generating-ssh-keys).

- - -

