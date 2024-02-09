FROM python:2.7-stretch

LABEL maintainer="feur25 <feur09@gmail.com>"

RUN apt-get update && apt-get install -y python-dev python3-dev libsasl2-dev libldap2-dev libssl-dev

VOLUME /data

EXPOSE 5000

CMD [ "python", "./student_age.py" ]
