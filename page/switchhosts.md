## 浏览器如何得知网站服务器的ip?
-  向浏览器输入网址 [https://www.baidu.com/](http://www.baidu.com/),浏览器会查询本地计算机有没有存储域名baidu.com 对应的服务器IP, 如果存储了,浏览器直接向目标服务器发起三次握手的连接请求;如果没有存储, 则向DNS服务器发起"查询baidu.com对应服务器IP"的请求
- 本地计算机存储域名对应ip的文件就是hosts文件
- 如果我们更改了hosts文件, 就可以改变浏览器请求特定域名的资源时, 对应的服务器
- 在网站开发中, 为了模拟全仿真的测试环境, 也会改hosts, 比如我的网站fangyuanxiaozhan.com
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/54685175fd160e8c4f8c1cbb4eb60705.gif)

#### 上图中用到的工具就是SwitchHosts!

SwitchHosts开源地址: [https://github.com/oldj/SwitchHosts](https://github.com/oldj/SwitchHosts)

- macOS下载懒人链接: [SwitchHosts-macOS-x64_v3.3.12.5349.zip](https://github.com/oldj/SwitchHosts/releases/download/v3.3.12/SwitchHosts-macOS-x64_v3.3.12.5349.zip)

- Windows下载懒人链接: [SwitchHosts-win32-ia32_v3.3.12.5349.zip](https://github.com/oldj/SwitchHosts/releases/download/v3.3.12/SwitchHosts-win32-ia32_v3.3.12.5349.zip)
- 下载SwitchHosts-win32-ia32_v3.3.12.5349.zip后,解压压缩包, 进入解压的文件夹, 右键SwitchHosts! 并以管理员身份运行
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/fe8864db51c7b753470c3a01f13977f4.png)
- 给软件更改hosts的权限
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/044109a6f998d669242ea9ded837652a.png)

- 示例: SwitchHosts!新增关于百度的规则
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/d9fcf9d4c1c350b4b34371e6b2c2631d.gif)
- 示例: SwitchHosts!获取网络规则(使用了github的源比较慢)
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/f1e3e56cbc75f16714b13a3ea598945a.gif)
- 示例根据已有方案, 获得组合方案
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/2f28a3b11403de985e5bd493baca4497.gif)
- 删除方案
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/735e463a2507e26aabaefea84b2af5c8.gif)
- 打包导出方案
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/107a778af35204a7725c9dd3e781e780.gif)
- 导入方案
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/a268ff7f90c5edfdeda552296dfa4081.gif)

早期, GFW还不健全的时候, 访问Google不一定需要代理服务器, 改hosts就可以,但现在很难找到可用稳定的源了...

## 如果无法更改hosts
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/abdf947b3bbefed41179c6a183c8787a.png)
> 在Windows桌面新建一个hosts文件,替换`C:\Windows\System32\drivers\etc`中的hosts文件, 并为host开放权限
> ![](https://raw.githubusercontent.com/zhaoolee/GraphBed/master/images/163eb8ef6888e1efb4ac21ecc3826071.gif)

## 小结:
切换hosts对于普通用户而言, 其实完全不需要掌握, 对于软件开发者却是需要掌握的技能, SwitchHosts!能让软件开发者更方便的切换hosts, 而且开源跨平台, 是一个非常值得收藏的软件~

---
#### 本仓库Github链接: [https://github.com/oldj/SwitchHosts](https://github.com/oldj/SwitchHosts)



---


## 写在最后(我需要你的支持)
- 本文属于**Github星聚弃疗榜** 项目的一部分, 项目Github地址: [https://github.com/zhaoolee/StarsAndClown](https://github.com/zhaoolee/StarsAndClown)
- **Github星聚弃疗榜**, 为Github优秀创意项目写一封推荐信，让Github优秀项目造福人类~, 如果你喜欢这个项目, 希望你能为本项目添加一颗 星.

- StarsAndClown, Write a letter of recommendation for Github's outstanding creative projects, and let Github's outstanding projects benefit mankind~, If you like this project, I hope you can add a star  to this project.

