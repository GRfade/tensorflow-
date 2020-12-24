# tensorflow安装教程（简略版）
tensorflow安装教程（简略版）

这是一个简单版本的tensorflow安装教程


### 前提软件需要

- anaconda
- NVDIA驱动程序更新
-（不需要先下载什么cuda、cudnn）


### anaconda

在anaconda中创建一个环境，在这个环境中你怎么下载，怎么折腾都行，你要理解的是在你下载好anaconda后，里面自带了一个python解释器以及多个第三方库，这就相当于是一个虚拟环境了。

但我不建议你在这个环境里配，因为万一配错了 不好删除。

在重新创建好一个环境后，在环境里面下载tensorflow，这里有两个方法下载（不要用pycharm的界面化下载，也不要用anaconda的图形化界面下载，肯定会出问题，不出问题你牛逼！）

- conda install tensorflow=2.X
- pip install tensorflow==2.X

（建议版本不要太新，太新的话教程都没有，而且对应的cudnn好像也有点问题）

这里两个都可以，建议带上版本号，如果没有版本号的话默认下载最新版，就会对后面很麻烦，
下载完了之后（用镜像或者源下载）可以开始下载cuda和cudnn

这个时候你要记得你下载的tensorflow是哪个版本，**对应的版本对应的cuda和cudnn**

这里一定要注意，一定要**版本对应**

tips：这里有一个小细节，如果你下载的是tensorflow2.x版本的话，默认把cuda下载好了，所以你只需要下载cudnn就行了


想要知道你哪些没下载就很简单，打开虚拟环境运行python，import tensorflow，然后输出gpu信息 ，如果能输出来就说明你牛逼。如果不能你要看看报错信息，他会告诉你那个文件没安装

你按照没安装的文件进行安装就行了。


（ps多亏虚拟环境我安装了可能有十几遍 几乎pip conda  每一个都尝试了一遍 终于安装成功，）
