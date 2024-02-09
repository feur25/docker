FROM python:2.7-stretch

RUN apt-get update && apt-get install -y python-dev python3-dev libsasl2-dev libldap2-dev libssl-dev

EXPOSE 5000

CMD [ "python", "./student_age.py" ]
