# 命令
## 系统语言篇  
**echo $LANG** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  *查看当前系统使用的语言*  
**locale** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*查看当前系统已有的语言*   
**vi /etc/sysconfig/i18n**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*修改语言配置(低优先级)*  
**vi /etc/profile | 加入export LANG=en_US.UTF-8**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*修改语言 配置（高优先级）*  
**vi ~/.bashrc | 加入export LANG=en_US.UTF-8**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*修改语言配置（中优先级）*

---

## 系统权限篇
**sudo root** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *进入root权限*  
**reboot** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*重启*

---

## 网络连接篇
进入root权限   
**ls /etc/sysconfig/network-scripts**   
**vi /etc/sysconfig/network-scripts/ifcfg-ensxxx**  
修改bootproto 为"dhcp"，修改onboot为"yes"  
在wondows下开启虚拟机DHCP 和 Net服务 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **net start VMware DHCP Service**  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**net start VMware NET Service**  
重启虚拟机network服务&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **service network restart**

---
