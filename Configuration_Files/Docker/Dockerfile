FROM python:3.9-slim
RUN apt-get update; apt-get install iputils-ping curl -y
WORKDIR /flask-docker

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

COPY . .

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]