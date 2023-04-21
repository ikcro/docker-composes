

生成镜像：
```shell
docker build -f Dockerfile -t ikcro/confluence:6.15.9 .
```


获取许可：
```shell
docker exec -it `docker ps|grep confluence|awk '{print $1}'` /bin/bash  
cd /opt/atlassian/confluence/
java -jar atlassian-agent.jar -p conf -m test@test.com -n BAT -o https://www.visa.vip -s AAAA-BBBB-CCCC-DDDD

```


页面设置：
数据库链接使用READ-COMMITTED隔离级别
```shell
jdbc:mysql://172.18.0.2:3306/confluence?sessionVariables=tx_isolation='READ-COMMITTED'
```