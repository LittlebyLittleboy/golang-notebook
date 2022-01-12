### Go语言的开发工具

---
**第一部分：开发工具对比**
- **<a href="#1.1">1.1.Goland编译器</a>**
- **<a href="#1.2">1.2.VS Code编译器</a>**
- **<a href="#1.3">1.3.Vim Go编译器</a>**
- **<a href="#1.4">1.4.Sublime编译器</a>**

**第二部分：Goland安装**
- **<a href='#2.1'>2.1.Win7安装Goland</a>**
- **<a href='#2.2'>2.2.MacOS安装Goland</a>**
- **<a href='#2.3'>2.3.Linux安装Goland</a>**
- **<a href='#2.4'>2.4.Goland快捷键使用</a>**

**第三部分：VS Code安装**
- **<a href='#3.1'>3.1.Win7安装VS Code</a>**
- **<a href='#3.2'>3.2.MacOS安装VS Code</a>**
- **<a href='#3.3'>3.3.Linux安装VS Code</a>**
- **<a href='#3.4'>3.4.VS Code快捷键使用</a>**

**第四部分：Sublime安装**
- **<a href='#4.1'>4.1.Win7安装Sublime</a>**
- **<a href='#4.2'>4.2.MacOS安装Sublime</a>**
- **<a href='#4.3'>4.3.Linux安装Sublime</a>**

---
**<a id="1.1">1.1.Goland编译器</a>**
```
简介：GoLand是一个专为Go开发者设计的跨平台IDE，是由商业公司JetBrains提供的闭源收费的Go语言开发的集成开发环境。

优点：Goland具有强大的代码洞察，实时错误检测和修复建议、支持一步撤消的快速安全重构、智能代码补全、无用代码检测和文档提示；Goland探索和理解团队、遗留或外来项目需要花费大量时间和精力。 GoLand 代码导航可以帮助您快速切换至被屏蔽的方法、实现、用法、声明，或通过类型实现的接口；Goland强大的内置工具帮助运行和调试应用程序。 无需任何额外的插件或配置工作即可编写和调试测试，并直接在 IDE 中测试应用程序；GoLand 开箱即支持 Git、GitHub 和 Mercurial。 通过用户安装的插件支持 Perforce、ClearCase 等；Goland如果没有丰富的工具集，GoLand 不会成为真正的 IDE，除了核心 Go 开发外，它还支持 JavaScript、TypeScript、NodeJS、SQL、数据库、Docker、Kubernetes 和 Terraform。 这些功能组合起来，使其完美适用于任何任务，无论是现代 Web 应用程序还是开发运维工具。

缺点：Goland是闭源收费的IDE，资源消耗较大，占用内存较大。
```

**<a id="1.2">1.2.VS Code编译器</a>**
```
简介：VS Code由微软开发的一款功能强大的现代化轻量级代码编辑器IDE，免费开源。通过它强大的插件扩展能力，VS Code几乎支持主流语言的项目开发。

优点：VS Code是免费开源的编译器，占用内存低，启动速度较快，丰富的插件功能支持，全平台，内置了对JavaScript, TypeScript and Node.js,C++, C#, Python, PHP等语言的强大支持。

缺点：VS Code每次安装都需要重新安装配置插件，相比Goland编译器稳定性较弱。
```

**<a id="1.3">1.3.Vim Go编译器</a>**
```
简介：Vim应该是一款文本编辑器，但它却拥有了很多不该属于文本编辑器的能力，比如单词补全、ctags标签跳转、窗口分隔、崩溃文件恢复、文件diff、400多种文本高亮等。最重要的一点是，Vim有一套自己的脚本语言，这为它通过插件扩展自己的能力提供了可能；将Vim扩展成一款适合自己使用的GO IDE，不仅要编写许多复杂的配置与脚本，还需要各种插件的相互配合，才能实现我们的目标。比如前面介绍的那些IDE的常见功能，在Vim中都要逐一配置实现。

优点：Vim编译器占用资源较少，启动运行速度较快。

缺点：Vim支持插件扩展，但它要集成出VS Code的体验还是非常困难的。
```

**<a id="1.4">1.4.Sublime编译器</a>**
```
简介：Sublime是一个强大的文本编译器，而它的编码能力也是插件扩展来的。GoSublime就是为Sublime扩展GO功能的插件。

优点：Sublime编译器占用资源较少，启动运行速度较快。

缺点：Sublime支持插件扩展，但它要集成出VS Code的体验还是非常困难的。
```

**<a id='2.1'>2.1.Win7安装Goland</a>**
```
①.官网地址: https://www.jetbrains.com/go/,如果无法访问,需要科学上网进行下载。
```

```
②.Goland并不像Idea和Pycharm那样分为专业版和社区版,目前只有收费版,提供 30 天免费试用,试用到期后可以选择购买正版也可以上淘宝购买激活码或网上寻求破解版。
```

```
③。进入网站主页后，直接点击页面中间的Download按钮后就会自动识别当前系统进行下载,也可以点击右上角的Download按钮自行选择目标平台进行下载。
```
![Goland](https://www.showdoc.cc/server/api/common/visitfile/sign/53a6218e715d0c137bf30030c8a33fdb?showdoc=.jpg)

```
④.Windows版本安装比较简单，直接双击可执行文件，默认安装即可，默认安装位置是：C:\Program Files\JetBrains\GoLand 2019.3.1
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/602f94021d7d3efaefd530e433b777ab?showdoc=.jpg)

**<a id='2.2'>2.2.MacOS安装Goland</a>**
```
①.官网地址: https://www.jetbrains.com/go/,如果无法访问,需要科学上网进行下载。
```

```
②.Goland并不像Idea和Pycharm那样分为专业版和社区版,目前只有收费版,提供 30 天免费试用,试用到期后可以选择购买正版也可以上淘宝购买激活码或网上寻求破解版。
```

```
③。进入网站主页后，直接点击页面中间的Download按钮后就会自动识别当前系统进行下载,也可以点击右上角的Download按钮自行选择目标平台进行下载。
```
![Goland](https://www.showdoc.cc/server/api/common/visitfile/sign/53a6218e715d0c137bf30030c8a33fdb?showdoc=.jpg)

```
④.Mac电脑,安装Goland更为简单,直接下载拖动到Application分类,连安装目录都不用选择。
```

**<a id='2.3'>2.3.Linux安装Goland</a>**
```
①.下载Goland安装包：
sudo wget -P /opt https://download.jetbrains.8686c.com/go/goland-2019.3.2.tar.gz
```
```
②.解压Goland安装包：
sudo tar -xvf goland-2019.3.2.tar.gz -C /usr/local
```
```
③.修改Goland执行权限：
sudo chmod -R 755 /usr/local/goland-2019.3.2
```
```
④.执行Goland程序开启：
sudo ./goland.sh
```

**<a id='2.4'>2.4.Goland快捷键使用</a>**
```
①.Goland快捷键设置
步骤：File(文件)--->Settings(设置)--->Editor Actions(编辑器操作)

②.Goland快捷键使用
```
**文件操作相关的快捷键:**

| 组合键 | 功能 |
| --- | --- |
|Ctrl + E|打开最近浏览过的文件|
|Ctrl + N|快速打开某个 struct 结构体所在的文件|
|Ctrl + Shift + N|快速打开文件|
|Shift + F6|重命名文件夹、文件、方法、变量名等|

**代码格式化相关的快捷键:**

| 组合键 | 功能 |
| --- | --- |
|Ctrl + Alt + L|格式化代码|
|Ctrl + 空格|代码提示|
|Ctrl + /|单行注释|
|Ctrl + Shift + /|多行注释|
|Ctrl + B 或 F4|快速跳转到结构体或方法的定义位置（需将光标移动到结构体或方法的名称上）|
|Ctrl +“+ 或 -”|可以将当前（光标所在位置）的方法进行展开或折叠|

**查找和定位相关的快捷键:**

| 组合键 | 功能 |
| --- | --- |
|Ctrl + R|替换文本|
|Ctrl + F|查找文本|
|Ctrl + Shift + F|全局查找
|Ctrl + G|显示当前光标所在行的行号|
|Ctrl + Shift + Alt + N|查找类中的方法或变量|

**编辑代码相关的快捷键:**

| 组合键 | 功能 |
| --- | --- |
|Ctrl + J|快速生成一个代码片段|
|Shift+Enter|向光标的下方插入一行，并将光标移动到该行的开始位置|
|Ctrl + X|删除当前光标所在行|
|Ctrl + D|复制当前光标所在行|
|Ctrl + Shift + 方向键上或下|将光标所在的行进行上下移动（也可以使用 Alt+Shift+方向键上或下）|
|Alt + 回车|自动导入需要导入的包|
|Ctrl + Shift + U|将选中的内容进行大小写转化|
|Alt + Insert|生成测试代码|
|Alt + Up/Down|快速移动到上一个或下一个方法|
|Ctrl + Alt + Space|类名或接口名提示（代码提示）|
|Ctrl + P|提示方法的参数类型（需在方法调用的位置使用，并将光标移动至( )的内部或两侧）|

**编辑器相关的快捷键:**

| 组合键 | 功能 |
| --- | --- |
|Ctrl + Alt + left/right|返回至上次浏览的位置|
|Alt + left/right|切换代码视图|
|Ctrl + W|快速选中代码|
|Alt + F3|逐个向下查找选中的代码，并高亮显示|
|Tab|	代码标签输入完成后，按 Tab，生成代码|
|F2 或 Shift + F2|快速定位错误或警告|
|Alt + Shift + C|查看最近的操作|
|Alt + 1|快速打开或隐藏工程面板|

**<a id='3.1'>3.1.Win7安装VS Code</a>**
```
①.先到下载地址去选择合适自己系统的VS Code安装软件：https://code.visualstudio.com/download
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/ba9e4b87d9dd6668b040b5bdbb94a994?showdoc=.jpg)

```
②.演示如何在Windows下安装使用VS Code
```
![](https://www.showdoc.cc/server/api/common/visitfile/sign/3d162704b8c8e501078ee69ea57f2dac?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/535ae17f9423c6ba2514d7297c5686a8?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/daf6348fff7a45f4209b08a848061d2e?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/84290ee91f4bd82d2914bb8c09dabb8f?showdoc=.jpg)
**<a id='3.2'>3.2.MacOS安装VS Code</a>**
![](https://www.showdoc.cc/server/api/common/visitfile/sign/ceaf91694b498cea503fc7baab43428c?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/ab8d23b57b21725e0c135ec02b10409a?showdoc=.jpg)
**<a id='3.3'>3.3.Linux安装VS Code</a>**
![](https://www.showdoc.cc/server/api/common/visitfile/sign/3d062815003e0c2da421c98d7cd757ba?showdoc=.jpg)
![](https://www.showdoc.cc/server/api/common/visitfile/sign/d46cc43cbe59fe25341f9e327f77c415?showdoc=.jpg)

**<a id='3.4'>3.4.VS Code快捷键使用</a>**

**面板窗口 Board Windows**

|组合键 Key|功能 Function|
| --- | --- |
|Ctrl + Shift + P，F1|显示命令面板 Show Command Palette|
|Ctrl + P|快速打开 Quick Open|
|Ctrl + Shift + N|新窗口/实例 New window/instance|
|Ctrl + Shift + W|关闭窗口/实例 Close window/instance|

**基础编辑 Basic editing**

|组合键 Key|功能 Function|
| --- | --- |
|Ctrl+X|剪切行（空选定） Cut line (empty selection)|
|Ctrl+C|复制行（空选定）Copy line (empty selection)|
|Alt+ ↑ / ↓|向上/向下移动行 Move line up/down|
|Shift+Alt + ↓ / ↑|向上/向下复制行 Copy line up/down|
|Ctrl+Shift+K|删除行 Delete line|
|Ctrl+Enter|在下面插入行 Insert line below|
|Ctrl+Shift+Enter|在上面插入行 Insert line above|
|Ctrl+Shift+\|跳到匹配的括号 Jump to matching bracket|
|Ctrl+] / [|缩进/缩进行 Indent/outdent line|
|Home|转到行首 Go to beginning of line|
|End|转到行尾 Go to end of line|
|Ctrl+Home|转到文件开头 Go to beginning of file|
|Ctrl+End|转到文件末尾 Go to end of file|
|Ctrl+↑ / ↓|向上/向下滚动行 Scroll line up/down|
|Alt+PgUp / PgDown|向上/向下滚动页面 Scroll page up/down|
|Ctrl+Shift+[|折叠（折叠）区域 Fold (collapse) region|
|Ctrl+Shift+]|展开（未折叠）区域 Unfold (uncollapse) region|
|Ctrl+K Ctrl+[|折叠（未折叠）所有子区域 Fold (collapse) all subregions|
|Ctrl+K Ctrl+]|展开（未折叠）所有子区域 Unfold (uncollapse) all subregions|
|Ctrl+K Ctrl+0|折叠（折叠）所有区域 Fold (collapse) all regions|
|Ctrl+K Ctrl+J|展开（未折叠）所有区域 Unfold (uncollapse) all regions|
|Ctrl+K Ctrl+C|添加行注释 Add line comment|
|Ctrl+K Ctrl+U|删除行注释 Remove line comment|
|Ctrl+/|切换行注释 Toggle line comment|
|Shift+Alt+A|切换块注释 Toggle block comment|
|Alt+Z|切换换行 Toggle word wrap|

**导航 Navigation**

|组合键 Key|功能 Function|
| --- | --- |
|Ctrl + T|	显示所有符号 Show all Symbols|
|Ctrl + G|	转到行... Go to Line...|
|Ctrl + P|	转到文件... Go to File...|
|Ctrl + Shift + O|	转到符号... Go to Symbol...|
|Ctrl + Shift + M|	显示问题面板 Show Problems panel|
|F8|	转到下一个错误或警告 Go to next error or warning|
|Shift + F8|	转到上一个错误或警告 Go to previous error or warning|
|Ctrl + Shift + Tab|	导航编辑器组历史记录 Navigate editor group history|
|Alt + ←/→|	返回/前进 Go back / forward|
|Ctrl + M|	切换选项卡移动焦点 Toggle Tab moves focus|

**搜索和替换 Search and replace**

|组合键 Key|功能 Function|
| --- | --- |
|Ctrl + F|	查找 Find|
|Ctrl + H|	替换 Replace|
|F3 / Shift + F3|	查找下一个/上一个 Find next/previous|
|Alt + Enter|	选择查找匹配的所有出现 Select all occurences of Find match|
|Ctrl + D|	将选择添加到下一个查找匹配 Add selection to next Find match|
|Ctrl + K Ctrl + D|	将最后一个选择移至下一个查找匹配项 Move last selection to next Find match|
|Alt + C / R / W|	切换区分大小写/正则表达式/整个词 Toggle case-sensitive / regex / whole word|

**多光标和选择 Multi-cursor and selection**

|组合键 Key|功能 Function|
| --- | --- |
|Alt +单击|	插入光标 Insert cursor|
|Ctrl + Alt +↑/↓|	在上/下插入光标 Insert cursor above / below|
|Ctrl + U|	撤消上一个光标操作 Undo last cursor operation|
|Shift + Alt + I|	在选定的每一行的末尾插入光标 Insert cursor at end of each line selected|
|Ctrl + I|	选择当前行 Select current line|
|Ctrl + Shift + L|	选择当前选择的所有出现 Select all occurrences of current selection|
|Ctrl + F2|	选择当前字的所有出现 Select all occurrences of current word|
|Shift + Alt + →|	展开选择 Expand selection|
|Shift + Alt + ←|	缩小选择 Shrink selection|
|Shift + Alt + （拖动鼠标）|	列（框）选择 Column (box) selection|
|Ctrl + Shift + Alt +（箭头键）|	列（框）选择 Column (box) selection|
|Ctrl + Shift + Alt + PgUp / PgDown|	列（框）选择页上/下 Column (box) selection page up/down|

**丰富的语言编辑 Rich languages editing**

|组合键 Key|功能 Function|
| --- | --- |
|Ctrl + 空格 【atl + /】|	触发建议 Trigger suggestion|
|Ctrl + Shift + Space|	触发器参数提示 Trigger parameter hints|
|Tab	Emmet| 展开缩写 Emmet expand abbreviation|
|Shift + Alt + F|	格式化文档 Format document|
|Ctrl + K Ctrl + F|	格式选定区域 Format selection|
|F12|	转到定义 Go to Definition|
|Alt + F12|	Peek定义 Peek Definition|
|Ctrl + K F12|	打开定义到边 Open Definition to the side|
|Ctrl + .|	快速解决 Quick Fix|
|Shift + F12|	显示引用 Show References|
|F2	|重命名符号 Rename Symbol|
|Ctrl + Shift + . /，|	替换为下一个/上一个值 Replace with next/previous value|
|Ctrl + K Ctrl + X|	修剪尾随空格 Trim trailing whitespace|
|Ctrl + K M|	更改文件语言 Change file language|

**编辑器管理 Editor management**

|组合键 Key|功能 Function|
| --- | --- |
|Ctrl+F4, Ctrl+W|	关闭编辑器 Close editor|
|Ctrl+K F|	关闭文件夹 Close folder|
|Ctrl+\|	拆分编辑器 Split editor|
|Ctrl+ 1 / 2 / 3|	聚焦到第1，第2或第3编辑器组 Focus into 1st, 2nd or 3rd editor group|
|Ctrl+K Ctrl+ ←/→|	聚焦到上一个/下一个编辑器组 Focus into previous/next editor group|
|Ctrl+Shift+PgUp / PgDown|	向左/向右移动编辑器 Move editor left/right|
|Ctrl+K ← / →|	移动活动编辑器组 Move active editor group|

**文件管理 File management**

|组合键 Key|功能 Function|
| --- | --- |
|Ctrl+N|	新文件 New File|
|Ctrl+O|	打开文件... Open File...|
|Ctrl+S|	保存 Save|
|Ctrl+Shift+S|	另存为... Save As...|
|Ctrl+K S|	全部保存 Save All|
|Ctrl+F4|	关闭 Close|
|Ctrl+K Ctrl+W|	关闭所有 Close All|
|Ctrl+Shift+T|	重新打开关闭的编辑器 Reopen closed editor|
|Ctrl+K|	输入保持打开 Enter Keep Open|
|Ctrl+Tab|	打开下一个 Open next|
|Ctrl+Shift+Tab|	打开上一个 Open previous|
|Ctrl+K P|	复制活动文件的路径 Copy path of active file|
|Ctrl+K R|	显示资源管理器中的活动文件 Reveal active file in Explorer|
|Ctrl+K O|	显示新窗口/实例中的活动文件 Show active file in new window/instance|

**显示 Display**

|组合键 Key|功能 Function|
| --- | --- |
|F11|	切换全屏 Toggle full screen|
|Shift+Alt+1|	切换编辑器布局 Toggle editor layout|
|Ctrl+ = / -|	放大/缩小 Zoom in/out|
|Ctrl+B|	切换侧栏可见性 Toggle Sidebar visibility|
|Ctrl+Shift+E|	显示浏览器/切换焦点 Show Explorer / Toggle focus|
|Ctrl+Shift+F|	显示搜索 Show Search|
|Ctrl+Shift+G|	显示Git Show Git|
|Ctrl+Shift+D|	显示调试 Show Debug|
|Ctrl+Shift+X|	显示扩展 Show Extensions|
|Ctrl+Shift+H|	替换文件 Replace in files|
|Ctrl+Shift+J|	切换搜索详细信息 Toggle Search details|
|Ctrl+Shift+C|	打开新命令提示符/终端 Open new command prompt/terminal|
|Ctrl+Shift+U|	显示输出面板 Show Output panel|
|Ctrl+Shift+V|	切换Markdown预览 Toggle Markdown preview|
|Ctrl+K V|	从旁边打开Markdown预览 Open Markdown preview to the side|

**调试 Debug**

|组合键 Key|功能 Function|
| --- | --- |
|F9|	切换断点 Toggle breakpoint|
|F5|	开始/继续 Start/Continue|
|Shift+F5|	停止 Stop|
|F11 / Shift+F11|	下一步/上一步 Step into/out|
|F10|	跳过 Step over|
|Ctrl+K Ctrl+I|	显示悬停 Show hover|

**集成终端 Integrated terminal**

|组合键 Key|功能 Function|
| --- | --- |
|Ctrl+`|	显示集成终端 Show integrated terminal|
|Ctrl+Shift+`|	创建新终端 Create new terminal|
|Ctrl+Shift+C|	复制选定 Copy selection|
|Ctrl+Shift+V|	粘贴到活动端子 Paste into active terminal|
|Ctrl+↑ / ↓|	向上/向下滚动 Scroll up/down|
|Shift+PgUp / PgDown|	向上/向下滚动页面 Scroll page up/down|
|Ctrl+Home / End|	滚动到顶部/底部 Scroll to top/bottom|

**<a id='4.1'>4.1.Win7安装Sublime</a>**

**<a id='4.2'>4.2.MacOS安装Sublime</a>**

**<a id='4.3'>4.3.Linux安装Sublime</a>**

---
**参考网络文章**
[**Golang开发的IDE**](https://www.zhihu.com/question/326149717/answer/698600973)
[**Goland破解版IDE**](https://studygolang.com/topics/7615?fr=sidebar)
[**Goland快捷键**](http://c.biancheng.net/view/6216.html)

---
**作者：张电永**
**时间：2020-02-06 22:33:29 星期四**

