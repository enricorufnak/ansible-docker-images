FROM debian:7

MAINTAINER Enrico Rufnak <enrico@rufnak.de>

RUN echo 'deb http://http.debian.net/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list && \
    apt-get update && \
    apt-get install -y ansible && \
    echo "[local]\nlocalhost ansible_connection=local" > /etc/ansible/hosts

CMD [ "ansible-playbook", "--version" ]