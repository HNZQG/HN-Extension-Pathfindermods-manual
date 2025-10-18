## Pathfinder的安装及好处

https://github.com/Arkhist/Hacknet-Pathfinder
你可以在浏览器打开上述网址，下载并安装。
你也可以选择在我们的Q群940056115中
下载群文件的PathfinderInstaller.exe运行安装
选择文件夹，请选择hacknet所在目录

## 自动安装

如果您使用的是Windows，建议您使用安装程序。请从这里执行。只要运行安装程序，它会自动找到你的Hacknet文件夹，然后点击安装。从Steam启动Hacknet将会启动Pathfinder(在Windows上)！
如果您决定使用py来installer(或者你只是在Linux上并且必须使用它)记住它需要在你运行它之前安装python3和tk。
如果你在Linux上，一旦安装完成，确保自己+x StartPathfinder.sh。
要卸载，只需重新打开安装程序，然后单击卸载。这将清除安装程序所做的所有更改，同时也将删除你所有的插件。

## 手动安装

从Github下载Hacknet Pathfinder的压缩文件。
将内容提取到Hacknet的文件夹中。
运行PathfinderPatcher.exe(对于Linux用户，mono PathfinderPatcher.exe)。
(对于Linux)将Hacknet.bin.x86(_64)复制到HacknetPathfinder.bin.x86(_64)并使StartPathfinder.sh执行。
在Windows上运行HacknetPathfinder.exe或在Linux上运行StartPathfinder.sh来启动Pathfinder。

目前使用Pathfinder的较早扩展有 WnCry 和 小A的Tempest 以及ZQG 的 SR.OS Overlapping 可以适当的学习借鉴

它的主要好处在于它可以比原版更精确的检测到bug，顾名思义，它对扩展的判定更严。这有利于扩展作者去发现bug，解决bug。
其他好处在此处不进行列举。

## 游戏在加载前就崩溃了！(仅适用于Windows)

如果游戏在加载前崩溃，或者您在控制台中看到一个错误指出：试图从网络位置加载一个程序集，这将导致该程序集使用旧的.NET框架。
解决方法:在Windows上，进入BepInEx/core和BepInEx/plugins文件夹，打开每个DLL的属性，点击底部的Unblock复选框。
或者，在PowerShell运行此命令get-childitem "<Hacknet文件夹的路径>" | unblock-file
