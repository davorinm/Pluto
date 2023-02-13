FROM ubuntu:22.04

EXPOSE 5900

RUN apt update && \
	apt upgrade -y && \
	apt install -y xvfb x11vnc fluxbox

ENV X11VNC_PASSWORD="password"

COPY entrypoint.sh /opt/entrypoint.sh
RUN chmod +x /opt/entrypoint.sh

ENTRYPOINT /opt/entrypoint.sh
