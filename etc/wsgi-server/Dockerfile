FROM python:3.6.9

ENV PYTHONUNBUFFERED 1

WORKDIR /usr/src/app

COPY requirements.txt requirements.txt

RUN ["pip", "install", "--no-cache-dir", "-r", "requirements.txt"]

COPY ./src /usr/src/app

EXPOSE 3031

CMD ["uwsgi", "--module", "djangodockerexample.wsgi:application", "--master", "--processes", "2", "--die-on-term", "--socket", "wsgi-server:3031"]
