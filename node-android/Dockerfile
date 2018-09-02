FROM jenkins/jnlp-slave:3.23-1
MAINTAINER shengjun <shengjun8486@gmail.com>

RUN cd ~/ \
    && wget http://dl.google.com/android/android-sdk_r24.4.1-linux.tgz \
    && mkdir -p soft/android \
    && mkdir -p soft/android/android-sdk-linux/licenses \
    && tar -xvf android-sdk_r24.4.1-linux.tgz -C soft/android/ \
    && rm -f android-sdk_r24.4.1-linux.tgz

ENV ANDROID_HOME /home/jenkins/soft/android/android-sdk-linux
ENV PATH $PATH:$ANDROID_HOME/tools
ENV PATH $PATH:$ANDROID_HOME/platform-tools

RUN echo "8933bad161af4178b1185d1a37fbf41ea5269c55" >> $ANDROID_HOME/licenses/android-sdk-license \
    && echo "d56f5187479451eabf01fb78af6dfcb131a6481e" >> $ANDROID_HOME/licenses/android-sdk-license