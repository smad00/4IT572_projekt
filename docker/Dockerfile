FROM alpine:3.11.6

RUN apk add --update sudo \
            gcc \
            python \
            py-pip \
            libffi \
            openssl \
            ca-certificates \
            sshpass \
            openssh-client \
            rsync

RUN apk add --update --virtual build-dependencies python-dev \
            libffi-dev \
            openssl-dev \
            build-base

RUN pip install ansible

RUN pip install boto boto3

WORKDIR /ansible