FROM    kalilinux/kali-rolling

LABEL maintainer="breaker <791628659@qq.com>"

ARG TZ="Asia/Shanghai"


RUN echo "deb http://mirrors.aliyun.com/kali kali-rolling main non-free contrib\ndeb-src http://mirrors.aliyun.com/kali kali-rolling main non-free contrib" > /etc/apt/sources.list && \
    apt-get update && \
    apt install -y zsh wget vim git metasploit-framework&& \
    sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)" && \
    apt-get clean
    
WORKDIR /root

CMD ["zsh"]