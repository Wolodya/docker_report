FROM python:3.9.2

ENV PYTHONUNBUFFERED 1

COPY keyua/requirements.txt requirements.txt
RUN pip install -r /requirements.txt

COPY ./compose/python/entrypoint /entrypoint
RUN chmod +x /entrypoint

COPY ./compose/python/start /start
RUN chmod +x /start

COPY ./compose/python/celery/worker/start /start-celeryworker
RUN chmod +x /start-celeryworker

COPY ./compose/python/celery/beat/start /start-celerybeat
RUN chmod +x /start-celerybeat

COPY ./compose/python/celery/flower/start /start-flower
RUN chmod +x /start-flower

WORKDIR /keyua

ENTRYPOINT ["/entrypoint"]