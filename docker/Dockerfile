FROM alpine:3.11.6

RUN apk add --update gcc \
            python3 \
            py3-pip \
            libffi \
            openssl

RUN apk add --update --virtual build-dependencies python2-dev \
            python3-dev \            
            libffi-dev \            
            openssl-dev

RUN pip3 install --user ansible

RUN pip3 install --user boto boto3

CMD ["ansible-playbook"]