## 0fe46c5a-delta 每夜构建

-应该修复启动回路

Canary和Debug构建自相同的源代码。调试版本有更详细的日志，适合调试。Canary版本具有更少的日志，比Debug更稳定，并且适合大多数常见用途

如果你喜欢我的作品，可以在【PayPal/husky DG】(http://PayPal . me/husky DG)给我捐款

### 与官方Magisk不同

- [General]使用“Unmount modules”按模块管理已修改文件的可见性
- [Manager]支持安装到仿真器的系统分区中
-[常规]为` addon.d `将所需文件复制到`/system '
- [Manager]在中文ROM的语言设置中显示所有支持的语言
-[模块]支持无系统删除模块的文件或文件夹
-[常规]内置引导环路保护，通过magisk模块保护系统免受引导环路影响
- [General]调整F2FS驱动程序以修复未加密的f2fs `/data `上的问题
- [MagiskInit]支持在“初始化”开始之前替换系统文件的预初始化挂载
-

## 0fe46c5a-delta Nightly build

- Should fix bootloop

Canary and Debug are built from the same source code.  Debug builds have more detailed logs and are suitable for debugging. Canary builds have less logs, are more stable than Debug, and are suitable for most common uses

If you like my work, you can donate me at [PayPal/HuskyDG](http://paypal.me/huskydg)

### Diffs to official Magisk

- [General] Use "Unmount modules" to manage the visibility of modified files by module
- [Manager] Support installing into system partition for emulator
- [General] Copy required files to `/system` for `addon.d`
- [Manager] Show all supported languages in Language settings for Chinese ROM
- [Module] Support systemless deleting files or folders for modules
- [General] Built-in Bootloop Protection to protect system from bootloop by magisk module
- [General] Tune F2FS driver to fix problem on unencrypted f2fs `/data`
- [MagiskInit] Support Pre-Init mount that replaces system files before `init` starts
- [MagiskInit] Support loading custom rc script from pre-init directory
- [Modules] Support magic mount more partitions (`my_*`, `odm`, `optics`, `prism`)
- [Zygisk]: Switch to use native bridge by 5ec1cff
- [Module] Live patch `sepolicy.rule` if it is not found in `sepolicy.rules` directory
- [MagiskSU] Do not use local socket path
- [Module] Always inject magisk bins
- [MagiskInit] Introduce `early-mount.d/v2` to support pre-Init mount per module

### Magisk upstream

- Sync upstream source code to 350d0d600
