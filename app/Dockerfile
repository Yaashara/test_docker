FROM python:latest

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /code

RUN python -m venv /venv
RUN pip install -r packages.txt

COPY . /code

RUN cp -a templates /code/venv/Lib/site-packages/flask




