FROM python:latest

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /code

RUN python -m venv /code/venv
RUN pip install -r /code/packages.txt
RUN pip uninstall wergzeug
RUN pip install wergzeug==0.16.1

COPY . /code

RUN cp -a templates /code/venv/Lib/site-packages/flask