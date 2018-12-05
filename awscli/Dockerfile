#Dockerfile start

FROM centos:latest
MAINTAINER davidadixon@gmail.com

ENV PATH="/root/.local/bin:${PATH}"
RUN yum -y install epel-release
RUN yum -y update 
RUN yum -y install python
RUN yum -y install python-pip 
RUN pip install --upgrade pip
RUN pip install awscli --upgrade --user
RUN pip install saws --user
RUN yum -y install git
RUn yum -y install htop
RUN yum -y install vim
RUN yum -y install wget && yum clean all
RUN wget https://github.com/barnybug/cli53/releases/download/0.8.12/cli53-linux-amd64
RUN mv cli53-linux-amd64 /usr/local/bin/cli53
RUN chmod +x /usr/local/bin/cli53
# ENTRYPOINT ["/bin/echo", "Hello Alex"]