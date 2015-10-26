# Sublime Text 快捷键

## 0x00 介绍 (Introduce)
> Sublime Text具有漂亮的用户界面和强大的功能，例如代码缩略图，Python的插件，代码段等。还可自定义键绑定，菜单和工具栏。Sublime Text 的主要功能包括：拼写检查，书签，完整的 Python API ， Goto 功能，即时项目切换，多选择，多窗口等等。Sublime Text 是一个跨平台的编辑器，同时支持Windows、Linux、Mac OS X等操作系统。（百度百科）

**进入[Sublime Text 官网](http://www.sublimetext.com/)**， 目前Sublime Text 3 Beta版已发布，最新版本为Build 3083。

#### *下载Sublime Text*
- [Sublime Text 2下载](http://www.sublimetext.com/2) 
- [Sublime Text 3下载](http://www.sublimetext.com/3)

## 0x01 插件 (Plugins)
> Sublime Text 有一个强大的，基于python的插件API。Sublime Text插件丰富

### 安装Package Control

按Ctrl + ` 调出console，粘贴下列安装代码到底部命令行并回车：

**适用于Sublime Text 2**

	import urllib2,os;pf='Package Control.sublime-package';ipp=sublime.installed_packages_path();os.makedirs(ipp) if not os.path.exists(ipp) else None;open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read())
	
**适用于Sublime Text 3**

	import urllib.request,os;pf='Package Control.sublime-package';ipp=sublime.installed_packages_path();urllib.request.install_opener(urllib.request.build_opener(urllib.request.ProxyHandler()));open(os.path.join(ipp,pf),'wb').write(urllib.request.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read())

重启Sublime Text。如果在Perferences->Package Settings 中看到package control这一项，则安装成功。

### 用Package Control 安装其他插件
> 按下Cmd+Shift+P 调出命令面板，输入install并调出Install Package选项并回车，然后在列表中选中要安装的插件。

### 推荐插件
* **[Emmet](http://emmet.io/)** 概括的说，Emmet(其前身是Zen Coding) 是一个可以让你更快更高效地编写HTML/CSS，可以节省你大量时间的插件。

	![Emmet](https://github.com/liveNo/Sublime-Tutorial/raw/master/Screenshots/emmet.gif)
	
	<font color=red>调用Emmet快捷键：</font>⌃⌥↩。
* **[Git](https://github.com/kemayo/sublime-text-git)**   这个插件会将Git整合进你的SublimeText，使的你可以在SublimeText中运行Git命令，包括添加，提交文件，查看日志，文件注解以及其它Git功能。

	![GIT](https://github.com/liveNo/Sublime-Tutorial/raw/master/Screenshots/git.jpeg)
	
* **[AutoFileName](https://github.com/BoundInCode/AutoFileName)** 自动补全文件路径，非常方便。

	![AutoFileName](https://github.com/liveNo/Sublime-Tutorial/raw/master/Screenshots/autofilename.jpg)
	
* **[DocBlockr](https://github.com/spadgos/sublime-jsdocs)** DocBlockr会成为你编写代码文档的有效工具。当输入/**并且按下Tab键的时候，这个插件会自动解析任何一个函数并且为你准备好合适的模板

	![DocBlockr](https://github.com/liveNo/Sublime-Tutorial/raw/master/Screenshots/docblock.jpeg)
	
* **[Sublimerge Pro](http://www.sublimerge.com/)**  sublimerge是一个插件，而不是一个独立的应用程序。sublimerge 主要用于文件之间的对比。
	
	![Sublimerge Pro](https://github.com/liveNo/Sublime-Tutorial/raw/master/Screenshots/sublimerge.png)
	
		1.如果你安装了Package Control， ⌘⇧p([cmd]+[shift]+[p])打开命令控制板
		2.选择Package Control: Install Package
		3.搜索 Sublimerge pro 然后点击安装，即可。
		4.[ctrl]+[alt]+d可以调出与Clipboard进行比较。
	
* **[SFTP](http://wbond.net/sublime_packages/sftp)** 快速编辑远程服务器文件
* **[CTags](https://github.com/SublimeText/CTags)**  让Sublime 支持Ctags
* **[SublimeLinter3](https://github.com/SublimeLinter/SublimeLinter3)** 行内语法检测插件，支持： C/C++, Java, Python, PHP, JS, HTML, CSS, etc.
* **[Alignment](http://wbond.net/sublime_packages/alignment)** 简单到极致的多行选择和多行选择对齐插件
* **[Markdown-preview](https://github.com/revolunet/sublimetext-markdown-preview)** Markdown
* **[ChineseLocalization](https://github.com/rexdf/Chinese-Localization)** Sublime 汉化插件

	

## 0x02 主题 (Theme)
[Afterglow](https://github.com/YabataDesign/afterglow-theme)  **Afterglow is a minimal dark Theme for Sublime Text 2 and 3. Also it is a syntax color scheme. The theme is based on the great theme Spacegray. The syntax color scheme is mostly derived from idlefingers.**

![图片](https://github.com/liveNo/Sublime-Tutorial/raw/master/Screenshots/D4CD1C6C-F456-4EB3-BD17-7EFA58D5AA54.png)

[Material](https://github.com/equinusocio/material-theme) **点击看具体的吧**

![图片](https://github.com/liveNo/Sublime-Tutorial/raw/master/Screenshots/material-theme.png)



## 0x03 快捷键 (keymap)
> Sublime Text 常用快捷键（MAC 下） 
> 
> 符号说明 
> 
> - ⌘：command  
> - ⌃：control 
> - ⌥：option
> - ⇧：shift
> - ↩：enter
> - ⌫：delete

**打开/关闭/前往**

快捷键 		  	| 功能
------------ 	| ---------------------
⌘⇧N   			| 打开一个新的sublime窗口
⌘N   			| 新建文件
⌘⇧W   			| 关闭sublime，关闭所有文件
⌘W   			| 关闭当前文件
⌘P				| 跳转、前往文件、前往项目、命令提示、前往method等等（Goto anything）
⌘⇧T   			| 重新打开最近关闭的文件
⌘T				| 前往文件
⌘⌃P				| 前往项目
⌘R				| 前往method
⌘⇧P				| 命令提示
⌃G				| 前往行
⌘KB				| 开关侧栏
⌃`				| 打开控制台
⌃-				| 光标跳回上一个位置
⌃⇧-				| 光标恢复位置 

**编辑**

快捷键 		  	| 功能
------------ 	| ---------------------
⌘A				| 全选
⌘L				| 选择行（重复按下将下一行加入选择）
⌘D				| 选择词（重复按下时多重选择相同的词进行多重编辑）
⌃⇧M				| 选择括号的内容
⌘⇧↩				| 在当前行前插入新行
⌘↩				| 在当前行后插入新行
⌃⇧K				| 删除行
⌘KK				| 从光标处删除至行尾
⌘K⌫				| 从光标处删除至行首
⌘⇧D				| 复制（多）行
⌘J				| 合并（多）行
⌘KU				| 改为大写
⌘KL				| 改为小写
⌘C				| 复制
⌘X				| 剪切
⌘V				| 粘贴
⌘/				| 注释
⌘⌥/				| 块注释
⌘Z				| 撤销
⌘Y				| 恢复撤销
⌘⇧V				| 粘贴并自动缩进
⌘⌥V				| 从历史中选择粘贴
⌃M				| 跳转至对应的括号
⌘U				| 软撤销（可撤销光标移动）
⌘⇧U				| 软重做（可重做光标移动）
⌘⇧S				| 保存所有文件
⌘]				| 向右缩进
⌘[				| 向左缩进
⌘⌥T				| 特殊符号集
⌘⇧L				| 将选区转换成多个单行选区

**查找/替换**

快捷键 		  	| 功能
------------ 	| ---------------------
⌘f 	 		 	| 查找
⌘⌥f	 			| 查找并替换
⌘⌥g				| 查找下一个符合当前所选的内容
⌘⌃g				| 查找所有符合当前选择的内容进行多重编辑
⌘⇧F				| 在所有打开的文件中进行查找

**拆分窗口/标签页**

快捷键			| 功能
---------- 	| -----------
⌘⌥[1,2,3,4]	| 单列、双列、三列、四列
⌘⌥5				| 网格（4组）
⌃[1,2,3,4]	| 焦点移动到相应的组（分屏编号）
⌃⇧[1,2,3,4]	| 将当前文件移动到相应的组（分屏编号）
⌘[1,2,3,4]	| 选择相应的标签页

**快捷操作**

快捷键 		  	| 功能
------------ 	| ---------------------
⌘⌃上下键		| 两行交换位置
⌘KB				| 显示/隐藏侧边栏
















