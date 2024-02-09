FROM python:2.7-stretch

LABEL maintainer="feur25 <feur09@5gmail.com>"

COPY . /app
WORKDIR /app

RUN apt-get update -y

VOLUME /data

EXPOSE 5000

CMD [ "python", "./student_age.py" ]
