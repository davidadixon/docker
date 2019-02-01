FROM alpine:latest

MAINTAINER Alex Dixon <davidadixon@gmail.com>

RUN apk -v --update add \
python \
py-pip \
groff \
less \
nano \
wget \
git \
&& \
pip install --upgrade pip awscli s3cmd saws && \
mkdir /root/.aws && \
rm /var/cache/apk/*