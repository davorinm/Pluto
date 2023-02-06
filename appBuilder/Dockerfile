FROM ubuntu:22.04

RUN apt update && \
	apt upgrade -y

COPY files/firmware/plutosdr-sysroot-v0.35 /root/sysroot
COPY files/gcc-linaro-7.2.1-2017.11-x86_64_arm-linux-gnueabihf /root/gcc-linaro-7.2.1-2017.11-x86_64_arm-linux-gnueabihf
COPY source /root/source

RUN export PATH=$PATH:/root/gcc-linaro-7.2.1-2017.11-x86_64_arm-linux-gnueabihf/bin
