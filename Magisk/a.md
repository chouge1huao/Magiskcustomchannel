# alpha更新日志
重大行为变化：magiskd现在位于独立挂载命名空间，这也是su的全局挂载命名空间。 大部分su用例不会受到影响，如需init挂载命名空间，改为su -t 1。         

重大行为变化：magiskd内部挂载点对外隐藏，并于不再使用后卸载。    

## Magisk (577483fd-alpha)     
[App] 还原boot镜像后删除备份文件    
[General] 不自动解锁设备块     
[App] 不主动请求权限     
[General] 保留ROOTOVL临时文件     
[Zygisk] 卸载挂载不跳过com.android.systemui      
[App] 通过appcenter检查和下载更新       
[App] 添加遥测 https://t.me/s/magiskalpha/473      
[General] 重写MagiskHide，采用logcat实现。日志系统不正常的设备不要开启此功能。      
[General] 移除addon.d支持      
[General] 隐藏并清理magiskd内部挂载点      
[General] 取消/system/etc/hosts可写的例外,请修改/data/adb/modules/hosts/system/etc/hosts       
[Zygisk] 重构加载方式，与riru类似      
[MagiskSU] 支持移除权能     
[General] 支持用户限制Root权能 [使用旧版libsu的应用会错误识别为无root]     
[App] 添加备用DoH服务器        
[General] 安全模式不再挂载su到/system/bin/su，adb shell请使用/debug_ramdisk/su     
[Zygisk] 修复fd清理逻辑      
# 上游更新日志
## 2023.11.5 Magisk v26.4     
[MagiskBoot] Don't pad zeros if signed boot image is larger       
[MagiskPolicy] Fix genfscon and filename_trans     
[MagiskPolicy] Fix bug in libsepol      
[Zygisk] Fix and simplify file descriptor sanitization logic     
[App] Prevent OOM when patching AP tarfiles     
[App] Fix bug  in device configuration detection      
[Daemon] Fix certificate parsing of APKs      
[General] Fix logging errors from C++ code being ignored     