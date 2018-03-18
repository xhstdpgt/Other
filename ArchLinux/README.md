    无法打开内核设备“\\.\VMCIDev\VMX”: 系统找不到指定的文件。是否在安装 VMware Workstation 后重新引导?

    模块“DevicePowerOn”启动失败。

    未能启动虚拟机。

解决办法：
1. 打开虚拟机目录下的 *.vmx 文件（用“记事本”之类打开）；
2. 修改 vmci0.present = "TRUE" 的值为 "FALSH" ；
3. 保存后，即可重新打开虚拟机。

> ```确保虚拟机的 DHCP 和 NAT 服务已启动，如果没有，在启动后重启客户机```

# [ArchLinux](https://www.archlinux.org/)

官方文档：  
[Installation_guide](https://wiki.archlinux.org/index.php/Installation_guide)  
[Installation_guide_(简体中文)](https://wiki.archlinux.org/index.php/Installation_guide_(简体中文))

我的文档：  
[安装配置ArchLinux](install.md)  

1. 安装准备
2. 安装系统
3. 配置系统
4. 重启

安装其他软件，例如：  
方便网络配置的 ```# pacman -S net-tools``` 