# R6566BB1C-kitsune

警告！您使用的是Magisk的非官方版本，Magisk作者不支持该版本。此版本可能包含不稳定的修改，可能会损害您的设备或危及您的安全。不要向Magisk官方渠道报告任何问题或请求任何帮助。如果你使用这个版本，但不知道这是一个非官方版本，请切换到github.com/topjohnwu/Magisk的官方Magisk        
 使用unix域套接字通信 总是将magisk媒体夹插入/system/bin 在/system中使用magisk安装方法时，请始终使用/sbin作为magisk tmp 与官方Magisk不同[Zygisk]通过ptrace init注入受精卵         
[常规]禁用Zygisk时，使用MagiskHide隐藏 [常规]支持在模块的预初始化中挂载 [常规]支持将Magisk安装到/system中(用于模拟器)       
## 信用 
Kitsune Mask使用了ZygiskNext的一些代码，这是一个由Dr-TSNG和5ec1cff编写的开源项目，并在GPL-veersion 3.0下获得许可。ZygiskNext为KernelSU提供了Zygisk和Zygisk API支持的独立实现，并取代了Magisk的内置Zygisk。      

Magisk上游水平 头提交:ecb31ee      

# R6566BB1C-kitsune

WARNING! You are using an unofficial version of Magisk that is not officially supported by the Magisk author. This version may contain unstable modifications that could harm your device or compromise your security. Do not report any issues or request any help from official Magisk channels. If you use this version but do not know this is an unofficial version, please switch to the official Magisk at github.com/topjohnwu/Magisk

Use unix domain socket communication
Always inject magisk bins to /system/bin
Always use /sbin as the magisk tmp when using the magisk installation method into /system
Diffs to official Magisk
[Zygisk] Inject zygote by ptrace init (*)
[General] Use MagiskHide to hide when Zygisk is disabled
[General] Support mounting in pre-init for modules
[General] Support install Magisk into /system (for emulators)
## Credits
(*) Kitsune Mask is using some code from ZygiskNext, it is an open source project written by Dr-TSNG and 5ec1cff and licensed under GPL-veersion 3.0. ZygiskNext offers a standalone implementation of Zygisk and Zygisk API support for KernelSU and replaces Magisk’s built-in Zygisk.
Magisk upstream level
HEAD commit: ecb31ee