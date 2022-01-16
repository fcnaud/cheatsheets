# wsl

## 网络相关

**获取主机 ip**

```shell
ip route | grep default | awk '{print $3}'
# 或者
cat /etc/resolv.conf | grep nameserver | awk '{ print $2 }'
```

**获取 wsl ip**

``` shell
hostname -I | awk '{print $1}'
```
