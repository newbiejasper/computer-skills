1. 在windows平台下，我们打开jupyter notebook时系统默认是采用默认浏览器Edge，然呢Edge浏览器在显示效果上总会出现一些问题，比如TAB补全效果不好，所以我们需要设置自己中意的浏览器。比如谷歌浏览器：

在个人目录下即C:\Users\xxx\.jupyter下创建
jupyter_notebook_config.py

输入下列代码即可设置为谷歌浏览器
```python
import webbrowser
webbrowser.register('chrome', None, webbrowser.GenericBrowser('C:\\Program Files (x86)\\Google\\Chrome\\Application\\chrome.exe'))
c.NotebookApp.browser = 'chrome'
```