FROM python:2.7-stretch

RUN apt-get update && apt-get install -y wget

RUN echo "deb http://deb.debian.org/debian stretch main" >> /etc/apt/sources.list && \
    echo "deb http://security.debian.org/debian-security stretch/updates main" >> /etc/apt/sources.list

RUN apt-get update && apt-get install -y \
    python-dev \
    python3-dev \
    libsasl2-dev \
    libldap2-dev \
    libssl-dev

RUN pip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.14.0

EXPOSE 5000

CMD [ "python", "./student_age.py" ]
