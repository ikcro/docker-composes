

- [Dockerfile](Dockerfile) ： 添加延时队列插件的Image

```shell
# 构建镜像
docker build --platform linux/amd64 -t rabbitmq:3.12-management-alpine .
```

```shell
# 运行容器
docker-compose -f docker-compose.yml up -d
```