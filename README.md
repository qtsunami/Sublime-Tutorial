# Sublime Text 快捷键

## 介绍 (Introduce)
> Sublime Text具有漂亮的用户界面和强大的功能，例如代码缩略图，Python的插件，代码段等。还可自定义键绑定，菜单和工具栏。Sublime Text 的主要功能包括：拼写检查，书签，完整的 Python API ， Goto 功能，即时项目切换，多选择，多窗口等等。Sublime Text 是一个跨平台的编辑器，同时支持Windows、Linux、Mac OS X等操作系统。

## 插件 (Plugins)
> Sublime Text 有一个强大的，基于python的插件API。

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
> `==`

## 主题 (Theme)
[Afterglow](https://github.com/YabataDesign/afterglow-theme)  **Afterglow is a minimal dark Theme for Sublime Text 2 and 3. Also it is a syntax color scheme. The theme is based on the great theme Spacegray. The syntax color scheme is mostly derived from idlefingers.**

![图片](https://github.com/liveNo/Sublime-Tutorial/raw/master/Screenshots/D4CD1C6C-F456-4EB3-BD17-7EFA58D5AA54.png)

[Material](https://github.com/equinusocio/material-theme) **点击看具体的吧**

![图片](https://github.com/liveNo/Sublime-Tutorial/raw/master/Screenshots/material-theme.png)

## 快捷键 (keymap)
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
⌘⇧W   			| 关闭sublime，关闭所有文件
⌘⇧T   			| 重新打开最近关闭的文件
⌘T				| 前往文件
⌘⌃P				| 前往项目
⌘R				| 前往method
⌘⇧P				| 命令提示
⌃G				| 前往行
⌘KB				| 开关侧栏
⌃`				| 打开控制台

**编辑**

快捷键 		  	| 功能
------------ 	| ---------------------
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
⌘/				| 注释
⌘⌥/				| 块注释
⌘Y				| 恢复或重复
⌘⇧V				| 粘贴并自动缩进
⌃M				| 跳转至对应的括号
⌘U				| 软撤销（可撤销光标移动）
⌘⇧U				| 软重做（可重做光标移动）

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
















