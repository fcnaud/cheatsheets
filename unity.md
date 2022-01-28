# Unity

**定位.so崩溃**

* 在 NDK 目录下找到 `arm-linux-androideabi-addr2line.exe`。

```shell
arm-linux-androideabi-addr2line -C -f -e so库文件的路径 具体的内存地址
```
