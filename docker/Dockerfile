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

RUN pip install --user ansible

RUN pip install --user boto boto3

#RUN mkdir /ansible && \
#    mkdir -p /etc/ansible && \
#    echo 'localhost' > /etc/ansible/hosts

#WORKDIR /ansible

#CMD ["ansible-playbook", "--version"]