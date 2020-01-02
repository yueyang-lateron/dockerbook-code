FROM centos:7.6.1810
MAINTAINER YueYang "yueyang_lateron@163.com"
ENV REFRESHED_AT 2019-12-18

RUN yum install -y which
RUN gpg2 --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
RUN curl -sSL https://get.rvm.io | bash -s stable
ENV rvm_path /usr/local/rvm
RUN /bin/bash -ci "source '/usr/local/rvm/scripts/rvm'"
RUN rvm install 2.4.1
RUN gem install sinatra json redis
RUN mkdir -p /opt/webapp

EXPOSE 4567
CMD [ "/opt/webapp/bin/webapp" ]
