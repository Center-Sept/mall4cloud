FROM anapsix/alpine-java:8_server-jre_unlimited

MAINTAINER center-sept@163.com

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

RUN mkdir -p /mall4cloud-gateway

WORKDIR /mall4cloud-gateway

EXPOSE 8000

ADD ./target/mall4cloud-gateway.jar ./

CMD sleep 1;java -Dfile.encoding=utf-8 -Djava.security.egd=file:/dev/./urandom -jar -Xms512m -Xms512m -Xss384k mall4cloud-gateway.jar