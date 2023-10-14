FROM python:3.11-alpine

COPY . /app

WORKDIR /app
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

ENV FLASK_APP dock.py
ENV FLASK_RUN_HOST 0.0.0.0

CMD ["python", "-m", "flask", "run"]
EXPOSE 5000