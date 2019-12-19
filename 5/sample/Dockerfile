FROM centos:7.6.1810
MAINTAINER YueYang "yueyang_lateron@163.com"
ENV REFRESHED_AT 2019-12-18
RUN yum -y install epel-release
RUN yum -y install nginx
RUN mkdir -p /var/www/html/website
ADD nginx/global.conf /etc/nginx/conf.d/
ADD nginx/nginx.conf /etc/nginx/nginx.conf
EXPOSE 80
