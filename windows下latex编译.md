# 在windows上配置latex编译环境

## 在windows平台上选择Miktex发行版本

1. 进入[下载地址](https://miktex.org/download)，里面有一个==Basic MiKTex Installer==，下方就有一个==Download==的按钮，文件大小大概是192M.
2. 下载完成后，点击安装。就像我们平时平时安装软件一样，设置安装路径等等，也可以参考如下页面的[安装指导](https://miktex.org/howto/install-miktex)

## 安装sublime编辑器

sublime text3 编辑器是我们用来编译latex的界面工具。
1. [下载链接](https://download.sublimetext.com/Sublime%20Text%20Build%203126%20x64%20Setup.exe)，然后安装即可。
2. 打开sublime text3, 进入tools菜单，选择安装package control。按ctrl+shift+p快捷键就可以调出package control的页面，输入install packages，然后enter键；再输入Chineselocalization，然后enter。
3. 退出重启，就会发现sublime变成了中文界面。
4. 接着ctrl+shift+p快捷键，输入latextools，然后enter键。这样latex的编译环境就创建好了。
5. 当然sublime text是需要注册码的，我们可以在网上很容易找到[注册码](http://www.cnblogs.com/historymemory/p/6679553.html)，复制注册码，从begin licence开始到end licence结束。然后在sublime的帮助菜单，输入注册码，复制到框里即可。

## 安装pdf阅读器[sumatraPDF](http://rj.baidu.com/soft/detail/17862.html?ald)

## 最后一步啦

让我们试验一下，新建.tex文件，复制下列代码。保存，然后ctrl+B编译就可以了。
```Tex
\documentclass{ctexart}
\begin{document}
这是中文Hello,world!
\end{document}
```

