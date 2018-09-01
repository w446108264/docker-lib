FROM jenkins/jnlp-slave:latest
MAINTAINER shengjun <shengjun8486@gmail.com>

RUN cd ~/ \
    && wget http://10.8.126.240:8081/public/users/leo.zhong/shell/docker/debian-android.sh \
    && chmod 700 debian-android.sh \
    && ./debian-android.sh