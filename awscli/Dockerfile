#Dockerfile new1

FROM centos:latest
MAINTAINER davidadixon@gmail.com

ENV PATH="/root/.local/bin:${PATH}"
RUN yum -y install epel-release && \
    yum -y update && \
    yum -y install python && \
    yum -y install python-pip && \
    pip install --upgrade pip && \
    pip install awscli --upgrade --user && \
    pip install saws --user && \
    pip install boto3 && \
    pip install tqdm && \
    yum -y install git && \
    yum -y install htop && \
    yum -y install vim && \
    yum -y install nano && \
    yum -y install ipython && \
    yum -y install jq && \
    yum -y install wget && \
    yum clean all && \
    rm -rf /var/cache/yum && \
    wget https://github.com/barnybug/cli53/releases/download/0.8.12/cli53-linux-amd64 && \
    mv cli53-linux-amd64 /usr/local/bin/cli53 && \
    chmod +x /usr/local/bin/cli53 && \
    wget https://raw.githubusercontent.com/davidadixon/bash_profile/master/bash_profile && \
    mv ~/.bashrc ~/.bashrc_bkup -f && \
    mv bash_profile ~/.bashrc -f && \
    source ~/.bashrc && \
    . ~/.bashrc
# ENTRYPOINT ["/bin/echo", "Hello Alex"]