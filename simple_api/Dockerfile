FROM python:3
MAINTAINER Samir RAHOU 
RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip install flask flask_httpauth flask_simpleldap python-dotenv
COPY student_age.py /
VOLUME [ "/data" ]
EXPOSE 5000
CMD [ "python", "./student_age.py" ]
