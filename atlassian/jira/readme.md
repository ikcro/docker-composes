
生成镜像：
```shell
    docker build -t ikcro/jira:7.13.1 .
```

获取许可：
```shell
docker exec -it `docker ps|grep jira|awk '{print $1}'` /bin/bash 
 
cd /opt/atlassian/jira/

java -jar atlassian-agent.jar -p jira -m test@test.com -n BAT -o https://www.visa.vip -s BKOC-MNRR-G5OE-XXGF
```