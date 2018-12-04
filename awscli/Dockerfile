#Dockerfile start

FROM centos:latest
MAINTAINER davidadixon@gmail.com

RUN yum -y update
RUN yum -y install python
RUN curl "https://bootstrap.pypa.io/get-pip.py" -o "get-pip.py"
RUN python get-pip.py --user
RUN export PATH=~/.local/bin:$PATH
RUN source ~/.bash_profile
RUN pip install awscli --upgrade --user
RUN pip install saws --user
RUN yum -y install git
RUN yum -y install wget
RUN wget https://github.com/barnybug/cli53/releases/download/0.8.12/cli53-linux-amd64
RUN mv cli53-linux-amd64 /usr/local/bin/cli53
RUN chmod +x /usr/local/bin/cli53
ENTRYPOINT ["/bin/echo", "Hello Alex"]