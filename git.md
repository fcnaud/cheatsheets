# git

## config

### 换行

```shell
# 在 windows 上设置（默认打开的），提交时把 crlf 转换成 lf，拉取时将 lf 转换成 crlf
git config --global core.autocrlf true
# 在 linux 电脑上设置，提交时把 crlf 转换成在 lf, 拉取时不转换。
git config --global core.autocrlf input
```

### 代理

```shell
# 代理
git clone -c http.proxy="http://127.0.0.1:7890" # 指定代理
git config --global http.proxy "http://127.0.0.1:1080" # 设置全局代理
git config --global --unset http.proxy # 取消全局代理
```
