FROM openjdk:8-jre-slim

ARG mycat_version=1.6

MAINTAINER WilliamWei

ENV MYCAT_VERSION=$mycat_version \
    MYCAT_HOME=/opt/mycat \

ENV PATH=${PATH}:${MYCAT_HOME}/bin

RUN apt-get update && \
    apt-get install -y wget procps && \
    wget http://dl.mycat.io/1.6-RELEASE/Mycat-server-1.6-RELEASE-20161028204710-linux.tar.gz  -O mycat-${MYCAT_VERSION}.tar.gz && \
    mkdir -p ${MYCAT_HOME} && \
    tar -zxvf mycat-${MYCAT_VERSION}.tar.gz && \
    cp -r mycat/* ${MYCAT_HOME} && \
    rm mycat-${MYCAT_VERSION}.tar.gz && \
    rm -r mycat

WORKDIR ${MYCAT_HOME}

VOLUME ${MYCAT_HOME}/conf

EXPOSE 3306

CMD ["mycat", "start"]