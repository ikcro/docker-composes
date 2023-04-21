# 搭建文档：https://www.iots.vip/post/atlassian-series-crack.html

# 这边仅测试了7版本，其他版本理论上也没啥问题，自行测试一下
FROM cptactionhank/atlassian-jira-software:7.13.1

USER root

# 将破解包加入容器
COPY "atlassian-agent.jar" /opt/atlassian/jira/

# 设置启动加载
RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/jira/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/jira/bin/setenv.sh
