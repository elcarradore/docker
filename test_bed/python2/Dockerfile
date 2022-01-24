FROM python:3.9

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY . . 

EXPOSE 80

RUN apt-get update && apt-get install iputils-ping -y

CMD ["gunicorn", "--bind","0.0.0.0:80","wsgi:app"]
