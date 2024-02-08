FROM python:2.7-stretch

MAINTAINER Quentin feur09@gmail.com

RUN apt-get update -y && apt-get install -y \
    python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev \
    && pip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.14.0

COPY . /app
WORKDIR /app

EXPOSE 5000

CMD [ "python", "./student_age.py" ]