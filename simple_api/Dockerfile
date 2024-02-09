FROM python:2.7-stretch

MAINTAINER Quentin feur09@gmail.com

RUN apt-get update -y
RUN apt-get install -y python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev

VOLUME /data

COPY . /app
WORKDIR /app

EXPOSE 5000

CMD [ "python", "./student_age.py" ]