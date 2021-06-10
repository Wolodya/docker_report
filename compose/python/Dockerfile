FROM python:3.9.2

ENV PYTHONUNBUFFERED 1

COPY keyua/requirements.txt requirements.txt
RUN pip install -r /requirements.txt

COPY ./compose/python/entrypoint /entrypoint
RUN chmod +x /entrypoint

COPY ./compose/python/start /start
RUN chmod +x /start

WORKDIR /keyua
