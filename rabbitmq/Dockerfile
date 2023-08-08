FROM rabbitmq:3.12-management

# 安装curl和unzip
RUN apt-get update && \
apt-get install -y curl unzip

# 下载delayed_message_exchange插件
#RUN curl https://github.com/rabbitmq/rabbitmq-delayed-message-exchange/releases/download/v3.12.0/rabbitmq_delayed_message_exchange-3.12.0.ez > rabbitmq_delayed_message_exchange-3.12.0.ez && \
#mv rabbitmq_delayed_message_exchange-3.12.0.ez /opt/rabbitmq/plugins/ \

# 下载delayed_message_exchange插件并移动到正确的目录
RUN curl -LJO https://github.com/rabbitmq/rabbitmq-delayed-message-exchange/releases/download/v3.12.0/rabbitmq_delayed_message_exchange-3.12.0.ez && \
    mv rabbitmq_delayed_message_exchange-3.12.0.ez /opt/rabbitmq/plugins/rabbitmq_delayed_message_exchange-3.12.0.ez


# 启用插件
RUN rabbitmq-plugins enable rabbitmq_delayed_message_exchange