FROM ubuntu

RUN apt update
RUN apt install -y python python3-pip vim
RUN pip3 install flask

COPY app.py /home/app.py

ENTRYPOINT FLASK_APP=app.py flask run --host=0.0.0.0
