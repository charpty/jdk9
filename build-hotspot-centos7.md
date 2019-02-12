## 环境
操作系统：CentOS Linux release 7.4.1708
内核：Linux iZuf6avr5vrs9psxbmmt3iZ 3.10.0-693.17.1.el7.x86_64 #1 SMP Thu Jan 25 20:13:58 UTC 2018 x86_64 x86_64 x86_64 GNU/Linux
代码：https://hg.openjdk.java.net/jdk9/jdk9


## 代码下载
如果通过hg clone则是非常痛苦的，容易掉线且非常慢
建议先zip下载最外层目录，再一个个下载内层目录（hotspot、jdk、jaxp、corba等），成功率百分之百

## 编译

``` bash
yum install -y elfutils-libelf-devel freetype-devel alsa-lib-devel cups-devel libXi-devel gcc gcc-c++ libstdc++ libX*
sh configure --with-debug-level=slowdebug --disable-warnings-as-errors
make hotspot
```
