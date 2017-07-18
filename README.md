# less
less编译的方式
1、客户端编译：软件名称Koala
Koala 特性：
多语言支持 ：支持 less 、 sass 、 coffeescript 和 compass framework 。
实时编译： 监听文件，当文件改变时自动执行编译，这一切都在后台运行，无需人工操作。
编译选项： 支持自定义编译选项。
代码压缩： less

2、submile的less2css插件
Package Control安装less2css， less（高亮）
安装Less2Css;
步骤：
（1）快捷键 Ctrl+Shift+P（菜单 – Tools – Command Paletter），输入 install 选中Install Package并回车，输入或选择Less2Css（注意左下角的小文字变化，会提示安装成功）。
（2）https://github.com/duncansmart/less.js-windows 下载该文件并解压到本地目录（eg:D:\less.js-windows-master）；点击计算机 右击 属性，选择高级系统设置，编辑Path ,将解压目录，添加到PATH中。
（3） 安装完以上操作，重启Sublime后，Control+s 保存Less文件，会在同目录下生成相应的.css文件。至此操作已经完成。如果想改变快捷键和生成css的格式，打开复制Settings-Default内的内容到Settings-User中，更改其中的值，例如把minName变为True，minify变为True,会生成相应的x.min.css文件。如果编译时submile报错（unable to interpret argument clean-css-if itis a plugin(less-plugin-clean-css） 需要npm 里更新下less-plugin-clean-css，npm install less-plugin-clean-css

3、node 编译
1.下载notejs
https://nodejs.org/en/

2.首先你要安装lessc。我是用npm包管理器直接安装的，只需要一条命令，如下：
npm install less -g

3.检查lessc是不是安装成功了：
lessc -v

在 cmd中可以手动编译
然后可以手动编译less文件为css （f:\WorkFiles\天津欢乐谷\style\alan.less）
进入目录 ：cd f:\WorkFiles\天津欢乐谷\style
lessc alan.less > alan.css 编译less为css文件
