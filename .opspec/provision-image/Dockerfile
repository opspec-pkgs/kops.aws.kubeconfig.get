FROM python:3.8.0rc1-alpine

RUN pip install --no-cache-dir awscli \
    && apk add --no-cache curl \
    && curl -LO https://github.com/kubernetes/kops/releases/download/1.14.0/kops-linux-amd64 \
    && chmod +x kops-linux-amd64 \
    && mv kops-linux-amd64 /usr/local/bin/kops
