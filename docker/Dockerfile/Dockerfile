FROM centos/httpd:latest
MAINTAINER Rafael Ximenes "rafaximenes1@gmail.com"

RUN yum -y install git
RUN git clone http://softwarepublico.gov.br/gitlab/e-sic-livre/e-sic-livre.git

RUN yum -y install php
RUN yum -y install php-mysqli
RUN mkdir -p /var/www/html/esic
WORKDIR /e-sic-livre
RUN mv * /var/www/html/esic
WORKDIR /var/www/html
RUN -R chmod 777 esic
