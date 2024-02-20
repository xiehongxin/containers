# Docker Note

## Volume
```shell
# 列出所有未被容器使用的 Volume
$ docker volume ls -qf dangling=true

# 删除这些未被使用的 Volume
$ docker volume rm $(docker volume ls -qf dangling=true)

```

## Registry
```shell
# 查看使用的镜像源
$ docker info

```

refer:  https://gist.github.com/y0ngb1n/7e8f16af3242c7815e7ca2f0833d3ea6