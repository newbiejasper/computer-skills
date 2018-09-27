1. 在数学分析1的仓库中遇到了.synctex的文件，想要用.gitignore把它忽略掉。但是调价了忽略项\*.synctex没有起作用。
   原因：.gitignore只能对未被track的文件起作用，所以用过add,commit的文件就没有用了。
   解决方案:
   `git rm -r --cached .`
   `git add`
   `git commit -m "message"`
