FROM alpine:3.11.6

RUN apk add gcc \
            python3 \
            python-dev \
            py3-pip \
            libffi \
            libffi-dev \
            openssl \
            openssl-dev

RUN pip3 install --user ansible

RUN pip3 install --user boto boto3

CMD ["ansible-playbook"]