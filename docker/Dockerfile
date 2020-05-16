FROM alpine:3.11.6

RUN apk add --update sudo \
            gcc \
            python \
            py-pip \
            libffi \
            openssl

RUN apk add --update --virtual build-dependencies python-dev \
            libffi-dev \
            openssl-dev \
            build-base

#RUN apk add ansible

RUN pip install ansible

RUN pip install boto boto3

#RUN mkdir /ansible && \
#    mkdir -p /etc/ansible && \
#    echo 'localhost' > /etc/ansible/hosts

WORKDIR /ansible

#CMD ["ansible-playbook", "--version"]