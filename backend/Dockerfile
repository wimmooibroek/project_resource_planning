FROM python:3.9

WORKDIR /code

COPY . .

RUN pip install --no-cache-dir Django

ENV DOCKERIZE_VERSION v0.6.1
RUN wget https://github.com/jwilder/dockerize/releases/download/v0.6.1/dockerize-linux-amd64-v0.6.1.tar.gz \
  && tar -C /usr/local/bin/ -xzvf dockerize-linux-amd64-v0.6.1.tar.gz

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
