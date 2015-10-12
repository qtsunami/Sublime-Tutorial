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

## 快捷键 (keymap)
> Sublime Text 常用快捷键（MAC 下）

快捷键 		    | 功能
------------- | -------------
Content Cell  | Content Cell