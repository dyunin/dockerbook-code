FROM ubuntu:18.04
LABEL maintainer="james@example.com"
ENV REFRESHED_AT 2020-03-10

RUN apt-get -qq update && apt-get -qq install ruby ruby-dev build-essential redis-tools
RUN gem install --no-rdoc --no-ri sinatra json redis

RUN mkdir -p /opt/webapp

EXPOSE 4567

CMD [ "/opt/webapp/bin/webapp" ]
