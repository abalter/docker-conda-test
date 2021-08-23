FROM ubuntu

# install stuff
RUN apt-get update && apt-get install -y vim 

#<------ Can't use environment variable
ARG DOCKER_USER
ARG DOCKER_USER_PASSWORD

# create sudo user
RUN useradd -m -p ${DOCKER_USER_PASSWORD} -s /bin/bash ${DOCKER_USER}
RUN usermod -a -G sudo ${DOCKER_USER}
USER ${DOCKER_USER}
WORKDIR /home/${DOCKER_USER}
