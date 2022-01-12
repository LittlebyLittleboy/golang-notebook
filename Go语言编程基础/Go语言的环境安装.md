### Go语言的环境安装

---
**第一部分：Go软件安装配置**
- <a href="#1.1">**1.1.Wind7安装**</a>
- <a href="#1.2">**1.2.MacOS安装**</a>
- <a href="#1.3">**1.3.Linux安装**</a>

**第二部分：Go开发目录结构**
- <a href="#2.1">**2.1.个人开发目录**</a>
- <a href="#2.2">**2.2.流行开发目录**</a>
- <a href="#2.3">**2.3.企业开发目录**</a>

---
<a id="1.1">**1.1.Wind7安装**</a>
- **1.软件下载**
```html
官方下载地址：https://golang.org/dl/ (科学上网)
官方镜像地址：https://golang.google.cn/dl/（正常上网）
```
```html
检查系统版本：计算机--->右键--->属性--->[确认Windows版本和系统类型]
确定安装软件：下载windows-amd64类型软件包，否则无法安装或无法正常使用
```
```html
截止到2020年1月1日:[注:新版本更新频繁]
目前最新版本：go1.13.5.windows-amd64
本文安装版本：go1.11.5.windows-amd64
```
![latest](https://www.showdoc.cc/server/api/common/visitfile/sign/1166de4c3513de2b2ddadab27217e6f0?showdoc=.jpg)
![local](https://www.showdoc.cc/server/api/common/visitfile/sign/2f56fb9f9dec18b29eb88432622b02b0?showdoc=.jpg)


- **2.软件安装**
**方案一：可执行文件安装**
```html
①.可执行安装文件确认
②.安装位置默认或定制
③.安装开始结束及测试
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/860608da68f93d784f4f282cdfb7be52?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/21bcb7a4d4e57c3fc2bd424a6c584364?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/0972e2960a3827d7ff63ecfb8dce0dc7?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/e35a5467078a89aea80181fbb611ce2b?showdoc=.jpg)
**方案二：压缩包解压安装**
```html
①.安装包解压到安装位置
压缩包：
go1.13.5.windows-amd64.zip
解压包：
go1.13.5.windows-amd64/go
②.进入执行程序目录测试
进入：
cmd:cd go1.13.5.windows-amd64/go/bin
执行：
cmd:go.exe
③.后续配置系统环境变量
```


- **3.软件配置**
```html
计算机--->右键--->属性--->高级系统设置
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/ea9b728da44c8c40e13f3540812320f5?showdoc=.jpg)
```html
--->[系统属性]--->高级--->环境变量
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/ffd9c95783a714f42a7f76868904727f?showdoc=.jpg)
```html
--->系统变量--->新建GOROOT---编辑Path--->新建GOPATH
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/9916cd27b121019f61c022ea6f0fef29?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/3e1d7a53312998a367acb850aaea9990?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/44ddeca72c5be32af913b12e9e020cc9?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/2e6053c36cbaf3f5696fc0a78a01aa04?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/723b366368ddc2821f9bfbe877c666e9?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/f005934238be39794082d02b4ba1677b?showdoc=.jpg)
```html
用户变量：
①.删除安装过程中默认添加的配置：GOPATH删除，Path中go安装路径部分删除
系统变量：
①.检查安装过程中是否默认添加的GOROOT配置：GOROOT检查，若存在则不变，否则添加GOROOT系统变量
②.检查安装过程中是否默认添加的Path部分配置：Path检查，若已添加Go部分则不变，否则添加Go部分配置
③.检查系统变量是否已存在GOROOT系统变量，否则添加GOPATH系统变量，路径为项目工作目录路径（如：D:\Go\[src,bin,pkg],则添加D:\Go\，此目录为新建的）
```

<a id="1.2">**1.2.MacOS安装**</a>
- **1.软件下载**
- **2.软件安装**
- **3.软件配置**

<a id="1.3">**1.3.Linux安装**</a>
- **1.软件下载**
```html
官方下载地址：https://golang.org/dl/ (科学上网)
官方镜像地址：https://golang.google.cn/dl/（正常上网）
```
```html
检查系统版本：# cat /proc/version 或 # uname -a
确定安装软件：下载linux-amd64类型软件包，否则无法安装或无法正常使用
```
```html
截止到2020年1月1日:[注:新版本更新频繁]
目前最新版本：go1.13.5.linux-amd64.tar.gz
本文安装版本：go1.11.5.linux-amd64.tar.gz
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/90f62e13cbdaa34e7a0c28ab428f2851?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/69c160d499955957a2ffef37819e5089?showdoc=.jpg)
```shell
# 使用wget工具下载二进制安装包/go1.11.5.linux-amd64.tar.gz到opt文件夹下
# wget -O /opt/go1.11.5.linux-amd64.tar.gz https://dl.google.com/go/go1.11.5.linux-amd64.tar.gz
```

- **2.软件安装**
```shell
# 将下载好的文件解压到/usr/local目录下，如果提示没有权限，加上sudo以root用户的身份再运行。执行完就可以在/usr/local/下看到go目录了。
# mkdir -p /usr/local/go
# tar -zxvf go1.17.2.linux-amd64.tar.gz --strip-components 1 -C /usr/local/go
```

- **3.软件配置**
```shell
# 配置环境变量：Linux下有两个文件可以配置环境变量
①./etc/profile是对所有用户生效的,修改/etc/profile后要重启生效，但是我使用source命令加载/etc/profile也生效了；
②.$HOME/.profile是对当前用户生效的,修改$HOME/.profile后使用source命令加载$HOME/.profile文件即可生效。
③.根据自己的情况自行选择一个文件打开，一般添加到系统环境变量。
```
```shell
# sudo vim /etc/profile
# 添加内容如下，保存退出。
export GOROOT=/usr/local/go
export PATH=$PATH:$GOROOT/bin
export GOPATH=$HOME/Go
# 尝试使用source命令加载，否则重启
# source /etc/profile
# 检查是否安装成功
# go version && go env
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/465ae78c777bf8c37ee1351df2baaf22?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/6ada71864e41dad31f3e87f0a46949d4?showdoc=.jpg)

<a id="2.1">**2.1.个人开发目录**</a>
- **1.树形目录结构**
![](https://www.showdoc.cc/server/api/common/visitfile/sign/170a459468c803d87bed890332f674d2?showdoc=.jpg)

- **2.图形目录结构**
![](https://www.showdoc.cc/server/api/common/visitfile/sign/75e785d7f7e23bae8c22b71bdaa8298f?showdoc=.jpg)

<a id="2.2">**2.2.流行开发目录**</a>
- **1.树形目录结构**
![](https://www.showdoc.cc/server/api/common/visitfile/sign/cccfc46bd0a847ff0db219718c59c497?showdoc=.jpg)

- **2.图形目录结构**
```html
Go语言中也是通过包来组织代码文件，我们可以引用别人的包也可以发布自己的包，但是为了防止不同包的项目名冲突，我们通常使用顶级域名来作为包名的前缀，这样就不担心项目名冲突的问题了。
因为不是每个个人开发者都拥有自己的顶级域名，所以目前流行的方式是使用个人的github用户名来区分不同的包。
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/5339d752bec2fc65885c8166a0e9c736?showdoc=.jpg)
```
示例：Rose和Jack都有一个Go项目，那么这两个包的路径就会是：
# import "github.com/Rose/Go"
# import "github.com/Jack/Go"
我们可以从GitHub下载被人的包：
# go get github.com/jmoiron/sqlx
```

<a id="2.3">**2.3.企业开发目录**</a>

- **1.树形目录结构**
![](https://www.showdoc.cc/server/api/common/visitfile/sign/56d0246e8ccc790db182bb8b455b05a3?showdoc=.jpg)

- **2.图形目录结构**
![](https://www.showdoc.cc/server/api/common/visitfile/sign/b186c15e83b99e4e7fbf7bf8c8ee0257?showdoc=.jpg)

---
**参考网络文章**
[**从零开始搭建Go语言开发环境**](https://www.liwenzhou.com/posts/Go/install_go_dev/)

---
**作者：小和尚学编程**
**时间：2020-02-05 22:38:42 星期三**
