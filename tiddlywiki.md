# TiddlyWiki

- 创建

```shell
tiddlywiki wikiName --init server
```

- 启动

```shell
tiddlywiki path --listen             # 启动，默认端口
tiddlywiki path --listen port=8000   # 指定端口

# 本地 nodejs 版本启动时，激活两个依赖的插
tiddlywiki path +plugins/tiddlywiki/filesystem +plugins/tiddlywiki/tiddlyweb --listen
```
