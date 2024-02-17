FROM python:3.8-slim-buster

WORKDIR /python-docker


RUN pip3 install Flask

COPY . .

RUN apt-get update && apt-get install procps -y

CMD ["flask", "--app", "index", "run", "--host=0.0.0.0"]
