FROM gcr.io/educative-exec-env/educative-ubuntu-microvm:latest
RUN apt-get update && apt-get install -y docker.io
RUN apt-get install -y curl && apt-get install -y wget
RUN curl -L "https://github.com/docker/compose/releases/download/1.24.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose && chmod +x /usr/local/bin/docker-compose && ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose

RUN apt update &&\
	apt install -y curl git &&\
	curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh &&\
	bash nodesource_setup.sh &&\
	apt install -y nodejs

RUN	git clone https://github.com/rauhaanrizvi/simple-reactjs-app &&\
	cd simple-reactjs-app && npm install
