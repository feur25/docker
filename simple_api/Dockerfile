FROM python:2.7-stretch

LABEL maintainer="feur25 <feur09@gmail.com>"

COPY . /app

WORKDIR /app

RUN apt update -y && \
    apt install -y python-dev python3-dev libsasl2-dev libldap2-dev libssl-dev && \
    pip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.14.0

VOLUME /data

EXPOSE 5000

CMD [ "python", "./student_age.py" ]
