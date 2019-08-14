FROM node
USER root
RUN echo 'debconf debconf/frontend select Noninteractive' | debconf-set-selections \
&& apt-get update \
&& apt-get install -y software-properties-common \
&& apt-get install -y xsltproc dos2unix indent
