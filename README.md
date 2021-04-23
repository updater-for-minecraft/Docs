## updater——更新客户端小程序，Mod服好帮手(适用于2.6.5)

Updater好处都有啥？

1. 两种服务端支持，大佬小白没烦恼
2. 支持静态HTTP服务器（阿里腾讯对象存储、CDN、FTP）
3. 支持动态PHP服务端，安装简单，开箱即用，面板服友好
4. 支持`跟随启动`特性，在游戏启动前更新文件
5. 两种工作模式支持，指定路径更新和指定文件更新
6. 用正则表达式精细匹配要更新的目录
7. Updater本身支持自身热升级，升级新版不用重发zip包
8. 可执行文件打包，无需Jvav环境也能正常运行
9. CEF驱动，界面支持100%自定义

## 开始!

!> 在使用Updater之前，请确保您了解基本的计算机相关概念，比如：路径，HTTP，json文件，目录，URL，端口等

在开始使用之前，你需要从两种服务端类型中选择**其中一种**适合自己的

+ 如果你用过对象存储服务，CDN等云服务，建议选择`静态服务端`

+ 如果你是一个站长，做过网站，搭建过论坛等PHP软件，建议选择`PHP服务端`

+ 如果你是一位技术专家，想使用CDN发挥出Updater的全部能力，建议选择`静态服务端`

+ 如果你有现成的PHP环境和一个配置不错的网站主机，建议选择`PHP服务端`

+ 如果你有一位关系不错的大佬朋友，你想请他帮忙配置，请选择`静态服务端`

在选择好你要的服务端类型之后，请点击[起步](起步.md)，如果仍然无法做出决定，请点击[这里](服务端类型比较.md)查看两种服务端的详细对比

目录：

1. [起步](起步.md)
2. [PHP服务端安装](PHP服务端安装.md)
3. [静态服务端安装](静态服务端安装.md)
4. [服务端配置文件](服务端配置文件.md)
5. [服务端配置文件示例](服务端配置文件示例.md)
6. [小工具使用教程](小工具使用教程.md)
7. [客户端安装教程](客户端安装教程.md)
8. [常见问题解答](FAQ.md)
9. [从旧版本升级](从旧版本升级.md)
10. [自定义界面](自定义界面教程.md)
11.  [问题反馈](问题反馈.md)
12. [参与贡献](参与贡献.md)

## 开发计划

+ [x] ~~隐藏客户端程序的倒计时黑框，优化PCL2启动器的体验~~（`2021年3月12日/客户端2.1.3`）
+ [x] ~~使小工具`Deployer`额外支持FTP/SFTP上传操作~~（`2021年3月22日/小工具1.6`）
+ [x] ~~同时支持纯文本路径匹配模式和正则表达式匹配模式~~(`2021年3月28日/热更新包2.6.4`)
+ [x] ~~支持多线程下载~~（`2021年3月22日/客户端2.6.2`）
+ [ ] 配置文件可视化编辑

## 历史版本

1. [2.6.1文档](https://github.com/updater-for-minecraft/Docs/tree/2.6.1)
2. [2.6.3文档](https://github.com/updater-for-minecraft/Docs/tree/2.6.3)

---

更旧的版本：

1. [文档-2.5](https://github.com/updater-for-minecraft/Docs/tree/c49c065a9815b35c168d7d8616abf77d510ab2e0) 
2. [文档-2.4](https://github.com/updater-for-minecraft/Docs/tree/c49c065a9815b35c168d7d8616abf77d510ab2e0) 
3. [文档-2.1-2.2](https://github.com/updater-for-minecraft/Docs/tree/c49c065a9815b35c168d7d8616abf77d510ab2e0) 
4. [文档-2.0-2.1.1](https://github.com/updater-for-minecraft/Docs/tree/c49c065a9815b35c168d7d8616abf77d510ab2e0)
5. [文档-1.2.2](https://github.com/updater-for-minecraft/Docs/tree/c49c065a9815b35c168d7d8616abf77d510ab2e0)
6. [文档-1.2.1](https://github.com/updater-for-minecraft/Docs/tree/c49c065a9815b35c168d7d8616abf77d510ab2e0)
7. [文档-1.0-1.2.0](https://github.com/updater-for-minecraft/Docs/tree/c49c065a9815b35c168d7d8616abf77d510ab2e0)
8. [文档-FileSA远古版本/前ClientUpdater项目](https://github.com/updater-for-minecraft/Docs/tree/c49c065a9815b35c168d7d8616abf77d510ab2e0)

## 更新记录

<!-- tabs:start -->

### **热更新包**

> 2.4版本以前的热更新包是集成到服务端以前的，如果需要，请查阅服务端更新日志

```
2.6.7f3:   (2021-04-23)
1. 修复SystemExit被当做报错处理的问题

2.6.7f2:   (2021-04-23)
1. 修复退出命令无法执行的问题

2.6.7f1:   (2021-04-15)
1. 尝试修复日志文件输出的版本不正确的问题(但失败了)

2.6.7:   (2021-04-13)
1. 支持直接加载外部WEB资源作为界面
2. 不再提供console包

2.6.6:   (2021-04-13)
1. 支持手动触发更新功能
2. 支持加载外部URL

2.6.5f2:   (2021-04-01)
1. 在日志里增加了运行环境的信息输出
2. 规范化了日志内容
3. 在JS回调中增加了indev属性，用以判断是否被打包
4. 修复了意外误伤文件的问题
5. 尝试优化了界面加载速度

2.6.5f1:   (2021-03-28)
1. 修复了Release构建文件版本号不正确的问题

2.6.4:     (2021-03-28)
1. 界面支持手动退出
2. 支持设置CEF参数:http_server
3. 支持纯文本更新路径

2.6.3:     (2021-03-24)
1. 修复了2.6.2下载中断不会弹出提示框的问题

2.6.2:     (2021-03-24)
1. 支持多文件同时下载
2. 优化了UI
3. 增加了部分异常名称翻译

2.6.1:     (2021-03-10)
1. 改进了python异常无法显示详细信息的问题
2. 优化了列表字体

2.6alpha2:     (2021-02-07)
1. 修正了一些编译选项
2. 修正了一些错误信息的时态问题

2.6alpha1:     (2021-02-07)
1. 界面使用Chromium Embedded Framework驱动，HTML+JS搭建
2. 因为加载依赖的原因，服务端client.json配置文件内容整合到客户端配置文件内
3. 如果软件运行过程中出现严重错误会在工作目录生成updater.error.log文件
4. 修复运行之前不会自动清理信号文件的问题

2.5.2:
1. 修复删除客户端多余目录时会报错的问题

2.5.1:
修复：找不到配置文件文件提示窗口显示时依赖配置文件内容的依赖问题
默认会自动创建log文件
优化了一些调试输出

2.5：
支持向客户端程序报告发生的错误，在发生错误（比如网络原因）时会返回1而不是一直返回0
支持调整网站索引文件
修改了热更新包的文件名
调整了热更新包信号文件的路径（从`.minecraft/*.signal`->`.minecraft/updater/*.signal`）
调整了log文件的位置（`.minecraft/updater.log`->`.minecraft/logs/updater.log`）

2.4.7：
支持静态部署、支持集成到启动器（如HMCL），另外注意1.4版本和之前的版本协议不能互相兼容！
```

### **客户端**

```
2.1.3:   (2020-03-11)
1. 不再依赖tasklist.exe
2. 支持隐藏console黑窗
3. 支持单实例模式（后运行会kill掉先运行的同名进程）

2.1.2:   (2020-02-07)
1. 优化控制台输出提示文字（增加强制退出的倒计时说明）

2.1.1:   (2020-02-6)
1. 优化控制台输出提示文字
2. 强制退出倒计时10min -> 3min

2.1：   (2020-01-13)
1.支持2.5版本热更新包
2.发生错误时会返回1而不是一直返回0
3.优化热更新包的调用逻辑

2.0.3（b0108）：
支持集成到启动器（如HMCL）

2.0.2（a1201）：
增加对b64编码过的URL的处理支持

2.0.1（a0922）: 
修复了空格路径无法正常启动的问题

2.0（a0915）：
首次发布2.0版本

0.1b3:
增加GUI

0.1b2:
1.修改默认端口为26542
2.修复文件太多无法更新的问题
3.去除更新完成的信息框

0.1b1:
1.支持文件夹
2.支持多个文件夹，可更新模组文件夹，材质包文件夹，配置文件文件夹等
3.支持md5验证，完全一样的文件就跳过，避免浪费流量
4.支持多地址，可与多个服务器互相同步
5.修改默认端口为22123
6.支持多行命令，一行一句
7.同步规则从服务端获取，避免反复更新客户端
```

### **静态服务端**

```
2.5:
1. 通信协议v2.1，适配热更新包2.6版本
2. client.json整合到客户端内了

2.4:
首次发布
```

### **动态服务端**

```
2.5:
1. 整合了一些文件，目录变得更干净了
2. 通信协议v2.1，适配热更新包2.6版本
3. client.json整合到客户端内了

2.3:
支持2.0版本热更新包

2.2.2：（热更新包集成版本）
修复子目录文件无法下载的问题、修复空文件夹无法创建的问题、修复无法弹出报错信息的问题、增加Content-Length缺失的情景处理、增加客户端窗口部分配置功能

2.2.1：（热更新包集成版本）
增加对b64编码过的URL的处理支持

2.2.0：（热更新包集成版本）
使用了新的配置文件逻辑，更加清晰明了、修复了报错信息框无法弹出来的问题

2.1.2：（热更新包集成版本）
重构了主代码逻辑，优化了一些进度的描述

2.1.1：（热更新包集成版本）
修复了任务栏进度条在取消最小化后会丢失的问题

2.1: （热更新包集成版本）
制作了新的界面，取代了之前的终端界面，但是大小也大了不少

2.0.1: （热更新包集成版本）
规范了客户端配置文件的命名

1.2.x：
修复无法更新客户端根目录的问题

1.1.5：
修复了文件名过长会乱码的bug和修复了忽略文件功能无效的bug，并增加了找不到核心包和更新源文件夹的提示信息，下次准备增加单独针对某个文件的更新规则的支持和以正则表达式来忽略的文件机制，另外2.1版本不能和2.2版本混用

1.1.4：
修复了一些传输机制的问题和优化部分代码效率，仓库从coding移动到github

1.1.3：
底修复了客户端文件路径中含.（尤其是.minecraft目录）时忽略文件(夹)无效的问题
美化了一些客户端显示效果

1.1.2：
优化代码，变更一些文字提示

1.1.1：
将loader分离成一个单独的项目
修复"忽略文件"功能无法生效的问题
修复"无法删除应该被删除的文件/文件夹"的问题

1.1：
添加动态执行机制
添加文件忽略机制
修改默认端口为5398
修改JRE最低要求为1.8或者更高版本
添加内置的帮助文档

1.0：(2016-06-26)
修改通信协议，默认端口更换为28445
修改GUI界面，显示数据更详细
添加修改窗口标题的功能
添加AfterRun机制

0.3：(2016-06-23)
移除以脚本来启动的机制，改为直接运行

0.2：(2016-06-22)
修复Java7无法运行的问题

0.1：(2016-06-22)
第一个版本发布

```

### **小工具**

```
1.6.0:   (2020-03-22)
1. 支持FTP/SFTP
2. 进行了配置文件分离

1.5.1:   (2020-02-7)
1. 整合了JsonGenerator的功能
2. 重写了代码，整合了所有配置文件到config.json，不再杂乱

1.4:
（测试版本未公开）

1.3：
首次发布
```

<!-- tabs:end -->

## 开源地址

<!-- tabs:start -->

### **2.0版本**

1. 文档：https://github.com/updater-for-minecraft/Docs
2. 下载地址页面：https://github.com/updater-for-minecraft/DownloadLink
3. PHP服务端：https://github.com/updater-for-minecraft/PHPServer
4. 静态服务端：https://github.com/updater-for-minecraft/StaticServer
5. 热更新包：https://github.com/updater-for-minecraft/Hotupdate
6. 客户端：https://github.com/updater-for-minecraft/Client
7. 小工具：https://github.com/updater-for-minecraft/UtilityTool

### **1.0版本（不推荐）**

1. 服务端：https://github.com/updater-for-minecraft/updater-server
2. 核心包: https://github.com/updater-for-minecraft/updater-core (核心包通常内嵌与服务端Jar之中)
3. 客户端: https://github.com/updater-for-minecraft/updater-client (只是个空壳，核心逻辑在核心包里面)
4. 规则编辑器：https://github.com/updater-for-minecraft/updater-rulesEditor

<!-- tabs:end -->