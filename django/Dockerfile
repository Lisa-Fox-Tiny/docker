FROM python:3.9

WORKDIR /pagination

COPY ./pagination /pagination

RUN pip install -r /pagination/requirements.txt

ENV Project 1

RUN python manage.py migrate


CMD ["gunicorn", "--bind", "0.0.0.0:8000", "pagination.wsgi"]