# 如何绕过硬件限制强行安装Windows11系统
Shift+F10 #打开PowerShell窗口  
regedit #输入之后进入注册表  

HKEY_LOCAL_MACHINE\SYSTEM\Setup #打开Setup目录  

在Setup目录中 新建-> 项 ->将项重命名为 LabConfig  

在此项中新建 DWORD(32位)值;命名为 BypassTPMCheck;双击修改值为00000001(7个0,1个1)  

再新建 DWORD(32位)值;命名为 BypassSecureBootCheck;双击修改值为00000001(7个0,1个1)  

返回windows11安装程序的上一步正常安装  

参考YouTube视频：
https://www.youtube.com/watch?v=ktej0CDSQik
