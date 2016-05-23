FROM ubuntu:14.04

MAINTAINER Enrico Rufnak <enrico@rufnak.de>

RUN apt-get update && \
    apt-get install -y ansible && \
    echo "[local]\nlocalhost ansible_connection=local" > /etc/ansible/hosts

CMD [ "ansible-playbook", "--version" ]