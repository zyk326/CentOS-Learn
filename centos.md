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
在wondows下开启虚拟机DHCP 和 Net服务 **net start VMware DHCP Service**  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**net start VMware NET Service**  
重启虚拟机network服务&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **service network restart**

---
# 2021/03/15
    [用户名@主机 /当前目录]。  
    $ 普通账号 # 超级管理员。  
    所有命令小写 --tab命令补齐。  
    命令后加入&,开启terminal新窗口。  
    命令后加 / 可以带入命令参数。  
    命令后加; 效果和powershell 的pipe效果一样。
    dos的dir与ls一样。  
    cd 参数： . 表示当前目录  .. 表示上级目录  ~ 表示家目录  / 表示所有目录的起点，即根目录（相当于windows的盘符）。
    在linux里，如果文件以.开头，则默认隐藏。
    蓝颜色是目录，黑色是文件，绿色表示该路径有可执行的文件。 
**mv docu1.1 docu2.2** *改名 由1-2*  
**ls -a** *显示隐藏的文件与文件夹*  
**ls -l** *显示文件详细信息（只能查看文件，不能查看文件夹）*  
**cat file1** *查看file1文件内容*  
**cat file1 file2 > file3** *将文件写入file3*  
**cat file1 file2 >> file3** *将文件追加入file3*  
**more file**
**less file**  *b上一页， space下一页， q退出*
**mkdir -p ccc/ddd/eee** *创建文件目录*  
**rmdir ccc** *删除空文件夹 ccc*  
**rm -fr 文件名** *删除文件夹* 
**cp file1 file2** *拷贝file1 到file2*
**rm -r** *删东西（要询问）*  
**rm -rf** *删东西（不询问）*  
**cp -r demo1 demo2** *复制文件夹demo1 到 demo2,去掉参数-r 可以复制文件*  



---
# 2021/03/17
**ps -aux** *显示系统中全部的进程信息*  
**df** *查看系统磁盘分区情况和使用率*  
**cat /proc/meminfo** *or* **free** *查看系统内存使用情况*  
**parted工具 -- 使用 p 查看分区情况，quit退出**  
**zip -r(recurion递归) -q(安静模式quiet) -o(输出文件) filename path（绝对路径absolute path）** *把path路径下的文件打包成filename.zip*  
**du -h file** *查看file的大小，以K M G 为单位*  

---
# 2021/03/22
**touch file** *创建一个名为file的文件到当前文件夹*  
**gedit file** *对名为file的文件进行编辑， 以GUI的方式*  
**diff file1 file2** *对比两个文件的差别*  
**tar c(create)z(通过zip指令处理备份文件)v(verbose)f(指定备份文件) filename filepath** *压缩命令 czvf是参数 filename文件名 filepath文件路径*  
**tar x(extract)z(zip)v(verbose)f(file) filepath** *解压缩文件到当前路径*   
**whereis ls** *查找命令所有路径*  
**grep ls** *查找命令所在路径*   
**free** *cup内存占用情况*  
**top** **  
**date** *查看当前linux时钟*  
**cal** *日历*  
**pstree** *查看进程树*  
**kill pid** *根据pid结束进程*  
**^l** *=clear*
**uname -a** *查看版本*  
**man commit // info commit** *查看帮助手册*  
**shutdown** *关机命令， 需要参数*