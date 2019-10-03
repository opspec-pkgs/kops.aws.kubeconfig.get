FROM python:3.8.0rc1-alpine

ENV AWSCLI_VERSION=1.16.131

RUN pip install --no-cache-dir awscli==$CLI_VERSION \
    && mkdir /root/.aws \
    && apk add --no-cache curl \
    && curl -LO https://github.com/kubernetes/kops/releases/download/1.14.0/kops-linux-amd64 \
    && chmod +x kops-linux-amd64 \
    && mv kops-linux-amd64 /usr/local/bin/kops

VOLUME /root/.aws/