.PHONY: build run

all : build run

build:
	docker build -t ubuntuvnc .

run:
	# xhost + 192.168.1.160
	
	docker run -id -p 5900:5900 --name ubuntuvnc ubuntuvnc
	
	# docker run -it --rm -e DISPLAY=192.168.1.160:0 -v /tmp/.X11-unix:/tmp/.X11-unix --name ubuntuvnc ubuntuvnc
	# xhost -
	
connect:
	open vnc://127.0.0.1:5900
	
clean: 
	docker rm ubuntuvnc -f && \
	docker rmi ubuntuvnc
	