# Dockerfile for remote_node_1 and remote_node_2

FROM ubuntu:latest

# Install necessary packages
RUN apt-get update && apt-get install -y openssh-server sshpass && \
    mkdir /var/run/sshd && \
    echo 'root:docker' | chpasswd && \
    sed -i 's/#PermitRootLogin prohibit-password/PermitRootLogin yes/' /etc/ssh/sshd_config && \
    sed -i 's/#PasswordAuthentication yes/PasswordAuthentication yes/' /etc/ssh/sshd_config && \
    service ssh start

# Expose SSH port
EXPOSE 22

CMD ["/usr/sbin/sshd", "-D"]
