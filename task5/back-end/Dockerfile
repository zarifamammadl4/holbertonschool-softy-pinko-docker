FROM ubuntu:latest

RUN apt-get update
RUN apt-get upgrade -y

RUN apt-get install -y python3 python3-pip

# Install flask & flask-cors using override flag
RUN pip3 install --break-system-packages flask
RUN pip3 install --break-system-packages flask-cors

WORKDIR /app
COPY ./api.py /app/api.py

CMD ["python3", "api.py"]
