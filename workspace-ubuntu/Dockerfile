
FROM    ubuntu:latest

LABEL maintainer="breaker <791628659@qq.com>"

ARG TZ="Asia/Shanghai"

RUN apt-get update && \
    apt install -y zsh wget vim git net-tools iputils-ping htop && \
    sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" && \
    apt-get clean
    
WORKDIR /root

CMD ["zsh"]