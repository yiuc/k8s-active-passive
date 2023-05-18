FROM alpine:latest

RUN apk update && \
    apk --no-cache add \
         bash \
         curl \
         dos2unix

RUN wget -P /usr/bin/ --no-check-certificate https://storage.googleapis.com/kubernetes-release/release/$(wget --no-check-certificate -O - https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl && \
    chmod +x /usr/bin/kubectl