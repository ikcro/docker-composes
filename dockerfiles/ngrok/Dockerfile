# This my first nginx Dockerfile
# Version 1.0

# Base images 基础镜像
FROM centos

#MAINTAINER 维护者信息
MAINTAINER zhangtao

#环境变量
ENV PATH /home/ngrok:$PATH

#ADD  文件放在当前目录下，拷过去会自动解压
ADD ngrok_linux_arm64 /home/ngrok/

#WORKDIR 相当于cd
WORKDIR /home/ngrok

RUN chmod 777 /home/ngrok/ngrok && chmod 777 /home/ngrok/start.sh

#CMD 运行以下命令
CMD start.sh