#Dockerfile start

FROM centos:latest
MAINTAINER davidadixon@gmail.com

RUN yum -y update
RUN yum -y install python
RUN yum -y install python-pip
RUN pip install awscli --upgrade --user
RUN pip install saws
ENTRYPOINT ["/bin/echo", "Hello Alex"]