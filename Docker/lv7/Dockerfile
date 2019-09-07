FROM ubuntu
LABEL maintainer="Kohei <koh@arupaka.net>"
RUN sed -i -e "s%http://archive.ubuntu.com/ubuntu/%http://ftp.iij.ad.jp/pub/linux/ubuntu/archive/%g" /etc/apt/sources.list
RUN apt update
RUN apt install -y language-pack-ja-base language-pack-ja
RUN apt install -y tzdata && ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime
ENV LANG ja_JP.UTF-8
ENV LANGUAGE ja_JP:en
ENV LC_ALL ja_JP.UTF-8

RUN mkdir /root/remove-me
