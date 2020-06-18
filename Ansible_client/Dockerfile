FROM python

RUN apt-get update && apt-get install vim \
    ssh -y
RUN echo "root:redhat" | chpasswd

RUN sed -i 's/#PermitRootLogin prohibit-password/PermitRootLogin yes/g' /etc/ssh/sshd_config

EXPOSE 22    

ENTRYPOINT service ssh restart && bash