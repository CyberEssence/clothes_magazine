FROM python:3.10.2
ENV PYTHONUNBUFFERED 1
WORKDIR /app
COPY requirements.txt /project/requirements.txt
RUN pip install -r /project/requirements.txt
COPY . /app

CMD python manage.py runserver 0.0.0.0:8000