FROM alpine:latest

MAINTAINER Alex Dixon <davidadixon@gmail.com>

RUN apk -v --update add \
python \
py-pip \
less \
&& \
pip install --upgrade pip awscli saws && \
mkdir /root/.aws && \
rm /var/cache/apk/* && \
wget https://raw.githubusercontent.com/davidadixon/bash_profile/master/bash_profile && \
mv ~/.bashrc ~/.bashrc_bkup -f && \
mv bash_profile ~/.bashrc -f && \
source ~/.bashrc && \
. ~/.bashrc