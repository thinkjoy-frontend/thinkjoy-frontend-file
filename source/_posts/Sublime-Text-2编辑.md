title: Sublime Text 2编辑.md
date: 2015-11-27 08:21:16
categories: 环境配置
---
## 一、安装Package Control
1. 按ctrl + ` 快捷键或者菜单项View > Show Console 来调出命令界面
2. 粘贴代到命令界面并回车
3. 重启Sublime Text 2

``` python
import urllib2,os;pf='Package Control.sublime-package';ipp=sublime.installed_packages_path();os.makedirs(ipp) if not os.path.exists(ipp) else None;open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read())
``` 
#### 注：以下是Sublime Text 3的安装代码
``` python
import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
``` 
### 另外：本地安装方法
1. 点击Preferences > Browse Packages…菜单
2. 浏览一个文件夹，然后进入Installed Packages/文件夹
3. 下载 [Package Control.sublime-package](https://packagecontrol.io/Package%20Control.sublime-package)，然后复制到Installed Packages/目录下
4. 重启Sublime Text
5. [安装手册](https://packagecontrol.io/installation#st2)

## 二、安装Markdown Preview
1. 按command + shift + p
2. 输入pci 后回车(Package Control: Install Package)
3. 输入Markdown Preview回车

## 三、编辑

1. 按command + n 新建一个文档
2. 按command + shift + p
3. 使用Markdown语法编辑文档
4. 语法高亮，输入ssm 后回车(Set Syntax: Markdown)

## 四、在浏览器预览Markdown文档

1. 按command + shift + p
2. 输入mp 后回车(Markdown Preview: current file in browser)
3. 此时就可以在浏览器里看到刚才编辑的文档了
