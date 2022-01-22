# Fish

## shell 命令

## 语法

### 使用变量

```shell
set -l name value       # 设置局部变量，类似于 local name = value

# e.g.
set -l name fcnaud
echo hello $name        # hello fcnaud
```

### 条件判断

### 环境变量

```shell
set -x name value       # 设置环境变量，只对当前 shell 生效
set -gx name value      # 全局生效
set -Ux name value      # 全局生效，重启依然生效

# e.g.
set -gx http_proxy http://localhost:8080

set -e name             # 删除环境变量

# e.g.
set -e http_proxy

set PATH /new/path $PATH # 设置 Path
```

### 设置 alias

```shell
alias abbr="command"

# e.g.
alias vim="nvim"
alias la="ls -al"
```

## Snippet

- sudo 执行上一条命令

```shell
function sdl
  eval command sudo $history[1]
end
```

**参考链接**
- [使用 fish 的一些注意点 - 知乎 赵启明](https://zhuanlan.zhihu.com/p/26157081)
