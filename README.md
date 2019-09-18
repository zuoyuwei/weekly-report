# weekly-report
## ubuntu18.04 system install
### 1.进入开机界面，按F2进入启动菜单
### 2.选择UEFI开头的启动盘后，选择Install Ununtu
### 3.安装完成后无法进入ubuntu系统界面
    修改建议：在grub模式下添加nomodeset参数，告诉内核不要加载显卡而用BIOS模式直到图形界面运行
### 4.重新启动可以正常安装，同样安装在c盘目录下，分配132G看空间给ubuntu系统
### 5.安装过程选择other option
    然后根目录，/，分配内存
    设置swap分区
    然后/home分配内存
    ×××在Device for boot loader installation选项里，选择刚刚type为biosgrub的设备（刚刚作为reversed bios boot area）的设备号,例如/dev/nvmeOn1p5 ext4,继续安装×××
    然后设置用户，密码，完成安装，重启
###  6.重启之后依然选用在splash后添加nomodeset
