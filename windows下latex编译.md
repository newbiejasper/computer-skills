# 在windows上配置latex编译环境

## 在windows平台上选择texlive发行版本

1. 搜索下载texlive。
2. 安装过程参考这篇[百度经验](https://jingyan.baidu.com/article/f0e83a2588f6d022e5910128.html)。

## 安装sublime编辑器

sublime text3 编辑器是我们用来编译latex的界面工具。
1. [下载链接](https://download.sublimetext.com/Sublime%20Text%20Build%203143%20Setup.exe)，然后安装即可。
2. 打开sublime text3, 进入tools菜单，选择安装package control。按ctrl+shift+p快捷键就可以调出package control的页面，输入install package，然后enter键；再输入Chineselocalization，然后enter。
3. 退出重启，就会发现sublime变成了中文界面。
4. 接着ctrl+shift+p快捷键，输入install packages,按enter键进入，输入latextools，然后enter键。这样latex的编译环境就创建好了。
5. 当然sublime text是需要注册码的，我们可以在网上很容易找到[注册码](http://blog.csdn.net/qq_33678670/article/details/69397550)，复制注册码，从begin licence开始到end licence结束。然后在sublime的帮助菜单，输入注册码，复制到框里即可。
6. 按照以上安装插件的方法，接着安装latex-cwl和latex snippets插件，第一个插件有自动补全的功能，比如你希腊字母忘记怎么打了，可以只输入首字母，就会提示你以这个字母开头的所有命令。第二个插件是代码块的功能，为了提高输入效率的，比如，你想打公式是一个分式1/2,需要输入\frac{1}{2},代码其实很长，还有好多括号，很容易出错。这个时候snippet的功能就体现出来了,安装这个包之后，只需要输入frac,按下tab键，就可以快速生成模板。

## 安装pdf阅读器[sumatraPDF](http://rj.baidu.com/soft/detail/17862.html?ald)

## 最后一步啦

让我们试验一下，打开sublime text，新建.tex文件，复制下列代码。保存，然后ctrl+B编译就可以了。
```Tex
\documentclass{ctexart}
\begin{document}
这是中文Hello,world!
\end{document}
```

此时应该会弹出package control的对话框，你应该选择采用xelatex引擎编译。

