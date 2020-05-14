FROM alpine:3.11.6

RUN apk add python3 \
apk add python-dev \
apk add py3-pip \
apk add libffi \
apk add libffi-dev \
apk add openssl \
apk add openssl-dev \
pip3 install ansible boto boto3

CMD ["ansible-playbook"]