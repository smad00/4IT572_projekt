FROM alpine:3.11.6

RUN apk add gcc \
            python3 \
            py3-pip \
            libffi \
            openssl

RUN apk add --virtual build-dependencies python3-dev \
            python2-dev \
            libffi-dev \            
            openssl-dev

RUN pip3 install --user ansible

RUN pip3 install --user boto boto3

CMD ["ansible-playbook"]