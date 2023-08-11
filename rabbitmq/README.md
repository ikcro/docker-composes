

- [Dockerfile](Dockerfile) ： 添加延时队列插件的Image

```shell
# 构建镜像
docker build --platform linux/amd64 -t rabbitmq:3.12-management-alpine .
```

```shell
# 运行容器
docker-compose -f docker-compose.yml up -d
```

```shell
# 改名字
docker tag 760dcbefb9a01b4c09e334d2495521a870c2816fd98daab99f302f7a0dd8c590 registry.cn-beijing.aliyuncs.com/ikcro/rabbitmq:3.12-management
```

```shell
# 推送到阿里云
docker push registry.cn-beijing.aliyuncs.com/ikcro/rabbitmq:3.12-management
```