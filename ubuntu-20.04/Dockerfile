FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
	apt-get install -y net-tools procps iproute2 iputils-ping curl && \
	apt-get install -y wget netcat locales tzdata unzip zip procps tcpdump && \
	ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && \
	dpkg-reconfigure -f noninteractive tzdata && \
	locale-gen zh_CN.utf8

ENV TZ=Asia/Shanghai LANG=zh_CN.utf8
