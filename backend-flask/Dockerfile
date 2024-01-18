FROM python:3.9.17-slim-buster

WORKDIR /backend-flask

COPY requirements.txt requirements.txt

RUN pip3 install -r requirements.txt

COPY . .

ENV FLASK_ENV=development

# EXPOSE $(PORT)

CMD ["python", "-m", "flask", "run", "--host=0.0.0.0", "--port=4567"]
