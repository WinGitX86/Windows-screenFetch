Windows screenFetch

<img src="screenshots/ss.png"/>

ScreenFetch <hr>

screenFetch 最初是一个“Bash 截图信息工具”。简单来说，它可以在终端中显示关于你系统的详细信息，并且会附带检测到的 Linux 发行版的 ASCII 艺术标志。

这个工具本身无法在 Windows 上原生运行，这个项目是我尝试提供一个不需要在 Windows 上获取 Linux 环境的解决方案。

<a href="https://github.com/KittyKatt/screenFetch"> 原始项目可以在 KittyKatt 的仓库中找到。</a>

有何不同？ <hr>

原始的 screenFetch 需要系统支持 bash，因此无法在 Windows 上原生使用！这是一个小规模项目，旨在 Windows 上“模仿” screenFetch 的行为。

Windows screenFetch 是一个 PowerShell 脚本，而不是 Bash 程序。因此，不需要像 <a href="https://www.cygwin.com/">Cygwin</a> 或 <a href="http://www.mingw.org/wiki/msys">MinGW</a> 这样的类 Linux 环境。它可以在 Windows 上作为 PowerShell 脚本原生运行，在 PowerShell 或命令提示符控制台中执行。

由于此工具仅设计用于 Windows 环境，因此不支持调用任何 Linux 发行版 ASCII 艺术标志的参数。

安装 <hr>

Windows screenFetch 可通过 <a href="https://www.powershellgallery.com/packages/windows-screenfetch">Powershell Gallery</a> 获取和管理。

<b>PowerShell</b>

<b>注意</b>：如果你在它上传到 PowerShell Gallery 之前使用过 windows-screenfetch，你需要先删除本地实例和相关环境变量，然后再运行以下安装命令。

安装模块后，只需运行 <code>Screenfetch</code> 命令，就可以使用了。

<b>~~命令提示符~~</b>

不再支持

使用参数 <hr>

· -distro 参数允许你指定要显示的 ASCII 标志
· 目前可用的替代选项是苹果标志，请参阅 AsciiArtGenerator 了解可能的扩展

<br>
<img src="screenshots/mac.png">

故障排除 <hr>

如果你按照安装步骤操作，但遇到以下错误：

```
文件 C:\<你的路径>\screenfetch.ps1 没有数字签名。
系统将不会执行该脚本。
```

一个常见的解决方法是在具有管理员权限的 shell 中运行 PowerShell 命令 Set-ExecutionPolicy Unrestricted。

联系我 <hr>

以下是我最活跃的两个社交平台

· julianchow@outlook.com
· https://twitter.com/JulianChow94

该仓库不提供发行版下载