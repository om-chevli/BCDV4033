# ./ansible_control/Dockerfile

FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y ansible sshpass openssh-client

RUN echo "root:docker" | chpasswd

CMD ["tail", "-f", "/dev/null"]
