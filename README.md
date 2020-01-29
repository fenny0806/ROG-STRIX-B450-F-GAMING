# ROG-STRIX-B450-F-GAMING OC EFI

**电脑配置**

**CPU：AMD Ryzen 7 3700X**

**主板：ROG-STRIX-B450-F-GAMING**

**内存：十铨 夜莺 DDR4 3000Mhz**

**硬盘1：SN750 M.2 1T**

**硬盘2：三星 EVO860 256G**

**硬盘3：西数 1T**

**硬盘4：intel 545 256G**

**显卡：ROG-STRIX-RX580-O8G-GAMING**

**当前系统版本**

![image-20200129181216857](/Users/youridol/Library/Application Support/typora-user-images/image-20200129181216857.png)

------

修改"关于本机" CPU型号方法

下载好BBedit然后按下操作

1.进入恢复模式 打开终端 关闭SIP模式

终端中输入：

SIP关闭

```
csrutil disable
```

SIP开启

```
csrutil enabled
```

SIP状态查询

```
csrutil status
```

2.打开终端

终端中输入：

```
sudo -s
```

```
sudo mount -u -o rw /
```

3.然后前往文件夹输入下面目录路径

```
/System/Library/PrivateFrameworks/AppleSystemInfo.framework/Versions/A/Resources/zh_CN.lproj/
```

将目录下的"Processors.strings"赋予可写权限

3.1 右键打开"显示简介"

3.2 点击右下角的小锁，输入账户密码。

3.3 讲几个用户权限都选选择为读和写

4.用BBEdit 打开"Processors.strings"

找到原来在关于本机显示的CPU型号然后修改成你自己的CPU型号保存即可。