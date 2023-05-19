FROM ubuntu:20.04
LABEL maintainer '(< 0c3x >) Luan Victor (< 0c3x >)'

ENV TZ America/Sao_Paulo
WORKDIR /tmp
RUN apt -o Acquire::Check-Valid-Until=false -o Acquire::Check-Date=false update && \
    ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone && \
    apt install sudo -y && \
    sudo useradd blamer && \
    echo "blamer:password" | sudo chpasswd && \
    apt install -yq tzdata && \
    apt install curl -y && apt install openvpn -y && apt install dos2unix && \
    apt install gcc -y && \
    echo 'blamer ALL=(root) NOPASSWD: /usr/sbin/openvpn' >  /etc/sudoers.d/blamer && \
    echo 'blamer ALL=(root) NOPASSWD: /usr/bin/dos2unix' >>  /etc/sudoers.d/blamer && \
    echo 'blamer ALL=(root) NOPASSWD: /usr/sbin/base64' >>  /etc/sudoers.d/blamer && \
    echo 'Defaults:blamer env_keep += "LD_PRELOAD"' | sudo tee -a /etc/sudoers