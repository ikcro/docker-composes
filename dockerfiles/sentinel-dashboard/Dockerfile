# This my first nginx Dockerfile
# Version 1.0

# Base images 基础镜像
FROM openjdk:8

#MAINTAINER 维护者信息
MAINTAINER ikcro

#环境变量
ENV PATH /home/seata/seata-server-1.4.2/bin:$PATH

#ADD  文件放在当前目录下，拷过去会自动解压
#ADD https://github.com/alibaba/Sentinel/releases/download/1.8.3/sentinel-dashboard-1.8.3.jar /home/sentinel-dashboard/
ADD https://gh2.yanqishui.work/https://github.com/seata/seata/releases/download/v1.4.2/seata-server-1.4.2.tar.gz /home/

#WORKDIR 相当于cd
WORKDIR /home/seata/seata-server-1.4.2

#CMD 运行以下命令
CMD java -Dserver.port=8080 -Dcsp.sentinel.dashboard.server=localhost:8080 -Dproject.name=sentinel-dashboard -jar sentinel-dashboard-1.8.3.jar