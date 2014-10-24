# Node.js

使用 Homebrew 安装 [Node.js](http://nodejs.org/):

    $ brew update
    $ brew install node

一般 Node modules 被安装在每个项目的本地文件夹 `node_modules`，
但至少有几个包推荐你安装在全局：

[CoffeeScript](http://coffeescript.org/) and [Grunt](http://gruntjs.com/):

    $ npm install -g coffee-script
    $ npm install -g grunt-cli

### Npm usage

安装包:

    $ npm install <package> # Install locally
    $ npm install -g <package> # Install globally

安装包，并且将其保存你项目中的 `package.json` 文件:

    $ npm install <package> --save

查看 npm 安装的内容:

    $ npm list # Local
    $ npm list -g # Global

查看过期的包（本地或全局）:

    $ npm outdated [-g]

更新全部或特别指定一个包:

    $ npm update [<package>]

卸载包:

    $ npm uninstall <package>
