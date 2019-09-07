FROM ubuntu
LABEL maintainer="Kohei <koh@arupaka.net>"
RUN touch /root/FLAG{NEW_WORLD}
RUN touch /root/file1
RUN touch /root/file2
RUN touch /root/file3
RUN mkdir /root/folder1
RUN mkdir /root/folder2
RUN mkdir /root/folder3
RUN sed -i -e "s%http://archive.ubuntu.com/ubuntu/%http://ftp.iij.ad.jp/pub/linux/ubuntu/archive/%g" /etc/apt/sources.list
RUN apt update
RUN apt install -y language-pack-ja-base language-pack-ja
RUN apt install -y tzdata && ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime
ENV LANG ja_JP.UTF-8  
ENV LANGUAGE ja_JP:en  
ENV LC_ALL ja_JP.UTF-8
